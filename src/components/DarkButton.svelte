<a class="btn_dark_grey" href="contact.html">{content}
    <svg version="1.1" id="Calque_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
         viewBox="0 0 7.5 10.3" style="enable-background:new 0 0 7.5 10.3;" xml:space="preserve">
                        <style type="text/css">
                            .st0{fill:none;stroke-width:3;}
                        </style>
        <path id="Tracé_16" class="st0" d="M1.2,9.2l4.1-4.1L1.1,1.2"/>
                        </svg>
</a>

<script>
    export let content;
</script>

<style lang="scss">
  @import "static/global";

  .btn_dark_grey{
    -webkit-transition: all 0.3s;
    -moz-transition: all 0.3s;
    -o-transition: all 0.3s;
    transition: all 0.3s;
    border:solid $medium-grey 3px;
    font-family: 'Montserrat', sans-serif;
    font-weight:600;
    position:relative;
    font-size:0.9em;
    color:$medium-grey;
    z-index:1;
    padding: 12px 20px 12px 20px;

    svg{
      width:8px;
      margin-left:20px;
      stroke:$medium-grey;
      -webkit-transition: all 0.5s;
      -moz-transition: all 0.5s;
      -o-transition: all 0.5s;
      transition: all 0.5s;
    }
  }

  .btn_dark_grey:hover{
    color:white;
    text-decoration:none;

    svg{
      stroke:white;
    }
  }

  .btn_dark_grey::after {
    background: $medium-grey;
    display:block;
    content: '';
    position: absolute;
    z-index: -1;
    height: 104%;
    left: -1px;
    top: -1px;
    width: 0;
    -webkit-transition: all 0.3s;
    -moz-transition: all 0.3s;
    -o-transition: all 0.3s;
    transition: all 0.3s;
  }

  .btn_dark_grey:hover:after{
    width: 101%;
  }
</style>
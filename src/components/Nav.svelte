<script>
    import {_, locale, locales} from 'svelte-i18n';
</script>

<style lang="scss">
  nav {
    border-bottom: 1px solid rgba(255, 62, 0, 0.1);
    font-weight: 300;
    padding: 0 1em;
  }

  ul {
    margin: 0;
    padding: 0;
  }

  /* clearfix */
  ul::after {
    content: '';
    display: block;
    clear: both;
  }

  li {
    display: block;
    float: right;
  }

  a {
    text-decoration: none;
    padding: 1em 0.5em;
    display: block;
  }
  .dropdown {
    position: relative;
    display: inline-block;
  }

  .dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    padding: 12px 16px;
    z-index: 1;
  }

  .dropdown:hover .dropdown-content {
    display: block;
  }
</style>

<nav>
    <ul>
        <li><a  href="contact">{$_('nav.contact')}</a></li>
        <li><a rel=prefetch href="blog">{$_('nav.blog')}</a></li>
        <li class="dropdown"><a href="#">{$_('nav.entreprise.name')}</a>
            <div class="dropdown-content">
                <ul>
                    <li><a href="vision">{$_('nav.entreprise.vision')}</a></li>
                    <li><a href="approche">{$_('nav.entreprise.approche')}</a></li>
                    <li><a href="emplois">{$_('nav.entreprise.emplois')}</a></li>
                </ul>
            </div>
        </li>
        <li class="dropdown"><a href="#">{$_('nav.services.name')}</a>
            <div class="dropdown-content">
                <ul>
                    <li><a href="services-applications-cloud-native">{$_('nav.services.cloud')}</a></li>
                    <li><a href="services-embarques-et-iot">{$_('nav.services.iot')}</a></li>
                    <li><a href="services-logiciels-critiques">{$_('nav.services.critique')}</a></li>
                </ul>
            </div>
        </li>
        <li><a  href=".">{$_('nav.accueil')}</a></li>

        <!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
             the blog data when we hover over the link or tap it on a touchscreen -->
    </ul>
</nav>
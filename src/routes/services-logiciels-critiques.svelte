<script>
    import {_, locale, locales} from 'svelte-i18n';
    import {Row, Col, Button} from 'sveltestrap/src';
    import Paragraphe from '../components/Paragraphe.svelte';
    import CriticalTile from '../components/CriticalTile.svelte';
    import DarkButton from '../components/DarkButton.svelte';
    import { fly } from 'svelte/transition';

    let image1 = 'static/critical_illustr_1.png';

</script>

<style>


</style>

<div class="container">
    <Row>
        <Col xs="12" md="6">
            <Paragraphe titre={$_('critique.titres.0')} contenu={$_('critique.contenus.0')}/>
        </Col>
        <Col xs="12" md="6"><img in:fly="{{ y: 100, duration: 2000 }}" class="img-fluid" src="critical_illustr_1.png"></Col>
        <Col xs="12" md="6">
            <Paragraphe titre={$_('critique.titres.1')} contenu={$_('critique.contenus.1')}/>
        </Col>
        <Col xs="12" md="6">
            <Paragraphe titre={$_('critique.titres.2')} contenu={$_('critique.contenus.2')}/>
        </Col>
        <Col xs="12" md="6">
            <Paragraphe titre={$_('critique.titres.3')} contenu={$_('critique.contenus.3')}/>
        </Col>
        <Col xs="12" md="6">
            <Paragraphe titre={$_('critique.titres.4')} contenu={$_('critique.contenus.4')}/>
        </Col>
    </Row>

    <Row class="m-5">
        <Col xs="12" md="6"><img class="img-fluid" src="critical_illustr_2.png"></Col>
        <Col xs="12" md="6">
            <Paragraphe titre={$_('critique.titres.5')} contenu={$_('critique.contenus.5')}/>
        </Col>
        <Col xs="12" md="6">
            <Paragraphe titre={$_('critique.titres.6')} contenu={$_('critique.contenus.6')}/>
        </Col>
        <Col xs="12" md="6">
            <Paragraphe titre={$_('critique.titres.7')} contenu={$_('critique.contenus.7')}/>
            <Paragraphe titre={$_('critique.titres.8')} contenu={$_('critique.contenus.8')}/>
        </Col>
    </Row>
    <div class="container-fluid m-5">
        <Row>
            <Col xs="12"><h1>{$_('critique.titres.9')}</h1></Col>
            <Col xs="12" class="p-4">
                <DarkButton content="{$_('footer.contact')}"/>
            </Col>
        </Row>
    </div>

    <Row class="m-5">
        <Col xs="12" lg="6"><img class="img-fluid" src="critical_illustr_3.png"></Col>
        <Col xs="12" lg="6">
            <Paragraphe titre={$_('critique.titres.10')} contenu={$_('critique.contenus.10')}/>
        </Col>
    </Row>
    <Row class="m-5">
        <Col xs="12">
            <Paragraphe titre={$_('critique.titres.11')}/>
        </Col>
        <Col xs="12" md="4">
            <CriticalTile titre="{$_('critique.normes.1.titre')}" soustitre="{$_('critique.normes.1.domaine')}"/>
        </Col>
        <Col xs="12" md="4">
            <CriticalTile titre="{$_('critique.normes.2.titre')}" soustitre="{$_('critique.normes.2.domaine')}"/>
        </Col>
        <Col xs="12" md="4">
            <CriticalTile titre="{$_('critique.normes.3.titre')}" soustitre="{$_('critique.normes.3.domaine')}"/>
        </Col>
        <Col xs="12" md="4">
            <CriticalTile titre="{$_('critique.normes.4.titre')}" soustitre="{$_('critique.normes.4.domaine')}"/>
        </Col>
        <Col xs="12" md="4">
            <CriticalTile titre="{$_('critique.normes.5.titre')}" soustitre="{$_('critique.normes.5.domaine')}"/>
        </Col>
        <Col xs="12" md="4">
            <CriticalTile titre="{$_('critique.normes.6.titre')}" soustitre="{$_('critique.normes.6.domaine')}"/>
        </Col>
        <Col xs="12" md={{ size: '4', offset: 4 }}>
            <CriticalTile titre="{$_('critique.normes.7.titre')}"/>
        </Col>
    </Row>
    <Row  class="m-5">
        <Col xs="12">
            <Paragraphe titre={$_('critique.titres.12')}/>
        </Col>
        <Col xs="12" lg="6">
            <Paragraphe titre={$_('critique.titres.13')} contenu={$_('critique.contenus.13')}/>
        </Col>
        <Col xs="12" lg="6">
            <Paragraphe titre={$_('critique.titres.14')} contenu={$_('critique.contenus.14')}/>
        </Col>
        <Col xs="12"><p>{$_('critique.contenus.14')}</p></Col>
    </Row>
    <Row >
        <Col xs="12" md="3"><img class="img-fluid" src="client_logo_thales.svg"></Col>
        <Col xs="12" md="3"><img class="img-fluid" src="client_logo_safran.png"></Col>
        <Col xs="12" md="3"><img class="img-fluid" src="client_logo_schneider.png"></Col>
        <Col xs="12" md="3"><img class="img-fluid" src="client_logo_bpa.jpg"></Col>
    </Row>
    <Row>
        <Col xs="12" md="3"><img class="img-fluid" src="client_logo_vinci.png"></Col>
        <Col xs="12" md="3"><img class="img-fluid" src="client_logo_schneider.png"></Col>
        <Col xs="12" md="3"><img class="img-fluid" src="client_logo_adacore.png"></Col>
        <Col xs="12" md="3"><img class="img-fluid" src="client_logo_hexo.svg"></Col>
    </Row>
    <div class="container-fluid m-5">
        <Row>
            <Col xs="12"><h1>{$_('critique.titres.15')}</h1></Col>
            <Col xs="12">
                <DarkButton content="{$_('footer.contact')}"/>
            </Col>
        </Row>
    </div>
</div>
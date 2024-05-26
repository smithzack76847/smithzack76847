from yattag import Doc

doc, tag, text = Doc().tagtext()

doc.asis('<!DOCTYPE html>')
with tag('html'):
    with tag('head'):
        doc.asis('<!-- Site made with Mobirise Website Builder v5.9.18, https://mobirise.com -->')
        doc.stag('meta', charset='UTF-8')
        doc.stag('meta', **{'http-equiv': 'X-UA-Compatible', 'content': 'IE=edge'})
        doc.stag('meta', name='generator', content='Mobirise v5.9.18, mobirise.com')
        doc.stag('meta', name='twitter:card', content='summary_large_image')
        doc.stag('meta', name='twitter:image:src', content='assets/images/index-meta.png')
        doc.stag('meta', property='og:image', content='assets/images/index-meta.png')
        doc.stag('meta', name='twitter:title', content='Trezor.io/Start® - Starting Up Your Device®')
        doc.stag('meta', name='viewport', content='width=device-width, initial-scale=1, minimum-scale=1')
        doc.stag('link', rel='shortcut icon', href='assets/images/trezor-io-start-logo-128x128.png', type='image/x-icon')
        doc.stag('meta', name='description', content='Trezor.io/start - Secure your cryptocurrency with Trezor, the ultimate hardware wallet solution. Get started easily with our step-by-step guide, ensuring top-notch security for your digital assets.')
        with tag('title'):
            text('Trezor.io/Start® - Starting Up Your Device®')
        doc.stag('link', rel='stylesheet', href='assets/bootstrap/css/bootstrap.min.css')
        doc.stag('link', rel='stylesheet', href='assets/bootstrap/css/bootstrap-grid.min.css')
        doc.stag('link', rel='stylesheet', href='assets/bootstrap/css/bootstrap-reboot.min.css')
        doc.stag('link', rel='stylesheet', href='assets/theme/css/style.css')
        doc.stag('link', rel='preload', href='https://fonts.googleapis.com/css2?family=Inter+Tight:wght@400;700&display=swap&display=swap', as_='style', onload="this.onload=null;this.rel='stylesheet'")
        with tag('noscript'):
            doc.stag('link', rel='stylesheet', href='https://fonts.googleapis.com/css2?family=Inter+Tight:wght@400;700&display=swap&display=swap')
        doc.stag('link', rel='preload', as_='style', href='assets/mobirise/css/mbr-additional.css?v=OMRmLq')
        doc.stag('link', rel='stylesheet', href='assets/mobirise/css/mbr-additional.css?v=OMRmLq', type='text/css')
    
    with tag('body'):
        with tag('section', **{'data-bs-version': '5.1', 'class': 'image03 cid-udMYltwOI1', 'id': 'image04-0'}):
            with tag('div', klass='image-block m-auto'):
                with tag('a', href='https://trezor.io/start', target='_blank'):
                    doc.stag('img', src='assets/images/trezor-suite-app-official-congrats-on-your-new-trezor-1-1280x5419.webp', alt='trezor.io/start')
        
        with tag('section', klass='display-7', style='padding: 0;align-items: center;justify-content: center;flex-wrap: wrap;align-content: center;display: flex;position: relative;height: 4rem;'):
            with tag('a', href='https://mobiri.se/3249866', style='flex: 1 1;height: 4rem;position: absolute;width: 100%;z-index: 1;'):
                doc.stag('img', alt='', style='height: 4rem;', src='data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==')
            with tag('p', klass='display-7', style='margin: 0;text-align: center;'):
                text('\u2004')
        
        doc.stag('script', src='assets/bootstrap/js/bootstrap.bundle.min.js')
        doc.stag('script', src='assets/smoothscroll/smooth-scroll.js')
        doc.stag('script', src='assets/ytplayer/index.js')
        doc.stag('script', src='assets/theme/js/script.js')

# Print the generated HTML
print(doc.getvalue())

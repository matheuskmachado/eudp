<html>
    <body>
        <script type='text/javascript'>
            function initEmbeddedMessaging() {
                try {
                    embeddedservice_bootstrap.settings.language = 'pt_BR';

                    window.addEventListener("onEmbeddedMessagingReady", () => {

                        console.log("onEmbeddedMessagingReadyEUDP>> ");
                    });

                    embeddedservice_bootstrap.init(
                        '00D1U000000xbd2',
                        'CRC_Eudora',
                        'https://grupoboticario.my.site.com/ESWCRCEudora1700594760340',
                        {
                            scrt2URL: 'https://grupoboticario.my.salesforce-scrt.com'
                        }
                    );
                } catch (err) {
                    console.error('Error loading Embedded Messaging: ', err);
                }
            };
        </script>
        <script type='text/javascript' src='https://grupoboticario.my.site.com/ESWCRCEudora1700594760340/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
    </body>
</html>

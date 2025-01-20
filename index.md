<html>
  <body>
    <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00DIS000002DpEw',
				'Service_Agent_POC',
				'https://sdoagent-demo.my.site.com/ESWServiceAgentPOC1736267574818',
				{
					scrt2URL: 'https://sdoagent-demo.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://sdoagent-demo.my.site.com/ESWServiceAgentPOC1736267574818/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

<script>
        // Define the URL (you can also use window.location.href if needed)
        const url = "https://services.homedepot.com/services/serviceconnect/0121/30339/L222/hd/0bea4470c?source=browse";

        // Code to get dynamic URL from the browser window (uncomment to use)
        // var url = window.location.href;
        // console.log(url);

        // Extracting the part of the URL after 'serviceconnect/'
        const path = url.split("serviceconnect/")[1]; 

        // Split the path by '/'
        const parts = path.split('/');

        // Get the first three parameters
        const firstThreeParams = parts.slice(0, 3);
	const code1 = firstThreeParams[0];
	const code2 = firstThreeParams[1];
	const code3 = firstThreeParams[2];

        // Output the result as separate values in the console
        console.log(code1+'Code 1 > ' + firstThreeParams[0]);
        console.log(code2+'Code 2 > ' + firstThreeParams[1]);
        console.log(code3+'Code 3 > ' + firstThreeParams[2]);
    </script>

  </body>
</html>

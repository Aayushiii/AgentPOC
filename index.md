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

  </body>
</html>

# multi-step-faultrule
A sample proxy to trigger a default fault rule with that will initiate multiple steps

# Instructions
This proxy is meant to imitate the common use case of setting a default error rule with multiple steps/policies within it. In this example, the error is caused by a failed API Key security requirement and the fault rule steps are to make a service callout to mock the use case of sending a notice of failure to an external system and an assign message policy to customize the error response sent back to the user/client.

To use this repo download errorHandlingMultiStep.zip to your local computer, navigate to Apigee Dashboard > API Proxies > Create New > Upload Proxy Bundle, and upload the zip file there. Once the proxy is deployed simple call it without the required API Key to kick off the default fault rule.
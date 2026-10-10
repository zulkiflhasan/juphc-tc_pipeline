# Question 6 — IBM Cloud Code Engine deployment evidence

**Status: awaiting genuine IBM Cloud CLI output.** This guide is not evidence that the app has been deployed.

## Grading requirements

The application-details output must include:
- Name
- ID (application ID)
- Project Name
- **Project ID**
- **Age**
- **Created** (creation timestamp)
- Status
- URL
- Image and Port where shown

## Obtain and save verified output

Run in an authenticated IBM Cloud Shell session:

```bash
ibmcloud login --sso
ibmcloud target -r us-south
ibmcloud ce project select --name tax-calculator-project
ibmcloud ce application get --name tax-calculator 2>&1 | tee 06-deployed-on-cloud
cat 06-deployed-on-cloud
```

If your actual project or region is different, select the real values before the application-get command. If the application is missing, do not invent deployment details: deploy it first.

Only submit the contents of `06-deployed-on-cloud` if it is real output from IBM Cloud and includes Project ID, Age and Created. Do not copy the placeholder identifiers and `example.us-south.codeengine.app` URL from a sample.

The assessment Q6 requests terminal output, not a GitHub link. The existence of this repository cannot itself substantiate an IBM Cloud deployment.

After capturing evidence you may add your actual output file to this repository, provided it contains no secrets or sensitive metadata you do not want public.

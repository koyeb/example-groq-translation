<div align="center">
  <a href="https://koyeb.com">
    <img src="https://www.koyeb.com/static/images/icons/koyeb.svg" alt="Logo" width="80" height="80">
  </a>
  <h3 align="center">Koyeb Serverless Platform</h3>
  <p align="center">
    Deploy a Groq translation application on Koyeb
    <br />
    <a href="https://koyeb.com">Learn more about Koyeb</a>
    ·
    <a href="https://koyeb.com/docs">Explore the documentation</a>
    ·
    <a href="https://koyeb.com/tutorials">Discover our tutorials</a>
  </p>
</div>


## About Koyeb and the Groq translation application example

Koyeb is a developer-friendly serverless platform to deploy apps globally. No-ops, servers, or infrastructure management required.

This repository contains a language translation application built using Groq, speech-to-text (STT), and text-to-speech (TTS) technologies.  It allows the user to record audio in English, transcribe it, translate it into a different language, and then play it back in audio in the new language.

This example application is designed to show how real-time language translation applications using Groq can be deployed on Koyeb.

## Getting Started

Follow the steps below to deploy and run the Groq language translation application on your Koyeb account.

### Requirements

You need:

* a Koyeb account to successfully deploy and run this application. If you don't already have an account, you can sign-up for free [here](https://app.koyeb.com/auth/signup).
* a [Groq API key](https://console.groq.com/keys) so our application can leverage the platform's AI models.

### Deploy using the Koyeb button

The fastest way to deploy the Groq language translation application is to click the **Deploy to Koyeb** button below.

[![Deploy to Koyeb](https://www.koyeb.com/static/images/deploy/button.svg)](https://app.koyeb.com/deploy?name=example-groq-translation&type=git&repository=koyeb%2Fexample-groq-translation&branch=main&run_command=streamlit+run+main.py&instance_type=small&env%5BGROQ_API_KEY%5D=CHANGE_ME&ports=8501%3Bhttp%3B%2F&builder=buildpack)

Clicking on this button brings you to the Koyeb App creation page with everything pre-set to launch this application.  Modify the value of the `GROQ_API_KEY` environment value with your own key and launch the application.

_To modify this application example, you will need to fork this repository. Checkout the [fork and deploy](#fork-and-deploy-to-koyeb) instructions._

### Fork and deploy to Koyeb

If you want to customize and enhance this application, you need to fork this repository.

If you used the **Deploy to Koyeb** button, you can simply link your service to your forked repository to be able to push changes.
Alternatively, you can manually create the application as described below.

On the [Koyeb Control Panel](https://app.koyeb.com/), on the **Overview** tab, click the **Create Web Service** button to begin.

1. Select **GitHub** as the deployment method.
2. In the repositories list, select the repository you just forked.
3. In the **Builder** section, enable the **override** toggle associated with the **Run command** and enter `streamlit run main.py` in the field.
4. Under **Environment variables**, click **Add variable** to add your Groq API key as `GROQ_API_KEY`.
5. Under **Exposing your service**, change the port selection to port 8501, as used by Streamlit.
6. In the **Instance** section, select an Instance of type **Small** or larger.
7. Under **App and Service names**, rename your App to whatever you'd like. For example, `groq-translation`. Note the name will be used to create the public URL for this app. You can [add a custom domain](https://www.koyeb.com/docs/run-and-scale/domains) later if you'd like.
8. Finally, click **Deploy**.

You will be taken to the deployment page where you can follow the build of your application. Once the build is completed, your application is being deployed and you will be able to access it via `<YOUR_APP_NAME>-<YOUR_ORG_NAME>.koyeb.app`.

## Contributing

If you have any questions, ideas or suggestions regarding this application sample, feel free to open an [issue](https://github.com/koyeb/example-groq-translation/issues) or fork this repository and open a [pull request](https://github.com/koyeb/example-groq-translation/pulls).

## Contact

[Koyeb](https://www.koyeb.com) - [@gokoyeb](https://twitter.com/gokoyeb) - [Slack](http://slack.koyeb.com/)

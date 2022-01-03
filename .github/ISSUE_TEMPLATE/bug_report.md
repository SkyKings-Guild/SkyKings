name: Bug Report
description: Something not working properly? Tell us about it!
labels: [unconfirmed bug]
body:
  - type: markdown
    attributes:
      value: >
        Thanks for taking the time to fill out this bug report.
        If you want real-time support, consider joining our Discord at https://discord.gg/skykings instead.

        Please note that this form is for bugs only!
  - type: input
    attributes:
      label: Summary
      description: >
        A simple summary of your bug report
    validations:
      required: true
  - type: textarea
    attributes:
      label: Reproduction Steps
      description: >
         What you did to make it happen.
    validations:
      required: true
  - type: textarea
    attributes:
      label: Expected Results
      description: >
        What did you expect to happen?
    validations:
      required: true
  - type: textarea
    attributes:
      label: Actual Results
      description: >
        What actually happened?
    validations:
      required: true
  - type: textarea
    attributes:
      label: Additional Context
      description: If there is anything else to say, please do so here.

swagger: "2.0"
x-collection-name: AWS Config
x-complete: 1
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartConfigurationRecorder:
    get:
      summary: Start Configuration Recorder
      description: Starts recording configurations of the AWS resources you have selected
        to record in your AWS account.
      operationId: startConfigurationRecorder
      x-api-path-slug: actionstartconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorderName
        description: The name of the recorder object that records each configuration
          change made to the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders
  /?Action=StartConfigRulesEvaluation:
    get:
      summary: Start Config Rules Evaluation
      description: Runs an on-demand evaluation for the specified Config rules against
        the last known configuration state of the resources.
      operationId: startConfigRulesEvaluation
      x-api-path-slug: actionstartconfigrulesevaluation-get
      parameters:
      - in: query
        name: ConfigRuleNames
        description: The list of names of Config rules that you want to run evaluations
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Evaluations
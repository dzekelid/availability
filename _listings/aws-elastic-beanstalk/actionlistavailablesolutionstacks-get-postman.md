{
  "info": {
    "name": "AWS Elastic Beanstalk API List Available Solution Stacks",
    "_postman_id": "e0136bcb-f30d-48dc-8616-cb549006827f",
    "description": "Returns a list of the available solution stack names.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environments",
      "item": [
        {
          "id": "5b4caad9-c534-43a7-a455-6c20ebd3d989",
          "name": "abortEnvironmentUpdate",
          "request": {
            "url": "http://example.com/api/?Action=AbortEnvironmentUpdate?EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels in-progress environment configuration update or application version\n      deployment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68091692-105d-4826-af66-fceb88cfda91"
            }
          ]
        },
        {
          "id": "5334ba1a-a9ec-400c-820f-6a872b42bb8e",
          "name": "applyEnvironmentManagedAction",
          "request": {
            "url": "http://example.com/api/?Action=ApplyEnvironmentManagedAction?ActionId=ActionId&EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a scheduled managed action immediately."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87c19d59-eb56-4bda-9d65-da29cbcbe76d"
            }
          ]
        },
        {
          "id": "7c9eb12b-61a3-43b4-9cf4-80fed742c789",
          "name": "composeEnvironments",
          "request": {
            "url": "http://example.com/api/?Action=ComposeEnvironments?ApplicationName=ApplicationName&GroupName=GroupName&VersionLabels.member.N=VersionLabels.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create or update a group of environments that each run a separate component of a single\n      application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee943b36-970d-4df8-a1c0-72672564e9fb"
            }
          ]
        },
        {
          "id": "f77ea02d-c87e-4ba3-bbd6-3ded23fb29e1",
          "name": "createEnvironment",
          "request": {
            "url": "http://example.com/api/?Action=CreateEnvironment?ApplicationName=ApplicationName&CNAMEPrefix=CNAMEPrefix&Description=Description&EnvironmentName=EnvironmentName&GroupName=GroupName&OptionSettings.member.N=OptionSettings.member.N&OptionsToRemove.member.N=OptionsToRemove.member.N&SolutionStackName=SolutionStackName&Tags.member.N=Tags.member.N&TemplateName=TemplateName&Tier=Tier&VersionLabel=VersionLabel",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Launches an environment for the specified application using the specified\n      configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47690746-4415-43ae-8d6a-3e9741a94f99"
            }
          ]
        },
        {
          "id": "91016b75-38cc-4d29-887b-8757d15dd2ce",
          "name": "deleteEnvironmentConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEnvironmentConfiguration?ApplicationName=ApplicationName&EnvironmentName=EnvironmentName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the draft configuration associated with the running environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5923fd1-207e-41d7-8913-8716dfd1f199"
            }
          ]
        },
        {
          "id": "76524592-f866-4e60-9fa0-7ba869434ddc",
          "name": "describeEnvironmentHealth",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEnvironmentHealth?AttributeNames.member.N=AttributeNames.member.N&EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the overall health of the specified environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b9cfcaa-aee8-4ec2-8d12-b7ba70aa2479"
            }
          ]
        },
        {
          "id": "f0228ac7-3235-45c9-a344-c07f3de8ae79",
          "name": "describeEnvironmentManagedActionHistory",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEnvironmentManagedActionHistory?EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName&MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists an environment's completed and failed managed actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "967c19c6-9b66-4ee5-bffe-cddd3248e579"
            }
          ]
        },
        {
          "id": "baa36817-cbc8-4ab5-9842-97fd63767d57",
          "name": "describeEnvironmentManagedActions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEnvironmentManagedActions?EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName&Status=Status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists an environment's upcoming and in-progress managed actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "767e7b09-f651-4545-89e6-53f0ce5ead46"
            }
          ]
        },
        {
          "id": "0961d55b-e020-4b3a-a3da-3b25b0ba815c",
          "name": "describeEnvironmentResources",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEnvironmentResources?EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns AWS resources for this environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "263f6b3c-ff02-4e83-b60e-0d220187e1cf"
            }
          ]
        },
        {
          "id": "7bac2323-d74e-4470-9985-d2f929c369a0",
          "name": "describeEnvironments",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEnvironments?ApplicationName=ApplicationName&EnvironmentIds.member.N=EnvironmentIds.member.N&EnvironmentNames.member.N=EnvironmentNames.member.N&IncludedDeletedBackTo=IncludedDeletedBackTo&IncludeDeleted=IncludeDeleted&VersionLabel=VersionLabel",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns descriptions for existing environments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2faa8024-5775-455e-a501-975432288edd"
            }
          ]
        }
      ]
    },
    {
      "name": "DNS",
      "item": [
        {
          "id": "459cb06d-7673-4eac-af0d-1bfba47d82c2",
          "name": "checkDNSAvailability",
          "request": {
            "url": "http://example.com/api/?Action=CheckDNSAvailability?CNAMEPrefix=CNAMEPrefix",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks if the specified CNAME is available."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c2e5f27-ea37-482b-aced-3942bb85d938"
            }
          ]
        }
      ]
    },
    {
      "name": "Applications",
      "item": [
        {
          "id": "0a666a1f-e106-4db6-91c7-80f88c56d69f",
          "name": "createApplication",
          "request": {
            "url": "http://example.com/api/?Action=CreateApplication?ApplicationName=ApplicationName&Description=Description&ResourceLifecycleConfig=ResourceLifecycleConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an application that has one configuration template named default\n      and no application versions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9815b960-a5c0-4f15-b5c6-80d6e8539991"
            }
          ]
        },
        {
          "id": "623d7edf-f1a9-4147-823e-7380da2dba47",
          "name": "createApplicationVersion",
          "request": {
            "url": "http://example.com/api/?Action=CreateApplicationVersion?ApplicationName=ApplicationName&AutoCreateApplication=AutoCreateApplication&BuildConfiguration=BuildConfiguration&Description=Description&Process=Process&SourceBuildInformation=SourceBuildInformation&SourceBundle=SourceBundle&VersionLabel=VersionLabel",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an application version for the specified application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79effca1-84f0-4de6-8202-a40d4a1ef679"
            }
          ]
        },
        {
          "id": "330046bc-37e1-49cf-a560-20de3e7505c9",
          "name": "deleteApplication",
          "request": {
            "url": "http://example.com/api/?Action=DeleteApplication?ApplicationName=ApplicationName&TerminateEnvByForce=TerminateEnvByForce",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified application along with all associated versions and\n      configurations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0097425-b579-40ca-b5e4-61bc70db3e6e"
            }
          ]
        },
        {
          "id": "a5364d1d-6e5a-4911-9052-a4bed1a34d1b",
          "name": "describeApplications",
          "request": {
            "url": "http://example.com/api/?Action=DescribeApplications?ApplicationNames.member.N=ApplicationNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the descriptions of existing applications."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38d14a1a-85ec-4684-8c39-3c3ec5b02b70"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Templates",
      "item": [
        {
          "id": "21ef2148-1fdd-454d-9a62-177f1f630b42",
          "name": "createConfigurationTemplate",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationTemplate?ApplicationName=ApplicationName&Description=Description&EnvironmentId=EnvironmentId&OptionSettings.member.N=OptionSettings.member.N&SolutionStackName=SolutionStackName&SourceConfiguration=SourceConfiguration&TemplateName=TemplateName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08f1e310-f2fe-4e18-aef1-9bf1bcdece84"
            }
          ]
        },
        {
          "id": "d0130bc7-9fde-488f-82fb-62ce8889195c",
          "name": "deleteConfigurationTemplate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationTemplate?ApplicationName=ApplicationName&TemplateName=TemplateName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified configuration template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f378857e-c603-4a51-a743-7efff5a8ced4"
            }
          ]
        }
      ]
    },
    {
      "name": "Storage Location",
      "item": [
        {
          "id": "71d11d7b-70e4-4340-9051-968829774c6b",
          "name": "createStorageLocation",
          "request": {
            "url": "http://example.com/api/?Action=CreateStorageLocation?S3Bucket=S3Bucket",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the Amazon S3 storage location for the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65b0efc7-74ed-4d84-a640-dd74e29ed39e"
            }
          ]
        }
      ]
    },
    {
      "name": "Application Version",
      "item": [
        {
          "id": "4a5aa4b9-ef15-465f-b2e2-4d59b1029a04",
          "name": "deleteApplicationVersion",
          "request": {
            "url": "http://example.com/api/?Action=DeleteApplicationVersion?ApplicationName=ApplicationName&DeleteSourceBundle=DeleteSourceBundle&VersionLabel=VersionLabel",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified version from the specified application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67d33246-022c-4577-a71a-9674eed08063"
            }
          ]
        },
        {
          "id": "64d6a220-8b80-491a-8b2d-eba0111d3ccc",
          "name": "describeApplicationVersions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeApplicationVersions?ApplicationName=ApplicationName&MaxRecords=MaxRecords&NextToken=NextToken&VersionLabels.member.N=VersionLabels.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a list of application versions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9eaa567-24bf-42e7-854c-8e028a611696"
            }
          ]
        }
      ]
    },
    {
      "name": "ConfigurationOptions",
      "item": [
        {
          "id": "78bc9466-60e1-4609-9ece-814057d4a3d9",
          "name": "describeConfigurationOptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConfigurationOptions?ApplicationName=ApplicationName&EnvironmentName=EnvironmentName&Options.member.N=Options.member.N&SolutionStackName=SolutionStackName&TemplateName=TemplateName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the configuration options that are used in a particular configuration\n      template or environment, or that a specified solution stack defines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbd54e0a-bbea-48b2-b041-19293ebee1b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Settings",
      "item": [
        {
          "id": "b2be61a9-facd-4799-b6f7-ba885a7a73bc",
          "name": "describeConfigurationSettings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConfigurationSettings?ApplicationName=ApplicationName&EnvironmentName=EnvironmentName&TemplateName=TemplateName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of the settings for the specified configuration set, that is,\n      either a configuration template or the configuration set associated with a running\n      environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f3e6e63-6d2a-43cb-b6e2-5833faa579c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "d3bd8517-38da-42de-b72d-9502608623c9",
          "name": "describeEvents",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEvents?ApplicationName=ApplicationName&EndTime=EndTime&EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName&MaxRecords=MaxRecords&NextToken=NextToken&RequestId=RequestId&Severity=Severity&StartTime=StartTime&TemplateName=TemplateName&VersionLabel=VersionLabel",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of event descriptions matching criteria up to the last 6 weeks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "314f0a2e-73f6-4de4-90d5-178530698ae2"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances Health",
      "item": [
        {
          "id": "494126b9-57a5-4b71-be19-299877745e17",
          "name": "describeInstancesHealth",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancesHealth?AttributeNames.member.N=AttributeNames.member.N&EnvironmentId=EnvironmentId&EnvironmentName=EnvironmentName&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrives detailed information about the health of instances in your AWS Elastic\n      Beanstalk."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89c31948-6ba8-409f-a010-4c610b19cc6e"
            }
          ]
        }
      ]
    },
    {
      "name": "Solution Stacks",
      "item": [
        {
          "id": "a09e2048-453c-4211-96bd-56c15203f8e8",
          "name": "listAvailableSolutionStacks",
          "request": {
            "url": "http://example.com/api/?Action=ListAvailableSolutionStacks?SolutionStackDetails.member.N=SolutionStackDetails.member.N&SolutionStacks.member.N=SolutionStacks.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available solution stack names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6babf57d-97be-459e-9e80-deae52bb8e5e"
            }
          ]
        }
      ]
    }
  ]
}
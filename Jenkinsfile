properties([
  [
    $class: 'ParametersDefinitionProperty',
      parameterDefinitions: [
        [$class: 'hudson.model.ChoiceParameterDefinition', 
          choices: 'stop\napply\ndestroy\nconfigure\nvalidate\napplyonly',
          name: 'operation'
        ],
        [ 
          $class: 'hudson.model.StringParameterDefinition',
          name: 'deployment_name'
        ],
        [ 
          $class: 'hudson.model.PasswordParameterDefinition',
          name: 'crmAdminUserPasswd'
        ],
        [ 
          $class: 'hudson.model.PasswordParameterDefinition',
          name: 'crmServiceUserPasswd'
        ],
        [ 
          $class: 'hudson.model.PasswordParameterDefinition',
          name: 'sqlServiceUserPasswd'
        ],
        [ 
          $class: 'hudson.model.PasswordParameterDefinition',
          name: 'domain_join_user_password'
        ],
        [ 
          $class: 'hudson.model.PasswordParameterDefinition',
          name: 'cert_password'
        ]
      ]
    ],
    [$class: 'BuildDiscarderProperty', strategy: [$class: 'LogRotator',numToKeepStr: '5']]
])

  println "operation = ${operation}\n" +
      "deployment_name = ${deployment_name}\n" +
      "crmAdminUserPasswd = ${crmAdminUserPasswd}\n" +
      "crmServiceUserPasswd = ${crmServiceUserPasswd}\n" +
      "sqlServiceUserPasswd = ${sqlServiceUserPasswd}\n" +
      "domain_join_user_password = ${domain_join_user_password}\n" +
      "cert_password = ${cert_password}"

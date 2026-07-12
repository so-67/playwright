code for install playwright ::
1 - create folder on path
2 - open cmd on folder
3 - enter code on cmd :: 
    npm init playwright@latest
4 - for add my system browser on config file ::
    {
      name: 'chrome',
      use: {
        ...devices['Desktop Chrome'],
        channel: 'chrome',
      },
    },
5 - for exe test type code in terminal :: 
      npx playwright test
6 - npx playwright show-report
7 - for use code generator :: 
    npx playwright codegen --channel=chrome "https://example.com"


    

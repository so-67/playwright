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
///////////////////////////////////////////////////////////////////////////   

newman code ::
npm install -g newman‍‍‍
npm install -g newman-reporter-htmlextra
newman run postman_collection.json -e postman_environment.json -r cli,htmlextra
//////////////////////////////////////////////////////////////////////////////////
var movies = pm.response.json();
pm.environment.set("movieId", movies[0].id);
pm.environment.set("availableSeats", movies[0].availableSeats);
//////////////////////////////////////////////////////////////////////////////////

var sessionInfo = pm.response.json();
pm.environment.set("sessionId", sessionInfo.sessionId);
pm.environment.set("state", sessionInfo.state);

    

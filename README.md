NEW_RELIC_LICENSE_KEY="YOUR LICENSE KEY"
  
YOUR_COMMAND_OPTIONS="flask --app hello run --host=0.0.0.0"
NEW_RELIC_CONFIG_FILE="/home/ubuntu/flask_hello/newrelic.ini" /home/ubuntu/.local/bin/newrelic-admin run-program $YOUR_COMMAND_OPTIONS
  
YOUR_COMMAND_OPTIONS="gunicorn -w 4 -b 0.0.0.0 'hello'"
NEW_RELIC_CONFIG_FILE="/home/ubuntu/flask_hello/newrelic.ini" 
/home/ubuntu/.local/bin/newrelic-admin run-program $YOUR_COMMAND_OPTIONS
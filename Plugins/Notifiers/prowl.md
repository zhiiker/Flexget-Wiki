# *Prowl*
<div class="alert alert-success" role="info">
  
  <span class="glyphicon glyphicon glyphicon-cog"></span>
  &nbsp; Prowl can be used as a part of [notifier](/Plugins/Notifiers) plugin system.
</div>

Send messages to your iPhone using [Prowl](http://prowlapp.com).
## Configuration

| Option |Type|  Description | Default |
| --- | ---| --- |---|
|api_key|text|User's API Key. Can also be a list. **Required**
|title|text|Notification title|Gets default from [notify](/Plugins/Notifiers/notify) plugin|
|message|text| Notification message| Gets default from [notify](/Plugins/Notifiers/notify) plugin
|url|URL|Notification URL | Gets default from [notify](/Plugins/Notifiers/notify) plugin
|application|text|The name of your application or the application generating the event|`FlexGet`
|provider_key|text|Optional	Your provider API key. Only necessary if you have been whitelisted
|priority|numeric| Set message priority. Values between -2 and 2 are accepted.| `0`|
| file_template | text|Name of the template file to use. See [notify](/Plugins/Notifiers/notify) plugin for more details| 

### Example
Get your unique API key [here](/https://prowlapp.com/api_settings.php)

```
prowl:
  api_key: <your apikey>
```
# oauth2
# initially copied from the tutorial: http://www.hascode.com/2016/03/setting-up-an-oauth2-authorization-server-and-resource-provider-with-spring-boot/

Sample client commands:
curl -XPOST -k foo:foosecret@localhost:9000/hascode/oauth/token -d grant_type=password -d client_id=foo -d client_secret=abc123  -d redirect_uri=http://www.hascode.com -d username=bar -d password=barsecret
TOKEN=XXXXXXXXXXXXXXXXXXXXx
curl -H "Authorization: Bearer $TOKEN" http://localhost:9001/resource/
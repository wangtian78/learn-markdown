# This is H1 header
###### This is H6 header

![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)

```java
try (CloseableHttpClient httpClient1 = HttpClients.createDefault();
						CloseableHttpResponse res = httpClient1.execute(postUserInfo)) {
					String result = EntityUtils.toString(res.getEntity());
					logger.log(Level.INFO, "User info results:" + result);
					JSONObject userInfoObj = new JSONObject(result);
					username = userInfoObj.getString("preferred_username");
					name = userInfoObj.getString("displayName");
					userid = userInfoObj.getString("uniqueSecurityName");
					logger.log(Level.INFO, "****** user id: " + userid);
					userInfo = result;
				}
 ```

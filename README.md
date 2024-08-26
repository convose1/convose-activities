# Convose activity guide

 How we pass the user information to your activity, we pass it as params

const src="your_activity_url"
 const url= ${src}?channel_id=${chatId}&user_id=${uuid}&username=${username}&avatar=${avatar.url}


You can parse it like this 
first import useSearchParams at the top of your component
```
import { useSearchParams } from "react-router-dom";
```
inside your component you can access the passed params through the url like this
```
const [searchParams, setSearchParams] = useSearchParams();
 const params = extractParams(searchParams);
```
here is an example how you can design your activity to work with convose.com
[flashCard activity front end](https://github.com/convose1/flashcard-activity-frontend).




Our mission is to add many multiplayer activities and games to Convose, searchable through a popup in the chat:
![Onboarding 129](https://github.com/convose1/convose-activities/assets/20860711/2f393fee-d3db-4a24-ba33-b214fdc1f929)

Eventually, every possible activity/game you can imagine will be there. Our goal is to attract many developers to help us reach this goal by giving them 80% of any profits generated by the activities. Developers can choose when Youtube ads show over the activities:
![Onboarding 124 (8)](https://github.com/convose1/convose-activities/assets/20860711/5c056e32-2ca9-4d2f-a6f6-190d078ae17c)
Or have in-activity purchases or paid activities.

To build an activity for Convose just make a website of that activity, send us the URL and we will show the activity in Convose using Iframe. Ideally it should be responsive 
for both mobile & desktop. For mobile and desktop an activity would look like this:
 ![starting screen](https://github.com/convose1/convose-activities/assets/20860711/5356eb4d-4ad3-4e68-9e58-a7646e6054c8)
![user joined after](https://github.com/convose1/convose-activities/assets/20860711/36c4f99f-5479-41e2-accb-37db7dc3bd6b)


Right now we're just beginning these activities, so there's no formal process yet, we're looking for developers who could talk/work closely with our team. Talk with us by joining our slack here: https://join.slack.com/t/convosecommunity/shared_invite/zt-2drs8s092-o5_JnX3tpjl8Q4zOw0cmSQ or talk with Josh on Convose.

Incase you can't host the website of your activity yourself we can also host it on our server.

First step would be to create the game e.g., [codesandbox.io/](url) and test it with Josh. Then we'll work on integrating it with our platform (we will provide the user information like profile, name, etc ). Then we can test it directly on production to see what the users think. Then we can work on adding the adsense videos so your game can make money.

Hope to work with you!

# React Native Tabbar Interaction

Beautiful Tabbar Interaction with Sliding Inset FABs,
made with React Native.

![tabBar](doc/tabBar.gif)

# Installation

using npm:

```
npm install mindinventory/react-native-tab-bar-interaction
```

using yarn:

```
yarn add mindinventory/react-native-tab-bar-interaction
```

### Supported platform

- Android
- Ios

# Usage

```js

import TabBar from "@mindinventory/react-native-tab-bar-interaction";
...

const tabs = [
  {
    name: 'Home',
    activeIcon: <Icon name="home" color="#fff" size={25} />,
    inactiveIcon: <Icon name="home" color="#4d4d4d" size={25} />
  },
  {
    name: 'list',
    activeIcon: <Icon name="list-ul" color="#fff" size={25} />,
    inactiveIcon: <Icon name="list-ul" color="#4d4d4d" size={25} />
  },
  {
    name: 'camera',
    activeIcon: <Icon name="camera" color="#fff" size={25} />,
    inactiveIcon: <Icon name="camera" color="#4d4d4d" size={25} />
  },
  {
    name: 'Notification',
    activeIcon: <Icon name="bell" color="#fff" size={25} />,
    inactiveIcon: <Icon name="bell" color="#4d4d4d" size={25} />
  },
  {
    name: 'Profile',
    activeIcon: <Icon name="user" color="#fff" size={25} />,
    inactiveIcon: <Icon name="user" color="#4d4d4d" size={25} />
  },

];
...

return (
  <Tabbar
    tabs={tabs}
    tabBarContainerBackground='#fff'
    tabBarBackground='#6699ff'
    activeTabBackground='#6699ff'
    labelStyle={{ color: '#4d4d4d', fontWeight: '600', fontSize: 11 }}
    onTabChange={() => console.log('Tab changed')}
  />
);

```

## Component props

### Tabbar

| prop                      | value    | required/optional | description                                 |
| ------------------------- | -------- | ----------------- | -------------------------------------------- |
| tabs                      | array    | required          | It is user for showing icon and label.       |
| tabBarContainerBackground | string   | required          | Use for change tabBar container color.       |
| tabBarBackground          | string   | required          | Use for change tabBar background color.      |
| activeTabBackground       | string   | required          | Use for change active tab background color.  |
| labelStyle                | style    | required          | Use for apply style on tab label.            |
| onTabChange               | function | required          | Use to perform any action when click on tab. |

### tabs

| prop                      | value     | required/optional | description                                 |
| ------------------------- | --------  | ----------------- | ------------------------------------------- |
| name                      | string    | required          | use for showing tab label.                  |
| activeIcon                | component | required          | Use for showing tab active icon/image.      |
| inactiveIcon              | component | required          | Use for showing tab inactiveIcon icon/image.|


## Dependencies

- `react-native-svg`

# Version Migration

### Version: 2.0.1

How to migrate version **1.0.0** to **2.0.1** [Click here](VERSION_MIGRATION.md).

# LICENSE!

React-native-tabbar-interaction is [MIT-licensed](https://github.com/Mindinventory/react-native-tabbar-interaction/blob/master/LICENSE).

# Let us know!

We’d be really happy if you send us links to your projects where you use our component. Just send an email to sales@mindinventory.com And do let us know if you have any questions or suggestion regarding our work.

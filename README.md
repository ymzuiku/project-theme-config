# Project theme config

## [Scheme A (Recommend)](./src/Scheme-A.json)

- Using `themeType` change App colors and layout;
- Using other params change App workflow and show/hidden components.

```json
{
  "themeType": "HKAA",
  "appName": "HKAA",
  "displayName": "HKAA",
  "isShowFloatButton": true,
  "isShowTabbar": true,
  "shippingMethod": ["dineIn", "pickUp", "delivery"],
  "isCanUseTouristSign": true,
  "pageTypes": {
    "homePageType": "HKAAHomePage",
    "orderListType": "HKAAOrderList"
  }
}
```

## [Scheme B](./src/Scheme-B.json)

- Using `config` params change App workflow and show/hidden components;
- Using `colors` params change App theme colors;
- Using `units` params change App layout, like button size, font size, cell height, navigation height;
- Any one can simply modify the basic style.

```json
{
  "config": {
    "appName": "HKAA",
    "displayName": "HKAA",
    "isShowFloatButton": true,
    "isShowTabbar": true,
    "shippingMethod": ["dineIn", "pickUp", "delivery"],
    "isCanUseTouristSign": true,
    "pageTypes": {
      "homePageType": "HKAAHomePage",
      "orderListType": "HKAAOrderList"
    }
  },
  "colors": {
    "theme": {
      "fillPrimary": "#4F2B1A",
      "fillSecondary": "#4F2B1A",
      "fillPositive": "#4F2B1A",
      "fillNegative ": "#4F2B1A",
      "fillDark": "#4F2B1A",
      "fillSecondaryDark": "#4F2B1A",
      "fillLight": "#ffffff",
      "fillSecondaryLight": "#ece4d7",
      "textPrimary": "4F2B1A",
      "textSecondary": "4F2B1A",
      "textWeek": "4F2B1A",
      "textHint": "4F2B1A",
      "textDisabled": "4F2B1A"
    },
    "components": {
      "activityColor": "#7E46AA",
      "navigationBarBackground": "#7E46AA",
      "navigationBarIconFill": "#7E46AA",
      "navigationBarTilte": "#7E46AA",
      "navigationBarTextButton": "#7E46AA",
      "floatButtonBackground": "#7E46AA",
      "floatButtonIcon": "#ffffff"
    },
    "pages": {
      "storesList": {
        "navigationBarBackground": "#7E46AA",
        "headerTitle": "#7E46AA"
      },
      "sotreMenus": {
        "navigationBarBackground": "#7E46AA",
        "leftMenuTilte": "#7E46AA"
      }
    }
  },
  "units": {
    "theme": {
      "titleFontSize": 40,
      "textFontSize": 24,
      "infoFontSize": 16
    },
    "components": {
      "navigationBarHeight": 44,
      "tabBarHeight": 44,
      "tabBarIconSize": 22,
      "tabBarFontSize": 22,
      "floatButtonSize": 58,
      "floatButtonIconSize": 36
    },
    "pages": {
      "storesList": {
        "floatButtonSize": 58,
        "storesCellHeight": 110,
        "floatButtonIconSize": 36
      },
      "orderList": {
        "floatButtonSize": 40,
        "floatButtonIconSize": 20
      }
    }
  }
}
```

## [Scheme C](./src/Scheme-A.json)

- Using `config` params change App workflow and show/hidden components;
- Using `styles` set all components and pages styles;
- All static styles can hot update online, but only developers know how to modify them;
- Need draw all page again.

```json
{
  "config": {
    "appName": "HKAA",
    "displayName": "HKAA",
    "isShowFloatButton": true,
    "isShowTabbar": true,
    "shippingMethod": ["dineIn", "pickUp", "delivery"],
    "isCanUseTouristSign": true,
    "pageTypes": {
      "homePageType": "HKAAHomePage",
      "orderListType": "HKAAOrderList"
    }
  },
  "styles": {
    "components": {
      "input": {
        "paddingLeft": 8,
        "marginBottom": 8,
        "width": 200,
        "height": 44,
        "backgroundColor": "#f3f3f3",
        "borderRadius": 4
      },
      "button": {
        "borderRadius": 4,
        "justifyContent": "center",
        "alignItems": "center",
        "backgroundColor": "#f33",
        "width": 200,
        "height": 36
      }
    },
    "pages": {
      "homePage": {
        "naviagation": {
          "flexDirection": "column",
          "justifyContent": "center",
          "alignItems": "center",
          "width": "100%",
          "height": " 100%"
        }
      }
    }
  }
}
```

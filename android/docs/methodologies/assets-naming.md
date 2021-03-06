**WOLOX - ANDROID**

#Assets naming guide / Android

## Purpose
The following guide indicates the convention for assets naming used in Wolox.

## Table of contents

1. [General guidelines](#topic-general-guidelines)
2. [Naming convention](#topic-naming-convention)
3. [Naming conventions for the "type" field](#topic-type-conventions)
4. [Naming conventions for the "state" field](#topic-state-conventions)

## <a name="topic-general-guidelines"></a> General guidelines

* Every asset name must be in English
* You should always use **underscores** (`_`) instead of dashes(`-`) or spaces (` `)
* On Android, assets should be separated into folders by screen densities (drawable-hdpi, drawable-xhdpi, drawable-xxhdpi, etc.)
* 9patch assets will be generated by a developer from a base asset provided by a designer
* The main icon of the app (the one used for the launcher) should be named: `ic_launcher_icon`
* The launcher icon should be placed inside `mipmap-xxx` folders in every supported screen density

## <a name="topic-naming-convention"></a> Naming convention

For assets naming, the following convention will be used:
```
type_flow_name_state
```

1. **`type`**: Indicates the rol of the asset (`ic`, `bg`, `img`)
2. **`flow`**: The place where the asset is located in the app (`onboarding`, `profile`, `newsfeed`, etc.)
3. **`name`**: Name that uniquely identifies the asset inside the flow where it belongs (`location`, `message`, `friend_request`)
4. **`state`**: Indicates the state variant of an asset (`on`, `off`, `selected`, etc.)

Examples:
* `ic_profile_edit`
* `bg_onboarding_step_1`
* `img_newsfeed_placeholder`
* `ic_navigation_messages_on`

## <a name="topic-type-conventions"></a> Naming conventions for the `type` field

|    Role    |  Type |       Example       |
|:----------:|:-----:|:-------------------:|
| Icon       | `ic`  | `ic_map_location`   |
| Background | `bg`  | `bg_splash_logo`    |
| Image      | `img` | `img_profile_cover` |

## <a name="topic-state-conventions"></a> Naming conventions for the `state` field

|   Role   |    State   |             Example            |
|:--------:|:----------:|:------------------------------:|
| Active   | `on`       | `ic_chat_new_message_on`       |
| Inactive | `off`      | `ic_chat_new_messag_off`       |
| Disabled | `disabled` | `ic_chat_new_message_disabled` |

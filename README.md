# ![LOGO](logo.png) BBC iPlayer Business Layer **flow**ground Connector

## Description

A generated **flow**ground connector for the BBC iPlayer Business Layer API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/bbci.co.uk/1.0/openapi.json<br/>
Generated at: 2019-06-06T16:11:51+03:00

## API Description

The definitive iPlayer API.

## Authorization

Supported authorization schemes:
- API Key- Basic Authentication

## Actions

### Programmes by initial title character

> Get the Programmes whose title begins with the given initial character.

*Tags:* `A to Z`

#### Input Parameters
* `letter` - _required_ - Letter to search by, a to z or the string '0-9'
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `page` - _required_ - The page index.
* `per_page` - _required_ - The number of results to return.
* `initial_child_count` - _required_ - The depth to return child entities.
* `sort` - _required_ - The sort order of the results.
    Possible values: title.
* `sort_direction` - _required_ - Whether to sort ascending or descending
    Possible values: asc, desc.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.

### Get categories

> Get the list of all the categories in TV & iPlayer.

*Tags:* `Categories`

#### Input Parameters
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.

### Get sub-categories

*Tags:* `Categories`

#### Input Parameters
* `category` - _required_ - The category identifier to return results from.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.

### List all the episodes for a category.

> Get the list of all the episodes for a given category in TV & iPlayer.

*Tags:* `Episodes`

#### Input Parameters
* `category` - _required_ - The category identifier to return results from.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `page` - _required_ - The page index.
* `per_page` - _required_ - The number of results to return.
* `sort` - _optional_ - The sort order of the results.
    Possible values: recent, popular.

### List the highlights for a category.

> Get the editorial highlights of a given category in TV & iPlayer.

*Tags:* `Programmes (TLEOs)`

#### Input Parameters
* `category` - _required_ - The category identifier to return results from.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `mixin` - _optional_ - Request additional data in the output
    Possible values: live, promotions.

### List all the programmes for a category.

> Get the list of all the Programmes (TLEOs) for a given category in TV & iPlayer.

*Tags:* `Programmes (TLEOs)`

#### Input Parameters
* `category` - _required_ - The category identifier to return results from.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `page` - _required_ - The page index.
* `per_page` - _required_ - The number of results to return.

### List all the channels.

> Get the list of all the channels TV & iPlayer.

*Tags:* `Channels`

#### Input Parameters
* `region` - _optional_ - The region to get the channels for.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.

### Get broadcasts by channel

*Tags:* `Programmes (TLEOs)`

#### Input Parameters
* `channel` - _required_ - The channel identifier to limit results to.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `mixin` - _optional_ - Request additional data in the output
    Possible values: live, promotions.
* `per_page` - _required_ - The number of results to return.
* `from` - _optional_ - Time to return results from, e.g. -3h

### List the highlights for a channel.

> Get the editorial highlights of a given channel in TV & iPlayer.

*Tags:* `Channels`

#### Input Parameters
* `channel` - _required_ - The channel identifier to limit results to.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `live` - _optional_ - Whether to include live programmes
* `mixin` - _optional_ - Request additional data in the output
    Possible values: live, promotions.

### Get programmes by channel

*Tags:* `Programmes (TLEOs)`

#### Input Parameters
* `channel` - _required_ - The channel identifier to limit results to.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `page` - _required_ - The page index.
* `per_page` - _required_ - The number of results to return.

### Get schedule by channel

*Tags:* `Channels`

#### Input Parameters
* `channel` - _required_ - The channel identifier to limit results to.
* `date` - _required_ - The date to return the schedule for, yyyy-mm-dd format
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.

### Get Clips

*Tags:* `Episodes`

#### Input Parameters
* `pid` - _required_ - The programme identifier.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.

### Episode for a given pid.

> Get the episode for a given episode identifier.

*Tags:* `Episodes`

#### Input Parameters
* `pid` - _required_ - The programme identifier.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `mixin` - _optional_ - Request additional data in the output
    Possible values: live, promotions.

### Get Onward Journey

> Get Onward Journey (next programme)

*Tags:* `Episodes`

#### Input Parameters
* `pid` - _required_ - The programme identifier.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.

### Get Follow-ups (post-rolls)

*Tags:* `Episodes`

#### Input Parameters
* `pid` - _required_ - The programme identifier.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.

### Get Trailers (pre-rolls)

*Tags:* `Episodes`

#### Input Parameters
* `pid` - _required_ - The programme identifier.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.

### Get programme recommendations

*Tags:* `Episodes`

#### Input Parameters
* `pid` - _required_ - The programme identifier.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `page` - _required_ - The page index.
* `per_page` - _required_ - The number of results to return.

### Get programmes popular

*Tags:* `Episodes`

#### Input Parameters
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `page` - _required_ - The page index.
* `per_page` - _required_ - The number of results to return.
* `initial_child_count` - _required_ - The depth to return child entities.
* `sort` - _required_ - The sort order of the results.
* `sort_direction` - _required_ - Whether to sort ascending or descending
    Possible values: asc, desc.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `mixin` - _optional_ - Request additional data in the output
    Possible values: live, promotions.

### Get episodes by group, brand or series

*Tags:* `Episodes`

#### Input Parameters
* `pid` - _required_ - The programme identifier.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `page` - _required_ - The page index.
* `per_page` - _required_ - The number of results to return.
* `initial_child_count` - _required_ - The depth to return child entities.
* `sort` - _required_ - The sort order of the results.
* `sort_direction` - _required_ - Whether to sort ascending or descending
    Possible values: asc, desc.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `mixin` - _optional_ - Request additional data in the output
    Possible values: live, promotions.

### Get programme highlights

*Tags:* `Programmes (TLEOs)`

#### Input Parameters
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `mixin` - _optional_ - Request additional data in the output
    Possible values: live, promotions.

### Programme for a given pid.

> Get the programme for a given programme identifier.

*Tags:* `Programmes (TLEOs)`

#### Input Parameters
* `pid` - _required_ - The programme identifier.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `initial_child_count` - _required_ - The depth to return child entities.

### Child episodes for a given programme pid.

> Get the child episodes belonging to a given programme identifier.

*Tags:* `Episodes`

#### Input Parameters
* `pid` - _required_ - The programme identifier.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.
* `initial_child_count` - _required_ - The depth to return child entities.

### List all regions

> Get the list of all the regions TV & iPlayer.

*Tags:* `Regions`

#### Input Parameters
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.

### Get schema

*Tags:* `Metadata`

### Search

*Tags:* `Search`

#### Input Parameters
* `q` - _required_ - The term to search for.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.

### Search-suggest

*Tags:* `Search`

#### Input Parameters
* `q` - _required_ - The term to search for.
* `lang` - _required_ - The language for any applicable localised strings.
    Possible values: en, cy, ga, gd, pi.
* `rights` - _required_ - The rights group to limit results to.
    Possible values: mobile, tv, web.
* `availability` - _required_ - Whether to return all, or available programmes
    Possible values: all, available.

### Get status

> Get the current iPlayer business layer status. This tells the caller the status of the iPlayer data, but not necessarily the overall status of the website. In the future it might include the status of the dependent data services within the BBC.

*Tags:* `Metadata`

### Get user store purchases

*Tags:* `User`

#### Input Parameters
* `identity_cookie` - _required_ - The BBC-id cookie value

### Get user store recommendations

*Tags:* `User`

#### Input Parameters
* `identity_cookie` - _required_ - The BBC-id cookie value

### Get user watching

*Tags:* `User`

#### Input Parameters
* `identity_cookie` - _required_ - The BBC-id cookie value

## License

**flow**ground :- Telekom iPaaS / bbci-co-uk-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.

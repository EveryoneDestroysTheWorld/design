# Discord threads
## Title
### Format
```
[design#<issue number>] <issue name>
```

`<issue number>` is the issue number and `<issue name>` is the issue name. Don't put pull request info in the title; if the pull request gets rejected, the issue may still exist.

### Examples
* [design#126] Design feature function: Turf War tutorial
* [design#12] Design feature function: Matchmaking
* [design#108] Design player setting: Volume > Main volume

## Content
### Format
```
See changes: <files changed link>
# Dependencies
* <threads with dependency issue IDs>
# Criteria
## Completion criteria
* <action items from the issue>
## Acceptance criteria
* Complete completion criteria.
* Create this thread.
* Get approval from at least 75% of @Designers (DemoDemons).
# Tracking
* Issue: <issue link>
* Pull request: <pull request link>
```

If a dependency thread doesn't exist, just put the issue number without linking the thread.

### Examples
#### Issue #108
```
See changes: https://github.com/DemoDemons/design/pull/165/files?short_path=d3316fb#diff-d3316fb05acad21be87e618b4f1c79f7645fdcae5421321be89b95df838b2be7
# Dependencies
None
# Criteria
## Completion criteria
* Name the setting.
* Add an internal name to the setting.
* Describe the setting.
* State the setting's type.
* Add a default value to the setting.
* Categorize the setting. If the proper category doesn't exist, make it.
* Publish edits to a new branch. 
## Acceptance criteria
* Complete completion criteria
* Get approval from at least 75% of @Designers (DemoDemons) 
# Tracking
* Issue: https://github.com/DemoDemons/design/issues/108
* Pull request: https://github.com/DemoDemons/design/pull/165
```

#### Issue #126
```
See changes: https://github.com/DemoDemons/design/pull/167/files?short_path=679e335#diff-679e33502065efe2f653721be9175dde2a2afcb80bf3060f938a68a6a92304af
# Dependencies
* #"[design#54] Design game mode premise: Turf War"  
# Criteria
## Completion criteria
* Describe how the tutorial will play out.
* Publish edits to a new branch. 
## Acceptance criteria
* Complete completion criteria
* Get approval from at least 75% of @Designers (DemoDemons) 
# Tracking
* Issue: https://github.com/DemoDemons/design/issues/126
* Pull request: https://github.com/DemoDemons/design/pull/167
```

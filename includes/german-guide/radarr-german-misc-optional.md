<!-- markdownlint-disable MD041-->
??? abstract "Miscellaneous (Optional) - [Click to show/hide]"

    | Custom Format                                                                                                 |                              Score                              | Trash ID                                          |
    | ------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------: | ------------------------------------------------- |
    | [{{ radarr['cf']['bad-dual-groups']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#bad-dual-groups) | {{ radarr['cf']['bad-dual-groups']['trash_scores']['german'] }} | {{ radarr['cf']['bad-dual-groups']['trash_id'] }} |
    | [{{ radarr['cf']['no-rlsgroup']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#no-rlsgroup)         |   {{ radarr['cf']['no-rlsgroup']['trash_scores']['german'] }}   | {{ radarr['cf']['no-rlsgroup']['trash_id'] }}     |
    | [{{ radarr['cf']['obfuscated']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#obfuscated)           |   {{ radarr['cf']['obfuscated']['trash_scores']['german'] }}    | {{ radarr['cf']['obfuscated']['trash_id'] }}      |
    | [{{ radarr['cf']['retags']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#retags)                   |     {{ radarr['cf']['retags']['trash_scores']['german'] }}      | {{ radarr['cf']['retags']['trash_id'] }}          |
    | [{{ radarr['cf']['scene']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#scene)                     |      {{ radarr['cf']['scene']['trash_scores']['german'] }}      | {{ radarr['cf']['scene']['trash_id'] }}           |

    ---

    Breakdown and Why

    - **{{ radarr['cf']['bad-dual-groups']['name'] }}:** [*Optional*] These groups take the original release and add their own language track (e.g. AAC 2.0 Portuguese) as the first track. Afterward, FFprobe would determine that the media file is Portuguese. It's a common rule that you only add the best audio as the main track.
    Also they often even rename the release name into Portuguese.
    - **{{ radarr['cf']['no-rlsgroup']['name'] }}:** [*Optional*] Some indexers strip out the release group which could result in LQ groups being scored incorrectly. For example, a lot of EVO releases end up with a stripped group name. These releases would appear as "upgrades" and could end up getting a decent score after other CFs are scored.
    - **{{ radarr['cf']['obfuscated']['name'] }}:** [*Optional*] Use these only if you wish to avoid renamed releases.
    - **{{ radarr['cf']['retags']['name'] }}:** [*Optional*] Use this if you want to avoid retagged releases. Retagged releases often are not consistent with the quality of the original group's release.
    - :warning: **{{ radarr['cf']['scene']['name'] }}:** [*Optional*] We recommend not using this CF in the German Guide, as it often matches incorrectly due to the German release naming.
<!-- markdownlint-enable MD041-->

------------------------------------------------------------------------

layout: document\
category: Administration\
published: true\
title: "Extensions"\
tags:\
- Extension\
- Admin-side\
- Region\
- Plugins\
---

Extensions
==========

The **Extensions** region is not an out-of-the-box feature. It appears
to the higher [user
roles](http://docs.textpattern.io/administration/user-roles-and-privileges)
if any of the admin-side plugins that employ it are installed.

When relevant, the **Extensions** region will be seen in the
administration navigation from all admin-side views *except* when you
are in context of the **Plugins** panel, even for the administrator.
This behaviour ensures being able to safely deactivate and/or remove
outdated or buggy plugins if they are causing problems. To access the
**Extensions** panels from the **Plugins** panel, move to anywhere else
in the admin-side first, and the \***Extensions** region will appear in
the navigation again.

Plugins that use the Extensions region
--------------------------------------

When you upload a plugin that uses the **Extensions** region, a new
panel option will appear under the region that provides the plugin's
associated functionality or configuration controls. The following table
identifies the *supported* plugins that will do this, and their
corresponding panel labels. (Orphaned or otherwise abandoned plugins are
not listed here, intentionally.)

notextile.

<div itemscope itemtype="http://schema.org/Table">
  Plugin                                                                                                       Extensions panel label[^1]
  ------------------------------------------------------------------------------------------------------------ ----------------------------
  "arc\_redirect":http://forum.textpattern.com/viewtopic.php?id=36705                                          arc\_redirect
  "adi\_notes":http://forum.textpattern.com/viewtopic.php?id=27957                                             adi\_notes
  "asy\_jpcache":http://forum.textpattern.com/viewtopic.php?id=8352                                            ?
  [glz\_custom\_fields](http://forum.textpattern.com/viewtopic.php?id=23996)[^2]                               Custom Fields
  [ied\_plugin\_composer](http://textpattern.org/plugins/588/ied_plugin_composer) (Now maintained by "smd".)   Plugin Composer
  "msd\_admin\_colorpicker":http://forum.textpattern.com/viewtopic.php?id=26742                                ?
  "msd\_google\_map":http://forum.textpattern.com/viewtopic.php?id=30493                                       ?
  "rah\_change\_passwords":http://forum.textpattern.com/viewtopic.php?id=28696                                 ?
  "rah\_post\_versions":http://forum.textpattern.com/viewtopic.php?id=33855                                    ?
  "rah\_tabtor":http://forum.textpattern.com/viewtopic.php?id=34815                                            ?
  "smd\_admin\_themes":http://forum.textpattern.com/viewtopic.php?id=30952                                     ?
  "smd\_bio":http://forum.textpattern.com/viewtopic.php?id=31496                                               Bio config
  "smd\_redirect":https://github.com/Bloke/smd\_redirect                                                       Redirects
  "smd\_tags":http://forum.textpattern.com/viewtopic.php?id=28621                                              smd\_tags
  "smd\_where\_used":http://textpattern.org/plugins/984/smd\_where\_used                                       Where used
  "tru\_tags":http://forum.textpattern.com/viewtopic.php?id=15084                                              ?

notextile.

</div>
Unconventional panel placement
------------------------------

The use of the **Extensions** region is a convention adopted by plugin
developers to put administration-side plugin preferences and other
functional controls in a logical place, and that's a good thing when it
can be done.

Not all administration-side plugins use the **Extensions** region,
however. Some plugins will add their associated admin-side panel in one
of the core regions. This may happen when panel placement is decided
with respect to functional context over convention. Another reason may
be a concern for having too many plugin panels under the **Extensions**
region, though this is likely a moot issue for most Textpattern users.

Either way, it can be a little confusing when your hunting for plugin
panel functionality and it's not where you expect it to be. The issue is
still evolving and plugin developers will likely settle on a standard
process eventually, as well on a convention for creating plugin panel
labels.

[^1]: \[todo:note about UI element guidelines\]

[^2]: This plugin provides functionality that may arrive in core by
    Textpattern version 4.6 or the version after.
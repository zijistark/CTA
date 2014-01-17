CTA: Combat Trait Advancement
===

*A Crusader Kings II Mini-Mod for the Duel Engine*

## Summary ##

This module depends upon some form of the duel engine. Otherwise, there would be no combat traits to advance!

The module provides a combat trait advancement (CTA) system for adult rulers under 50 (and their marshals), AI and player alike. Earn experience points toward trait level-up via personal participation in battles and all types of victorious duels. Dramatically decrease the time taken to advance by applying yourself toward the new, associated set of CKII ambitions to advance your personal combat skills. Age, skill tier, and traits will also impact your rate of progress. You may only advance 1 level beyond that with which you reach adulthood. In the exceptional case that you start with no combat education whatsoever, then you are allowed to advance up to 2 levels, however.

## Compatibility Notes ##

CTA is highly modular, even with respect to its integration with the New Duel Engine.

- The only conflict which an integrator or user combining it at game launch with other mods will likely run into is in the file /common/on_actions/00_on_actions.txt, where CTA adds a single entry to the on_combat_pulse on_action's random_events list.  However, since it is unlikely that this mod will be integrated without the New Duel Engine, NDE's 00_on_actions.txt is the template upon which CTA's added hook is based (rather than vanilla).  Ergo, the 00_on_actions.txt will include the [minimal] additions over vanilla the author of NDE, jordarkelf, has added to enable battlefield duels.

- An override of the New Duel Engine's duel_engine_output_events.txt is provided to provide the combat experience-earning hook from victorious duels.  You may choose to hook CTA up to duels differently (just see cta.10's documentation in events/cta_events.txt for reference on what scopes are required in the event sequence which calls it), or you may even choose to disable duel input by deleting the included duel_engine_output_events.txt (battle participation experience will still work).

- Since CTA is targetted toward its parent mod, Project Balance (which itself integrates the New Duel Engine), it also references some of the extended character traits available in this mod (and other related mods, such as VIET).  For integration/usage with mods that lack these traits ("agile," etc.), the integrator has my assurance that the references to undefined traits won't break a single thing.

## Integration into Other Mods ##

Direct integration of this module in another mod requires the author's express permission, but if you want to do it, please ask.  It's extremely likely that you will receive both my permission and any needed assistance.  If I ever give you my permission for integration into a particular mod, it will be irrevocably yours for that mod.  Standard, liberal, polite reuse policy.

## Contribution ##

Contributions are welcome, particularly if they come in the form of GitHub pull requests.  I will retain ownership of small changes (i.e., may change them later or give someone else permission to integrate the mod into their project).  Large changes will be handled on a case-by-case basis.

## Contacting the Author ##

Please use email.  Related forums and such do work, but email is a much better way to correspond with me.  

Matthew D. Hall - *zijistark*  
azrinon@gmail.com  
Seattle, WA USA (Pacific Time)

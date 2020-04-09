  
 Demote headings (H1 → H2, etc.)
 HTML headings/IDs
 Wrap HTML
 Render HTML tags
Help: Docs, Bugs
<!----- Conversion time: 0.53 seconds.


Using this Markdown file:

1. Cut and paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β21
* Thu Apr 09 2020 07:23:10 GMT-0700 (PDT)
* Source doc: RChip 08: Implementing A Breaking Change Release
----->



## **RChip 08: Implementing A Breaking Change Release (Draft)**


### **Summary: **

SysOps runbook procedure for a breaking change release.


### **Definition:**

Breaking change release is a release that is not backwards compatible.  Should these procedures apply at the root shard level only or all shards? Protocol (data structures and/or API call parameters) breaking changes vs. specific implementation breaking change (scala vs java vs rust) ? Note that multiple language nodes can run in the same shard .. it might improve security and resilience.


### **Validators:**

All bonded node validators must participate in a breaking change release implementation to migrate from the old network to the new network at the block height announced by the Tech Governance team (with inputs from dev team).



1. Breaking change release can be submitted by:
    1. RChain core developers??
    2. Proposers??
2. Editorial, approval & communication
    3. Editorial - review and edit submitted release request.
    4. Approval - review edited release request
    5. Communication
        1. Announcement procedure
            1. Atlassian release notes
            2. Social media
                1. developer.rchain.coop website
                2. Discord - development channel on RChain pub
                3. Telegram - RChain community
                4. Weekly community debrief
                5. RChain YouTube channel
    6. List breaking change release in registry.
        2. Release number
        3. Change classification
            3. Soft update
            4. Breaking change
            5. Hard fork
        4. Implementation date
3. Validator identification - identify which validators are involved in the breaking change release implementation.
4. (Third item - help me here Tomislav, see log: tech governance is needed)
    7. [https://docs.google.com/document/d/1fvxMC6Bt5XwbVaLzYPy6ZPB8KzJvASO2sKRC6ZCPwpI/edit](https://docs.google.com/document/d/1fvxMC6Bt5XwbVaLzYPy6ZPB8KzJvASO2sKRC6ZCPwpI/edit)
5. Metrics
    8. **Block height start **- the block number at which validators must begin to implement a breaking change release.
        5. The recommendation is to treat validators that have not upgraded, as dead nodes until they upgrade
        6. How do we ensure that this doesn’t lead to a network security issue because most validators have not upgraded to the new release at the specified block height?
    9. **Block grace period** - the number of blocks within which validators must implement a breaking change release before being penalized (slashed?)
    10. **Block height slash** - the block number at which validators will be penalized for not completing a breaking change release implementation.
        7. (Incomplete implementation penalty - Slashing?)
6. Issue tree or stream??

<!-- Docs to Markdown version 1.0β21 -->


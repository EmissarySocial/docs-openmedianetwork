# NLNet Grant


## First 6 Months

### Ready Today
* **Federation** via ActivityPub inbox/outbox.  Interoperability with Mastodon, PeerTube, Lemmy, and others.  

* **Search** searchable dataset for content on the local site.  

* **Search: Actor** Remote actors (users and peer servers) can follow individual search queries via ActivityPub.  The search engine publishes an ActivityPub actor for every search query, which broadcasts a live news feed to other ActivityPub actors.

### Small Effort
* **Search: Federation** search services subscribe to content from the remote sites and aggregate content into one result set. (Ben)  

* **Search: Multiple Sources** - Update search engine to handle multiple sources. (Ben)  

* **Search: Delete Sources** - Remove content from search when its source is removed.  Include logic to KEEP "multi-sourced" content if one or more valid sources remain. (Ben)  

* **Search: Respect 'IsIndexable' Flag** - Mastodon has added an `IsIndexable` property that lets individuals choose if their content is indexable by search engines or not.  Confirm that Emissary honors this request, and update if not already implemented. (Ben)  

* **Remote Users** - Update Emissary permissions to allow remote users to be granted "edit" permissions on original articles. (Ben)

### Medium Effort
* **3-Column Layout ** - Create a new template for Emissary that uses OMN's traditional desktop layout. (Michael)  

* **Custom Article Templates** - Create a news article template, possibly based on Qwertylicious articles. Remove "paid" features. (Michael)  

* **Mobile UX** - Update the desktop layout to work on mobile devices. (Michael)  

* **Content Replication: Design** - Design and publish an [Fediverse Enhancement Proposal](https://codeberg.org/fediverse/fep): FEP-de2b Content Replication and Succession Planning (Michael, Ben)  

* **Content Filtering: Coop Integration** - Integration with [Coop](https://roost.tools/coop) content filtering server (Ben, Gov?)  

* **Content Filtering: Initial Rule Sets** - Set up initial boolean logic to represent trust relationships between servers. (Hamish?)  

* **Search Engine Flows** - When a server discovers content on a remote site, allow its search engine to relay this content to other "following" search engines. Stage 1: Per-source setting to activate/deactivate this ability on a source-by-source basis. (Ben)

## Second 6 Months

* **Comments** - Implement article comments based on ActivityPub (Michael)  

* **"Remote Editing"** - UX workflows to allow visitors to remote sites to edit a wiki article by signing in to the primary host. (Michael)  

* **Content Replication: Build** - Build to the design from first 6 months (Ben, Michael?)  

* **Content Filtering: Ongoing Work** - Update content filtering configuration based on lessons from real-world use (Hamish?)  

* **Search Engine Flows** - Add a per-source setting to each peered search server that would allow a server to rebroadcast remote content to search followers on its own search index. This would only happen after remote content has been filtered/approved by the Roost server. (Ben)


## Needs Additional Grant

* Federated Wiki, with synchronization of distributed edits

## ???
Temporal rollback filters
security auditing
accessibility compliance
# Bot commands list

{% hint style="danger" %}
GroundDug only gives the `GD_ADMINISTRATOR` permission to the **Administrators** once it joins the guild. Check the permissions commands for how to add permissions to another user.
{% endhint %}

### Miscellaneous commands

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">Usage and notes</th>
      <th style="text-align:left"><code>GD</code> permission required</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>botinfo</code>
      </td>
      <td style="text-align:left">Returns information about the bot, including guilds, users and shard latency
        information.</td>
      <td style="text-align:left"><code>None</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>help [module]</code>
      </td>
      <td style="text-align:left">
        <p>Provides a list of commands and their usage.</p>
        <p><code>[module]</code> - Which module results are provided back in a list</p>
      </td>
      <td style="text-align:left"><code>None</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>invite</code>
      </td>
      <td style="text-align:left">Receive a private message with a link to invite GroundDug.</td>
      <td style="text-align:left"><code>None</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>setprefix &lt;prefix&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Set a custom prefix for your guild locally. The bot default is <code>g!</code>.</p>
        <p><code>&lt;prefix&gt;</code> - The new prefix the bot will respond to</p>
      </td>
      <td style="text-align:left"><code>administrator</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>userinfo [user]</code>
      </td>
      <td style="text-align:left">
        <p>Obtain information about a user, such as the server join date, account
          age and server roles.</p>
        <p><code>[user]</code> - The user to lookup. If none is provided, message
          author will be used.</p>
        <p><code>user</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a>&lt;code&gt;&lt;/code&gt;</p>
      </td>
      <td style="text-align:left"><code>None</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>badges [user]</code>
      </td>
      <td style="text-align:left">
        <p>Returns the badges given by the bot to a user, signifying the trust level
          the user has in relation to the bot.</p>
        <p><code>[user]</code> - The user to obtain badges for. If none is provided,
          badges for author will be returned.</p>
        <p><code>user</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a>&lt;code&gt;&lt;/code&gt;</p>
      </td>
      <td style="text-align:left"><code>None</code>
      </td>
    </tr>
  </tbody>
</table>### Admin commands

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">Usage and notes</th>
      <th style="text-align:left"><code>GD</code> permission required</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>admin ban &lt;member&gt; [reason]</code>
      </td>
      <td style="text-align:left">
        <p>Bans a member from the guild.</p>
        <p><code>&lt;member&gt;</code> - The member which will be banned from the
          guild</p>
        <p><code>[reason]</code> - The reason the member is being banned from the
          guild</p>
        <p><code>member</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a><code> </code>and in the guild.</p>
      </td>
      <td style="text-align:left"><code>ban_members</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>admin gag &lt;member&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Stops a user from talking in all voice channels.</p>
        <p><code>&lt;member&gt;</code> - The member which will be revoked of <code>Speak</code> permissions
          on all voice channels</p>
        <p><code>member</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a>and in the guild.</p>
      </td>
      <td style="text-align:left"><code>mute_members</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>admin hackban &lt;id&gt; [reason]</code>
      </td>
      <td style="text-align:left">
        <p>Bans a user by their ID from the guild without them needing to be in the
          guild.</p>
        <p><code>&lt;id&gt;</code> - The ID of the user which will be banned from
          the guild</p>
        <p><code>[reason]</code> - The reason the member is being banned from the
          guild</p>
        <p><code>id</code> must be <a href="discord-references.md"><code>discord.id</code></a>&lt;code&gt;&lt;/code&gt;</p>
      </td>
      <td style="text-align:left"><code>ban_members</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>admin mute &lt;member&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Stops a user from typing in all text channels.</p>
        <p><code>&lt;member&gt;</code> - The member which will be revoked of <code>Send Messages</code> permissions
          in all text channels</p>
        <p><code>member</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a>and in the guild.</p>
      </td>
      <td style="text-align:left"><code>mute_members</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>admin purge [amount] [check]</code>
      </td>
      <td style="text-align:left">
        <p>Deletes multiple messages at once from the text channel the command was
          ran in.</p>
        <p><code>[amount]</code> - Specifies the amount of messages to be deleted
          from the text channel, 100 by default.</p>
        <p><code>[check]</code>- What messages should be deleted</p>
        <p><code>check</code> can be either:</p>
        <ul>
          <li><code>member</code> - Removing all messages posted by accounts which aren&apos;t
            classified as bots.</li>
          <li><code>bot</code> - Removing all messages posted by accounts which are bots.</li>
          <li><code>all</code> - Removing messages from any account</li>
        </ul>
        <p>If <code>check</code> is not provided, the <code>all</code> check will be
          used.</p>
      </td>
      <td style="text-align:left"><code>manage_messages</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>admin raid &lt;state&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Enables or disables raid mode.</p>
        <p><code>&lt;state&gt;</code> - Whether raid mode is activated or not.</p>
        <p><code>state</code> must be either <code>true</code> or <code>false</code>
        </p>
        <p><b>What is raid mode?</b>
        </p>
        <p>Raid mode prevents new users from joining your server while it is activated.
          <br
          />This is to allow your moderators to ban any people trying to raid your
          server at any given time.</p>
        <p><b>What will the user see?</b>
        </p>
        <p>If a user joins while a server is being raided, they will receive a message,
          letting them know that the server is currently on lockdown.</p>
        <p><em>In future, GroundDug will also generate an invite for when a user wishes to join when raid mode is deactivated.</em>
        </p>
      </td>
      <td style="text-align:left"><code>administrator</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>admin softban &lt;member&gt; [reason]</code>
      </td>
      <td style="text-align:left">
        <p>Bans a member and immediately unbans them from the guild, removing their
          messages.</p>
        <p><code>&lt;member&gt;</code> - The member which will be banned from the
          guild</p>
        <p><code>[reason]</code> - The reason the member is being banned from the
          guild</p>
        <p><code>member</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a><code> </code>and in the guild.</p>
      </td>
      <td style="text-align:left"><code>ban_members</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>admin ungag &lt;member&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Allows a user from talking again in all voice channels.</p>
        <p><code>&lt;member&gt;</code> - The member which will be given<code>Speak</code> permissions
          on all voice channels</p>
        <p><code>member</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a>and in the guild.</p>
      </td>
      <td style="text-align:left"><code>mute_members</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>admin unmute &lt;member&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Allows a user to typing in all text channels again.</p>
        <p><code>&lt;member&gt;</code> - The member which will be given <code>Send Messages</code> permissions
          in all text channels</p>
        <p><code>member</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a>and in the guild.</p>
      </td>
      <td style="text-align:left"><code>mute_members</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>admin kick &lt;member&gt; [reason]</code>
      </td>
      <td style="text-align:left">
        <p>Kicks a member from the guild.</p>
        <p><code>&lt;member&gt;</code> - The member which will be banned from the
          guild</p>
        <p><code>[reason]</code> - The reason the member is being banned from the
          guild</p>
        <p><code>member</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a><code> </code>and in the guild.</p>
      </td>
      <td style="text-align:left"><code>kick_members</code>
      </td>
    </tr>
  </tbody>
</table>### GD Permissions

| Permission | Permission meaning |
| :--- | :--- |
| `GD_MANAGE_MESSAGES` | Allows users to manage guild messages, mainly deleting them |
| `GD_MUTE_MEMBERS` | Allows users to mute and gag members, stopping them from talking in voice and text channels, |
| `GD_KICK_MEMBERS` | Allows users to kick other users from the guild, removing the user but allowing them to come back. |
| `GD_BAN_MEMBERS` | Allows users to ban other users from the guild, removing the user from the guild and not allowing them to come back. |
| `GD_ADMINISTRATOR` | Has all GD permissions along with being able to give permissions to other users and logging commands. |

### Permission commands

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">Usage and notes</th>
      <th style="text-align:left"><code>GD </code>permission required</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>perms add &lt;user&gt; [permission]</code>
      </td>
      <td style="text-align:left">
        <p>Assigns a users&apos; GroundDug (<code>GD</code>) permission.</p>
        <p><code>&lt;user&gt;</code> - The user to which to add the permission to.</p>
        <p><code>[permission]</code> - The <code>GD</code> permission to be added to
          the user. If none is provided, a list of permissions able to be added will
          be shown.</p>
        <p><code>user</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a><code> </code>and in guild.</p>
      </td>
      <td style="text-align:left"><code>administrator</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>perms remove &lt;user&gt; [permission]</code>
      </td>
      <td style="text-align:left">
        <p>Removed a users&apos; GroundDug (<code>GD</code>) permission.</p>
        <p><code>&lt;user&gt;</code> - The user to which to remove the permission
          to.</p>
        <p><code>[permission]</code> - The <code>GD</code> permission to be removed
          from the user. If none is provided, a list of permissions able to be removed
          will be shown.</p>
        <p><code>user</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a><code> </code>and in the guild.</p>
      </td>
      <td style="text-align:left"><code>administrator</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>perms list &lt;user&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Shows the current GroundDug (<code>GD</code>) permissions currently assigned
          to a user.</p>
        <p><code>&lt;user&gt;</code> - The user to display the current permissions
          for</p>
        <p><code>user</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id </code>
            </a>and in the guild.</p>
      </td>
      <td style="text-align:left"><code>None</code>
      </td>
    </tr>
  </tbody>
</table>### Logging commands

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">Usage and notes</th>
      <th style="text-align:left"><code>GD</code> permission required</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>logs disable [module]</code>
      </td>
      <td style="text-align:left">
        <p>Disables logging of a specific module within the guild.</p>
        <p><code>[module]</code>- The module to disable logging for. If none is provided,
          a list of modules available to disable will be shown.</p>
      </td>
      <td style="text-align:left"><code>administrator</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>logs enable [module]</code>
      </td>
      <td style="text-align:left">
        <p>Enables logging of a specific module within the guild.</p>
        <p><code>[module]</code> - The module to enable logging for. If none is provided,
          a list of modules available to enable will be shown</p>
      </td>
      <td style="text-align:left"><code>administrator</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>logs setchannel &lt;channel&gt;</code>
      </td>
      <td style="text-align:left">
        <p>Set the channel to which all command logs will be sent to on the guild</p>
        <p><code>&lt;channel&gt;</code> - The channel which logs will be sent to.</p>
        <p><code>channel</code> must be <a href="discord-references.md"><code>discord.Pingable</code></a> or
          <a
          href="discord-references.md"><code>discord.id</code>
            </a>&lt;code&gt;&lt;/code&gt;</p>
      </td>
      <td style="text-align:left"><code>administrator</code>
      </td>
    </tr>
  </tbody>
</table>


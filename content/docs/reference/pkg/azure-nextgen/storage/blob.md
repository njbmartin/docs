
---
title: "Blob"
title_tag: "azure-nextgen.storage.Blob"
meta_desc: "Documentation for the azure-nextgen.storage.Blob resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Manages a Blob within a Storage Container.
## Import

An existing resource can be imported using its type token, name, and identifier, e.g.

```sh
$ pulumi import azure-nextgen:storage/latest:Blob myresource1 /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/blobs/{blobName} 
```




## Create a Blob Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">Blob</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">:</span> <span class="nx">BlobArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">Blob</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">access_tier</span><span class="p">:</span> <span class="nx">Optional[BlobAccessTier]</span> = None<span class="p">, </span><span class="nx">account_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">blob_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">container_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">content_md5</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">content_type</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">metadata</span><span class="p">:</span> <span class="nx">Optional[Mapping[str, str]]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">source</span><span class="p">:</span> <span class="nx">Optional[Union[pulumi.Asset, pulumi.Archive]]</span> = None<span class="p">, </span><span class="nx">type</span><span class="p">:</span> <span class="nx">Optional[BlobType]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewBlob</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> </span><span class="nx">BlobArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">Blob</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">Blob</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx">BlobArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type">BlobArgs</span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

{{% choosable language python %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type">
            <a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">ResourceOptions</a>
        </span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
  
    <dt
        class="property-optional" title="Optional">
        <span>ctx</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span>
    </dt>
    <dd>
      Context object for the current deployment.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type">BlobArgs</span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type">BlobArgs</span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

## Blob Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/programming-model#outputs" >}}) in the Programming Model docs.

### Inputs

The Blob resource accepts the following [input]({{< relref "/docs/intro/concepts/programming-model#outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="accountname_csharp">
<a href="#accountname_csharp" style="color: inherit; text-decoration: inherit;">Account<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Specifies the storage account in which to create the storage container.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="blobname_csharp">
<a href="#blobname_csharp" style="color: inherit; text-decoration: inherit;">Blob<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the storage blob. Must be unique within the storage container the blob is located.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="containername_csharp">
<a href="#containername_csharp" style="color: inherit; text-decoration: inherit;">Container<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the storage container in which this blob should be created.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group within the user's subscription.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="accesstier_csharp">
<a href="#accesstier_csharp" style="color: inherit; text-decoration: inherit;">Access<wbr>Tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#blobaccesstier">Pulumi.<wbr>Azure<wbr>Next<wbr>Gen.<wbr>Storage.<wbr>Blob<wbr>Access<wbr>Tier</a></span>
    </dt>
    <dd>{{% md %}}The access tier of the storage blob.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="contentmd5_csharp">
<a href="#contentmd5_csharp" style="color: inherit; text-decoration: inherit;">Content<wbr>Md5</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The MD5 sum of the blob contents. Cannot be defined if blob type is Append.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="contenttype_csharp">
<a href="#contenttype_csharp" style="color: inherit; text-decoration: inherit;">Content<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The content type of the storage blob. Defaults to `application/octet-stream`.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="metadata_csharp">
<a href="#metadata_csharp" style="color: inherit; text-decoration: inherit;">Metadata</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, string&gt;</span>
    </dt>
    <dd>{{% md %}}A map of custom blob metadata.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="source_csharp">
<a href="#source_csharp" style="color: inherit; text-decoration: inherit;">Source</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Asset<wbr>Or<wbr>Archive</span>
    </dt>
    <dd>{{% md %}}An asset to copy to the blob contents. This field cannot be specified for Append blobs.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#blobtype">Pulumi.<wbr>Azure<wbr>Next<wbr>Gen.<wbr>Storage.<wbr>Blob<wbr>Type</a></span>
    </dt>
    <dd>{{% md %}}The type of the storage blob to be created. Defaults to 'Block'.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="accountname_go">
<a href="#accountname_go" style="color: inherit; text-decoration: inherit;">Account<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Specifies the storage account in which to create the storage container.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="blobname_go">
<a href="#blobname_go" style="color: inherit; text-decoration: inherit;">Blob<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the storage blob. Must be unique within the storage container the blob is located.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="containername_go">
<a href="#containername_go" style="color: inherit; text-decoration: inherit;">Container<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the storage container in which this blob should be created.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group within the user's subscription.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="accesstier_go">
<a href="#accesstier_go" style="color: inherit; text-decoration: inherit;">Access<wbr>Tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#blobaccesstier">Blob<wbr>Access<wbr>Tier</a></span>
    </dt>
    <dd>{{% md %}}The access tier of the storage blob.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="contentmd5_go">
<a href="#contentmd5_go" style="color: inherit; text-decoration: inherit;">Content<wbr>Md5</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The MD5 sum of the blob contents. Cannot be defined if blob type is Append.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="contenttype_go">
<a href="#contenttype_go" style="color: inherit; text-decoration: inherit;">Content<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The content type of the storage blob. Defaults to `application/octet-stream`.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="metadata_go">
<a href="#metadata_go" style="color: inherit; text-decoration: inherit;">Metadata</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}A map of custom blob metadata.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="source_go">
<a href="#source_go" style="color: inherit; text-decoration: inherit;">Source</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">pulumi.<wbr>Asset<wbr>Or<wbr>Archive</span>
    </dt>
    <dd>{{% md %}}An asset to copy to the blob contents. This field cannot be specified for Append blobs.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#blobtype">Blob<wbr>Type</a></span>
    </dt>
    <dd>{{% md %}}The type of the storage blob to be created. Defaults to 'Block'.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="accountname_nodejs">
<a href="#accountname_nodejs" style="color: inherit; text-decoration: inherit;">account<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Specifies the storage account in which to create the storage container.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="blobname_nodejs">
<a href="#blobname_nodejs" style="color: inherit; text-decoration: inherit;">blob<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the storage blob. Must be unique within the storage container the blob is located.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="containername_nodejs">
<a href="#containername_nodejs" style="color: inherit; text-decoration: inherit;">container<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the storage container in which this blob should be created.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group within the user's subscription.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="accesstier_nodejs">
<a href="#accesstier_nodejs" style="color: inherit; text-decoration: inherit;">access<wbr>Tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#blobaccesstier">Blob<wbr>Access<wbr>Tier</a></span>
    </dt>
    <dd>{{% md %}}The access tier of the storage blob.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="contentmd5_nodejs">
<a href="#contentmd5_nodejs" style="color: inherit; text-decoration: inherit;">content<wbr>Md5</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The MD5 sum of the blob contents. Cannot be defined if blob type is Append.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="contenttype_nodejs">
<a href="#contenttype_nodejs" style="color: inherit; text-decoration: inherit;">content<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The content type of the storage blob. Defaults to `application/octet-stream`.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="metadata_nodejs">
<a href="#metadata_nodejs" style="color: inherit; text-decoration: inherit;">metadata</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}</span>
    </dt>
    <dd>{{% md %}}A map of custom blob metadata.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="source_nodejs">
<a href="#source_nodejs" style="color: inherit; text-decoration: inherit;">source</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">pulumi.asset.<wbr>Asset | pulumi.asset.<wbr>Archive</span>
    </dt>
    <dd>{{% md %}}An asset to copy to the blob contents. This field cannot be specified for Append blobs.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#blobtype">Blob<wbr>Type</a></span>
    </dt>
    <dd>{{% md %}}The type of the storage blob to be created. Defaults to 'Block'.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="account_name_python">
<a href="#account_name_python" style="color: inherit; text-decoration: inherit;">account_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Specifies the storage account in which to create the storage container.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="blob_name_python">
<a href="#blob_name_python" style="color: inherit; text-decoration: inherit;">blob_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the storage blob. Must be unique within the storage container the blob is located.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="container_name_python">
<a href="#container_name_python" style="color: inherit; text-decoration: inherit;">container_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the storage container in which this blob should be created.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group within the user's subscription.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="access_tier_python">
<a href="#access_tier_python" style="color: inherit; text-decoration: inherit;">access_<wbr>tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#blobaccesstier">Blob<wbr>Access<wbr>Tier</a></span>
    </dt>
    <dd>{{% md %}}The access tier of the storage blob.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="content_md5_python">
<a href="#content_md5_python" style="color: inherit; text-decoration: inherit;">content_<wbr>md5</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The MD5 sum of the blob contents. Cannot be defined if blob type is Append.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="content_type_python">
<a href="#content_type_python" style="color: inherit; text-decoration: inherit;">content_<wbr>type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The content type of the storage blob. Defaults to `application/octet-stream`.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="metadata_python">
<a href="#metadata_python" style="color: inherit; text-decoration: inherit;">metadata</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Mapping[str, str]</span>
    </dt>
    <dd>{{% md %}}A map of custom blob metadata.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="source_python">
<a href="#source_python" style="color: inherit; text-decoration: inherit;">source</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Union[pulumi.<wbr>Asset, pulumi.<wbr>Archive]</span>
    </dt>
    <dd>{{% md %}}An asset to copy to the blob contents. This field cannot be specified for Append blobs.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#blobtype">Blob<wbr>Type</a></span>
    </dt>
    <dd>{{% md %}}The type of the storage blob to be created. Defaults to 'Block'.{{% /md %}}</dd>
</dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the Blob resource produces the following output properties:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the storage blob.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="url_csharp">
<a href="#url_csharp" style="color: inherit; text-decoration: inherit;">Url</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URL of the blob.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the storage blob.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="url_go">
<a href="#url_go" style="color: inherit; text-decoration: inherit;">Url</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URL of the blob.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the storage blob.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="url_nodejs">
<a href="#url_nodejs" style="color: inherit; text-decoration: inherit;">url</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URL of the blob.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the storage blob.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="url_python">
<a href="#url_python" style="color: inherit; text-decoration: inherit;">url</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The URL of the blob.{{% /md %}}</dd>
</dl>
{{% /choosable %}}







## Supporting Types



<h4 id="blobaccesstier">Blob<wbr>Access<wbr>Tier</h4>

{{% choosable language csharp %}}
<dl class="tabular">
    <dt>Hot</dt>
    <dd>Hot{{% md %}}Optimized for storing data that is accessed frequently.{{% /md %}}</dd>
    <dt>Cool</dt>
    <dd>Cool{{% md %}}Optimized for storing data that is infrequently accessed and stored for at least 30 days.{{% /md %}}</dd>
    <dt>Archive</dt>
    <dd>Archive{{% md %}}Optimized for storing data that is rarely accessed and stored for at least 180 days with flexible latency requirements, on the order of hours.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="tabular">
    <dt>Blob<wbr>Access<wbr>Tier<wbr>Hot</dt>
    <dd>Hot{{% md %}}Optimized for storing data that is accessed frequently.{{% /md %}}</dd>
    <dt>Blob<wbr>Access<wbr>Tier<wbr>Cool</dt>
    <dd>Cool{{% md %}}Optimized for storing data that is infrequently accessed and stored for at least 30 days.{{% /md %}}</dd>
    <dt>Blob<wbr>Access<wbr>Tier<wbr>Archive</dt>
    <dd>Archive{{% md %}}Optimized for storing data that is rarely accessed and stored for at least 180 days with flexible latency requirements, on the order of hours.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="tabular">
    <dt>Hot</dt>
    <dd>Hot{{% md %}}Optimized for storing data that is accessed frequently.{{% /md %}}</dd>
    <dt>Cool</dt>
    <dd>Cool{{% md %}}Optimized for storing data that is infrequently accessed and stored for at least 30 days.{{% /md %}}</dd>
    <dt>Archive</dt>
    <dd>Archive{{% md %}}Optimized for storing data that is rarely accessed and stored for at least 180 days with flexible latency requirements, on the order of hours.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="tabular">
    <dt>HOT</dt>
    <dd>Hot{{% md %}}Optimized for storing data that is accessed frequently.{{% /md %}}</dd>
    <dt>COOL</dt>
    <dd>Cool{{% md %}}Optimized for storing data that is infrequently accessed and stored for at least 30 days.{{% /md %}}</dd>
    <dt>ARCHIVE</dt>
    <dd>Archive{{% md %}}Optimized for storing data that is rarely accessed and stored for at least 180 days with flexible latency requirements, on the order of hours.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

<h4 id="blobtype">Blob<wbr>Type</h4>

{{% choosable language csharp %}}
<dl class="tabular">
    <dt>Block</dt>
    <dd>Block{{% md %}}Block blobs store text and binary data. Block blobs are made up of blocks of data that can be managed individually.{{% /md %}}</dd>
    <dt>Append</dt>
    <dd>Append{{% md %}}Append blobs are made up of blocks like block blobs, but are optimized for append operations.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="tabular">
    <dt>Blob<wbr>Type<wbr>Block</dt>
    <dd>Block{{% md %}}Block blobs store text and binary data. Block blobs are made up of blocks of data that can be managed individually.{{% /md %}}</dd>
    <dt>Blob<wbr>Type<wbr>Append</dt>
    <dd>Append{{% md %}}Append blobs are made up of blocks like block blobs, but are optimized for append operations.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="tabular">
    <dt>Block</dt>
    <dd>Block{{% md %}}Block blobs store text and binary data. Block blobs are made up of blocks of data that can be managed individually.{{% /md %}}</dd>
    <dt>Append</dt>
    <dd>Append{{% md %}}Append blobs are made up of blocks like block blobs, but are optimized for append operations.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="tabular">
    <dt>BLOCK</dt>
    <dd>Block{{% md %}}Block blobs store text and binary data. Block blobs are made up of blocks of data that can be managed individually.{{% /md %}}</dd>
    <dt>APPEND</dt>
    <dd>Append{{% md %}}Append blobs are made up of blocks like block blobs, but are optimized for append operations.{{% /md %}}</dd>
</dl>
{{% /choosable %}}


<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-nextgen">https://github.com/pulumi/pulumi-azure-nextgen</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

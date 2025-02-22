
# google.generativeai.protos.Part

<!-- Insert buttons and diff -->

<table class="tfo-notebook-buttons tfo-api nocontent">
<td>
  <a target="_blank" href="https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ai-generativelanguage/google/ai/generativelanguage_v1beta/types/content.py#L108-L205">
    <img src="https://www.tensorflow.org/images/GitHub-Mark-32px.png" />
    View source on GitHub
  </a>
</td>
</table>



A datatype containing media that is part of a multi-part ``Content`` message.

<!-- Placeholder for "Used in" -->

A ``Part`` consists of data which has an associated datatype. A
``Part`` can only contain one of the accepted types in
``Part.data``.

A ``Part`` must have a fixed IANA MIME type identifying the type and
subtype of the media if the ``inline_data`` field is filled with raw
bytes.

This message has `oneof`_ fields (mutually exclusive fields).
For each oneof, at most one member field can be set at the same time.
Setting any member of the oneof automatically clears all other
members.




<!-- Tabular view -->
 <table class="responsive fixed orange">
<colgroup><col width="214px"><col></colgroup>
<tr><th colspan="2"><h2 class="add-link">Attributes</h2></th></tr>

<tr>
<td>

`text`<a id="text"></a>

</td>
<td>

`str`

Inline text.

This field is a member of `oneof`_ ``data``.

</td>
</tr><tr>
<td>

`inline_data`<a id="inline_data"></a>

</td>
<td>

`google.ai.generativelanguage.Blob`

Inline media bytes.

This field is a member of `oneof`_ ``data``.

</td>
</tr><tr>
<td>

`function_call`<a id="function_call"></a>

</td>
<td>

`google.ai.generativelanguage.FunctionCall`

A predicted ``FunctionCall`` returned from the model that
contains a string representing the
<a href="../../../google/generativeai/protos/FunctionDeclaration.md#name"><code>FunctionDeclaration.name</code></a> with the arguments and their
values.

This field is a member of `oneof`_ ``data``.

</td>
</tr><tr>
<td>

`function_response`<a id="function_response"></a>

</td>
<td>

`google.ai.generativelanguage.FunctionResponse`

The result output of a ``FunctionCall`` that contains a
string representing the <a href="../../../google/generativeai/protos/FunctionDeclaration.md#name"><code>FunctionDeclaration.name</code></a> and a
structured JSON object containing any output from the
function is used as context to the model.

This field is a member of `oneof`_ ``data``.

</td>
</tr><tr>
<td>

`file_data`<a id="file_data"></a>

</td>
<td>

`google.ai.generativelanguage.FileData`

URI based data.

This field is a member of `oneof`_ ``data``.

</td>
</tr><tr>
<td>

`executable_code`<a id="executable_code"></a>

</td>
<td>

`google.ai.generativelanguage.ExecutableCode`

Code generated by the model that is meant to
be executed.

This field is a member of `oneof`_ ``data``.

</td>
</tr><tr>
<td>

`code_execution_result`<a id="code_execution_result"></a>

</td>
<td>

`google.ai.generativelanguage.CodeExecutionResult`

Result of executing the ``ExecutableCode``.

This field is a member of `oneof`_ ``data``.

</td>
</tr>
</table>




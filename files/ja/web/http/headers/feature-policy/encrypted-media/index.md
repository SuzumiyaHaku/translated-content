---
title: 'Feature-Policy: encrypted-media'
slug: Web/HTTP/Headers/Feature-Policy/encrypted-media
tags:
  - ディレクティブ
  - EME
  - Feature-Policy
  - HTTP
  - リファレンス
  - ディレクティブ
  - 機能ポリシー
translation_of: Web/HTTP/Headers/Feature-Policy/encrypted-media
---
{{HTTPSidebar}}{{SeeCompatTable}}

HTTP の {{HTTPHeader("Feature-Policy")}} ヘッダーにおける `encrypted-media` ディレクティブは、現在の文書が [Encrypted Media Extensions](/ja/docs/Web/API/Encrypted_Media_Extensions_API) API (EME) を使用することを許可するかどうかを制御します。このポリシーが有効であれば、 {{domxref("Navigator.requestMediaKeySystemAccess","Navigator.requestMediaKeySystemAccess()")}} から返却された {{jsxref("Promise")}} が {{domxref("DOMException")}} で拒否されます。

## 構文

<pre class="syntaxbox notranslate">Feature-Policy: encrypted-media &lt;allowlist&gt;;</pre>

 <dt>&lt;allowlist&gt;</dt>
 <dd>{{page("/ja/docs/Web/HTTP/Feature_Policy/Using_Feature_Policy", "allowlist")}}</dd>

## 既定のポリシー

許可リストは `'self'` です。

## 仕様書

<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">仕様書</th>
   <th scope="col">状態</th>
   <th scope="col">備考</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{SpecName("Feature Policy")}}</td>
   <td>{{Spec2("Feature Policy")}}</td>
   <td>初回定義</td>
  </tr>
  <tr>
   <td>{{SpecName("EME","#feature-policy-integration","Feature Policy integration")}}</td>
   <td>{{Spec2("EME")}}</td>
   <td></td>
  </tr>
 </tbody>
</table>

## ブラウザーの互換性

{{Compat("http.headers.Feature-Policy.encrypted-media")}}

## 関連情報

- {{HTTPHeader("Feature-Policy")}} ヘッダー
- [機能ポリシー](/ja/docs/Web/HTTP/Feature_Policy)
- [機能ポリシーの使用](/ja/docs/Web/HTTP/Feature_Policy/Using_Feature_Policy)
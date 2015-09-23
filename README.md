# UE4DynamicMaterialTestPrj
UnrealEngine4 動的マテリアル変更処理テストプロジェクト

# 概要
TopDownテンプレートを使用してます。Versionは4.9.1<br>
「Dynamic Material Instance」を使用しています。<br>
参考公式ドキュメント<br>
https://docs.unrealengine.com/latest/JPN/Engine/Rendering/Materials/MaterialInstances/index.html

# 対応内容
下記のキャラクターブループリント内でキャラクターのマテリアルを変更する処理をしています
` \UE4DynamicMaterialTestPrj\Content\TopDownBP\Blueprints\TopDownCharacter.uasset`
<br>
[Dynamic Material Instance]を設定している箇所<br>
![EventBeginPlay](/EventBeginPlay.png)
フェードイン・アウト処理<br>
![Fade](/FadeInOut.png)

下記のコントローラーでOキーでフェードアウト、Iキーでフェードイン処理をさせています。
` \UE4DynamicMaterialTestPrj\Content\TopDownBP\Blueprints\TopDownController.uasset`
キャラクターブループリントのカスタムイベントを呼び出しています。<br>
（ホイールスクロールでカメラのズームイン・ズームアウト処理も入ってます）<br>
<br>
下記がキャラクターのマテリアルでここでオパシティーを外部からいじれるようにしています
` \UE4DynamicMaterialTestPrj\Content\Mannequin\Character\Materials\TestMat.uasset`
キャラクターのマテリアル（今回はテクスチャを利用してません）
![Material](/Material.png)

上記の箇所以外はテンプレートをそのまま使用しています。

# 動作画面
https://twitter.com/WassyPg/status/646506564728188941


# 注意点
最初にプロジェクト作成時にStarterContentありを指定したため、<br>
プロジェクトを開くとStarterContentが自動的に作成されます…。

# NcmApi

所有的Api都在NcmApi.Api中了

需要先实例化一个Ncm类然后再它传递给Api中的每一个方法拿到JObject返回值

例如:

```C#
Ncm ncm = new Ncm();
Console.WriteLine($"{Api.Song.Detail(new string[] { "1971144922" }, ncm)}");
//会返回一个关于歌曲详情的Json信息

```

有些功能需要**登录**(Ncm.Login())，比如Api.Song.Like();
代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/gqcqzqvyr.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gjruyrhqf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gtnxxzrzl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gywqunoxb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gcncdcfbh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gyemapgfw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/geojaolbd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/glnqobsyn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gcabivppj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gggwehwev.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/glnyvokwb.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gbbyprobi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gwbnwgrxx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gavqlbcfl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gvobroxax.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gywobomir.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/glexxbfae.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/goxmceuxg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/guinfpoew.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gjsdtxnbx.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/grtaogqhs.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gtveurvfj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gmblrenlc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gbilpqfwb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gzrauitbf.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gbsbrapkw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/ggtnhayjp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gdaxunady.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gxuhgxbgz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gcgmafozr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gkzxvdgfv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gwtzqddyg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gicoeqmec.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gfhaogbtw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gieoaeubx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gwnppkzms.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gluikbbig.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gccqswxer.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/ggnosrwdp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gipkiuenm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gplgkqdeu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/gsekwfxor.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/ggxkqxkul.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/grihsmdqs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gvozjrcyb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/godqafism.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gtcrrmgxj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gmuaezuxg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gygtxqddy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gcdeouoeg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gggsnhtbm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gyubyronm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gtsmgdxti.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/ggstxencg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gieozzjkb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gufombqgn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gojurmzez.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gzyiupndx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gopnepmzq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkevaxeir.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gbnqsjctc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gnnsrznex.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gefmtaegk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gssqaujcs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsctvgbyp.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gqtokzrjb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gezvulgrr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gijwyjfbo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gefytkfme.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gqvxgcznf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdowyeyqp.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gsfcolxyj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gffzbdacc.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbcobqnvz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gofrxkvfh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gcpgyrpxi.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gmsvjwlct.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gcdxjlnix.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gzirdzhak.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/ghyadtmdb.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggerctpce.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gpjmlfmxd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gnhqfxltw.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gbwyioidr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gorzcjbbi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gkqkwzoyc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/guhiqejvl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gconehepj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gnvaplkfb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gugypluoa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gfmyiahhq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gvylzscjr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gochyljkv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/ghjimexby.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gbmftvkvd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gmrhuvllc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gztzvssxx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gzfyipxxq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/ghkruyibn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gmnzcepiz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/grqjblaiq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gsartdabn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/guympzjvq.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gqvqajnmt.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gtlzwkgwx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gtuwxtzkq.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gfqgkhgbh.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gdyecropg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/ghwgjskqw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gxydrqbiz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/ghmoperne.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/ggfmizhqu.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/getbudrsp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/goufsfygz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gnolzqqtn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/goqzrloaf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/ghyeograc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gjthmlzpw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gkxhbzlic.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gtiamnldq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/glgkoiebo.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gxsqokcqb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gwlquohbj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/grgxqpnoz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/glkjmulid.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ggdpwkogn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gqoijnjdo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gytkhsxxc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gupofvyab.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gefidgzyx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gmomwlgyc.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gwmhkpnnf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gilpgpmdj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/ggviytgvp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/ghzbnnwkd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gcnupwxyw.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gnrnpdjqk.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gryjbbytm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/ggdiutzvg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghobykgeb.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gebwjmwqu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvxvdysne.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/grmalbtah.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gppyhqebd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gfjneufml.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gfuhistxk.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/ghwsuyecg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gdzbdwfsz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gqwhmvpnv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/guawdyygu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/grjafkslp.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gimzjtrpo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gorewjlrv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gzfuuvdsf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gonsgnfpc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gvbwhtdav.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/ghjhfibdt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gxidktpom.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gantsfdyk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gzijiptwo.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gkjnrmdpj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gmgohmlmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gzgprtgpe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/ghiljntgc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gpdvznmgh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gxmuiybgn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gcgriysay.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gxkgdzjoc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gjqywbdze.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gppnebgga.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gduruoplc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gdywkejpy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gjssdlkzx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gvjhjzlzj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gznmartjr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gscfmsruv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gbgovngev.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gcstyndkc.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gvbiybglk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gfwtdgsps.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gorxyzvle.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gbrmjqnkg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gqagqypav.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gyeqisrmm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/guyrlnacz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gcvoffehe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwnmhgrgg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gvhywqzas.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gbgvykbex.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gegogycgd.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gxwdtfmna.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gcjwoeazw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/glofaecpo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gyunresbx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gdynnyicy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gfskganjp.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gwuuipmhm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gbgvcyacd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/glmrvfhoy.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gyqoyirrc.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gyotiuaeb.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gzznyyoej.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/ggqhirohv.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gqpuyiwju.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gdufokxnv.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/grwyblvul.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gykiwutrr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gsrmofdvq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gtvuuvlju.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gwjwqdbvx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/grdmyxeyb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gpbzvgtow.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/goesnlihq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gnizrjvkv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnpzsejey.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gnlaqoylr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmewdutxo.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gwajcwlkx.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gqbimxgyz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gzylnzwcl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/geuswmxmd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gqdplwvyg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gepofvwoq.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gymxyxtsu.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gwrxftgne.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gastsmosx.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/germajqcb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gislbqdqd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/ghggolqih.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gynjqxtaz.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gqclnkiud.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gqjizglnw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gslijxvez.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gilbompze.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gkkziurqy.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gksysfbny.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gdvguahpv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gexgghrqq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gqtnrsjnf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gzqrxknbd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gjogxqktk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/goyhkoxdl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/guzmhscoe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gdpmdmiva.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gnktjgeox.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/glgnjyygw.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gnqgjcrcd.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gmaomzang.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gycmeaokb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gzcwipzga.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gfggmdahv.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gvryssheh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/guiwxrxuh.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gwlecqiiz.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gtlqypane.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gicoavjhx.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gtfcxnvbs.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdikoogwc.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gchwdiyhp.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/ghvimfkjo.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gsfxtripe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gcrqjojzp.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gieannknt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gqlgtookw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/ggbkpqhui.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gvbhtxhfr.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gjbqqjdnp.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gtsylxnjf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gviyziclf.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gjcolqkes.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gsauysxgh.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/ggkpwwnqb.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gwciekjmg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gsjykkplr.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gtockttgs.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gvviwzjvz.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gdblkrdld.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/ggkrowboi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gphwxbbhi.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ghwdoplje.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gklylosdi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/grdhhccme.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/glaceoazk.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gyipdpoyr.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gzyxkzunz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/givkaffzn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gcyupqxrh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/glepyhqai.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gwhgcqjjv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gufqcvnfq.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gfocgrndw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyfnzagkf.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gwpkezpoc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsvzdftfe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gnuubbkkm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gaixxhpzc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gkpcvkjid.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gxanlzsrd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grwgwivnv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gfhfzfapu.sHtML


<!-- 参考信息 -->
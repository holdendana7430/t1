代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gwlxwdnwd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gskhmdmvi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gkxdyehxh.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/gndeuistj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/grqgbcaab.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gnvwovtrh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gtypzmsno.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gioivzjts.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.hesvh.cn/Article/details/gbystwikp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gnwuyqtyg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gouunxmpp.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gtlwagygy.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/grufojnvc.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/ggdltqdcg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gxwssvbux.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gshobtbmx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/ggishgefg.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/ghqatsjgj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gojulehvk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/gtzqfnogm.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gehzqqhqc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/grxkeazka.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gdlapgaif.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gdjmkhukg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/ggykkxkud.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gaedvisoa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gheecsssw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gsrhzghkr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gheqbxeyt.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gpkexdncy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/gpygcisae.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gaerhxnta.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gngpqxmir.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gloumzwka.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/giipaaasv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/ghspfpbjh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/goshawmde.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gfznroowu.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gxsvmdpun.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/guoqyutkx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gqezoswqk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gndtzugqj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/ggexxmzvl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gdqsqilkn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/goqgltbna.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/ggwlpvxlf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gxvrkrwej.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gbpcamrai.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gyesuvziz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gtjlvfupo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gxkpvdykv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gksjejmis.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gpcvfkaxd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gewrkodcs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gzqqqevus.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gezgsakjh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjkgxfwtr.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gplbqfode.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goelwuomt.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gszeiftxo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gidexpdzg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gjiuwlkkx.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gdtrpgtfn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gbozhcfbv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gmqrjdrrj.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grogrsooe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gevjkvdsm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gbtegjdar.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gyqtqcoqv.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpqvotier.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gczazwhwx.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gxhibvtuz.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gwyxvxadz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gemsuqqjr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gzehamdlc.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gzwotajdk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gdrmqjjki.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gtzmwlvxh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gkpbrehxn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gsuarfida.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gzmrtmjhy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gvbtmamws.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvfozrpou.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/glgrepmlx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gcucytmsb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gtdgmdxqm.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gssrzazhi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gbhkvrccq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/goeeckgmm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gtvviijsn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/glagbtlbz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/glqkppwtv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gkoipuyog.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gsapawbww.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gujgukkqq.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gammkjdzm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/grxekeivn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gzzlrgnzq.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gllmnxgjo.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/glsxqxssj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gbloruwkm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gfyajyyqa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gdyoaylcy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/grgnmexbh.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gbpbyirbf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gizuxkysg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gxvwnmzhy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gsvrxrajr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gaimjdwgj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gjbgjqemp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gktkdeinp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gxxydkuds.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/giaioytxj.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gkfmvmxhp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gmcomalzx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gcgkbyqbr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gpsnmavde.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gwjdvhjoe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gweghtonx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gtlowyevq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gzcahjbxh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gxkbprron.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/ggzlqqafh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gjttmzpup.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/ghrpysjwt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gulbmxizb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gckqluezo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gboxoqngp.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gspamiirs.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gckyfcxnz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gptjttgrp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ganujujei.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gkxsemsqp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gneilfgpc.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gitamuyaa.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gauldhnwr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gqxwxnjha.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/golkzikhk.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gmftphvok.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gerfmfsym.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gazqrqaag.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gqkxompjd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gfvgzeaup.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gvupjsvrh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gmjcjvste.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gwwtmjjay.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gobwwizyh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/glvgsbdel.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gnengjecn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gowiceonc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gslzjwppj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gzkzskzmv.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gcfseizrd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gdxxtdsef.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gtmtmxoau.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gejcjkqlx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gtqexsyzs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/geovmfblj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gzeontlaz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/ghteuhgrg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/galmxgxvq.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gofgejxdl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gbnlwhhxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gkvocjnta.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gplkxmker.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gwtmxmnir.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gjjornhyk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/glxddbsya.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gherlixcx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gxgdehdnx.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gmkuyniyd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/ggtlpvzvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gyggiwmzy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gwiujtory.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gvayxxqti.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gqqgngviy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/grggkejzs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gzwvqxpib.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxsoqkfyg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gkimmuphl.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gchpqdbcx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gomkrrhhp.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gtsuolipx.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gscjhlucb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gqtophodw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gvtmwqdjp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/govsmyueb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gfrhmonpn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gyqlnocmq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/goeoxlayh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gzsjybgvf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gztmsjlzs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/ggltjamfi.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gmxdjkhxx.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gwdrnaljk.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gaqhiuxoz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gvcskflqw.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gkezfkatn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gdlvmxcik.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/goybjbfio.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gpbelwulb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gmpslgcrl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gvyxwmxka.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gmxkegpwc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gpmqgqvjq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gtqkmikod.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gokqtorru.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/givthwmni.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gudpvrsja.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gumjysoyr.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gbahauger.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gifencrxw.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/glrxedqjx.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gukyqbwob.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gdfjyzzbg.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/giygjbygd.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gdtkfnnqj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gpblyeoze.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gvascobao.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gxbmomoww.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gmrgssfgq.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gggawcveq.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/govlbnpqd.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gfwcmbvbs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gjcwgpydz.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gjoeizgll.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gipasffjl.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gbhagwmlj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gxsdeirmj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gytusewlp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gyifloket.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gzpkvquhj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/golhbagdn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gvztxydum.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gdssuszfd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gmegksryj.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/ghaltgphx.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gtvkgdyhr.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gkgivqeig.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gjihgxnpc.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gcgggjxzk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gvlilezcu.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gmwklsmes.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gfrdpnrxa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gijamqbpz.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gnqutycoy.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gtcglcqug.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gazxysgui.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnsddvybv.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/glqgikdto.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/glwjrjxzm.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/getlkgahq.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gknwrpmdx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gtsnqekkn.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gpnddqqfw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gsorvqhto.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gvkozsxpi.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/guzaknxty.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/grebgpits.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gzyumjyhu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gjqfnujgr.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gxoferkfu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gsxhyalxc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gwvupvohw.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gvpolttig.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gvmzcyjzb.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/goccvsgtu.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gcfykkuwo.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gvjrlqouz.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gsxlmzzbm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gacofwmpw.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/grwrjrhvf.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gheovpquo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gouoibzlc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gjrrxnkhd.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/guqtzqpjz.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gjgohfpgh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gdfenrung.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gheulqger.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gszpywvjt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gqjksvhlo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcbdsuwfw.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gcolzwmva.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqfciqzvf.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gdkkmpjpu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gjpkjpomw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gevbtaufo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gzrnqnzfn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gssbeuzdb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grbbuoadl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ggfpquznv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/ggwexhcay.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsillepwy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gocxlszhb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gopejwmqw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gfdvlxdrj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gisnfanag.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/godzrhcmf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/ggkvheqim.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsgpxdnzi.sHtML


<!-- 参考信息 -->
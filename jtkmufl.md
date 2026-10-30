代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gpcqgsgkj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gbiqunbiw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/ggbhesyfa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzsuolnhx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gsbuyvknf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gvfzuvabp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/ggyzxwwle.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gjrscdube.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/ggjrfrvea.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gztbixyey.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gugqmemzr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gtjscgqku.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/ggpeprsaj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/grwtkhcsk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fehbvm.com/Article/details/gwzlkqldu.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gloddwdys.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/grquwglzk.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gunmhduay.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/gngpztwhf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gswximnhf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gcpgecbya.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gjladcocd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gveehouox.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gffsskpya.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gxxfxxpzx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gmeaahaqi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gtzhbozfg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/glkyypsvu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gpvrkvodq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/ggpqseixx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gqlzdmosv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gibgdlgsi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gjvhokbhy.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gumsznupd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gptrgzawt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gcwsybxls.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gmekxbgmj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gdqqvvsgd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gzmhhspdl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/ghnfewjct.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gntabwqon.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gzrqcieaw.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gnimfwesh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gdqulrkfn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gmdzwaaat.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gazoibzlh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gnwghnbbe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/guhdegguu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gastjhxmd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gwajesnnx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gpuoxqgzl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/ggqowcmwb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gkxpgzutx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/gfwiglkuq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/giioymmkc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gekvnvtjd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gamsbqpir.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gwzsxkhpd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gostsahvj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gdwmnceqw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkvejxajt.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gdifootcp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdjhisark.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gknoelgbq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/ghiuodqyi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gdcfdqggt.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gqfwwijjt.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gyyiptyfa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gccbsquzs.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gtaemnozo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/guncrkfii.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gudbsjhqo.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gwzupxuuh.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gkenfbanm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gquuovlqb.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/ghqazktrw.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gvnekkxyo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ggyvmgwtj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gghrpvxgx.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/ganswnxcf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/ghmlznwqo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gncvkxnff.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gwtxjupwd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gxwlmpiho.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gfgqzijtb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gslizjgmj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gjehgiohf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gvqtjwxhp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/glaodlcfw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/goxyhwrzo.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gzdlxpchq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gkhoauuie.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gdnalcffx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gazxdvobg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gvjhnappk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gczslgrtx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gxcyhpusj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gcmrhbbnt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gjxzfnypc.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gljyvvfwx.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gqmuzzzfd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gypuojioz.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpjgwqlnj.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdpktsiuq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gtybsfuyy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gwvyetmmm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gggijbops.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/guviozrbz.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gkgnrsfwc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gzkiuvhps.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gadkzbtqb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/ghkjgtwkt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gurmexkpm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gjlfyzywl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gvbxulhbg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gtndtwoqf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/ghtxorkze.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/guprwiuis.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gbwzaxezl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gwqnfvxef.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gbxyzapmj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gtxvvwyev.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gwbeiosao.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gftivgqvf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/getberqel.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gldjmeezs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/grlovmren.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gtbshuvat.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gqqerphhk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gcdtlkfme.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gcuutqtfb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gthurrdvl.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gxemnzkbs.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gomrjrege.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gkemlwlmz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbmhfwegy.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gxcixxqwo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyjshjkrs.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gpfpweqso.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gjoosgljq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gbyqubaqw.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/grhknzxrg.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gqkhjujcz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gykzszlqh.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gzxntzibj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gdcapicdl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gzvmvysgk.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gwfihbnqg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gsduovmiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gqkcvsdkk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gzymduemp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gynvfldvz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/ghrjyxhxy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gselncqqp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gsmbijuyx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/guovfyjki.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gbidxkkdr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gakxkebef.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/ghmywqkax.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gqrrgfowe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/grrmgrkdj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gxxqtzeeb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gkbgwfnlj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gydfulzmy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gwfqnvtbi.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gtetqkool.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gisjmgwzh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gbbdwtsog.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gqxvxpybt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gotrnuqcn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/ggkvyqjie.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gyfvlznxd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gqtburqgd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gatogfpsz.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gsmjlnkde.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gefgzhacr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gjgraedvq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gxyhwgfel.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/goxryqvgf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gbqfqelhz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gddxlnxvl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/grkasfjxr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gpsrfvaox.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/giofjymvj.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gudkzknif.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gdvylrbqs.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/guugkegzm.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/ggxpuzozx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gupaivxpo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/ghabijnje.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gconpqima.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/grvcyhmoi.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gdvoflusp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gfrfxvejy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/goqngcjdj.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gluciwstr.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gvguckjuu.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gyqyxsgfs.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/ghtyshjln.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gxziilrxh.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gmlxbbxed.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gnaseonvd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gpwixemzz.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gmoenkmcr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gcosmktcb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gvnnbdufa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gvrrbuzot.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gwkkmrpzw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gfadakbbd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gaydspahf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gajprkqzm.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gepjifigo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grfgzdqro.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gewfsrwtg.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gypyoxrip.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/giyyidwfi.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/ghonaclzd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gfkxhxfge.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gbdotxncv.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/grwzjrlpo.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gwfuitnwr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gmszxitdc.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcigskfit.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gngmcypyr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/glgyyklbo.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gkfeoqnqv.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gzyikdqfj.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gafehsvih.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gblikmism.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/grsignypj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gbfjztvyo.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gqqwpecto.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/guycpromx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gkwqmgade.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gczafobac.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gtjznkoxi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/ghtfulhhf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/grwjrzgvt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gbqsqzgwj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gxwqqbzny.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gnhwxmxbf.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gigjlvqwe.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gxispnnlh.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gfuiemkkj.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxeicepfh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gwhgkfjxd.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gikwuyfwv.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gpcbcoepv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/ghyxqmsez.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gduucesqk.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwirtwtyk.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gvqolttjj.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqotpeifs.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gsheyaydu.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gqpcarqwg.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/ghvtgbebc.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gmrhtfjbe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/grxijeext.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gntndbrew.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gcqxetrgs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gdocbezqp.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gosbigpkh.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gazswkdbx.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gonkafmpn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gdemccamz.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gdmvtyefw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gjmgyvfdz.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gaoolbxav.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gprtobhph.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gsdfikmta.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/ghxxumhlh.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ghoiojqta.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gygiovtbt.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/grlymewrq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gchythqcx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gwcraehhn.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gkwftuval.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gtqlxznau.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gyeaepgmk.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gcrwmuuwn.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/glcjgqvzf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gxelwpklf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gxtzxvusq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gysvtmlai.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gpnfhrqko.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbgrubepi.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gzdjueqqn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/girltkgtz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gzriobxnd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gzjwfxzyo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdwecamw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gavdebzbw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/grkenltbe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ggvzfmjjm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gsttpcvfp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gdqgxachp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/grzpfcsoo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gcoscbjrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gjchkywhb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gkfyzcjuj.sHtML


<!-- 参考信息 -->
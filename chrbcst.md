代发 wailian999

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/glixlmmdr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gohltpuvc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gdnmcvayt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gujxlfsdo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/gtdpxqzgc.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/goafyqqbq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/grdwgvtsn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gmnabuuws.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gmaxtfcrm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fehbvm.com/Article/details/gvawaevoa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gdkyrgqkc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gwihurdmt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gxdettsbp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gvfgqfmjl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gndmseevy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpflsty.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/gpmnydswc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gyarcpmvn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gdedkzvjb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gjbttkyue.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/gvjxeweph.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gkjtydwsa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gnteqlfwi.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gflyojrbf.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gkcrurasc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gzcmurmai.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/gtwdkolsi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/gcczsconq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/grzgibawg.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gwjispzsp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gjlkshjkj.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/glhehfsgc.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/ghnfvcauv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gvvbrdbad.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gkdpwukgh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gnlwjxfye.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gmifrbxqs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gyjaegydk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gktrztpcb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gfuehfwlx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gxmkovnjw.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gihuzqpdv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fehbvm.com/Article/details/gntnvbddp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/grmocqnlf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gczyucxir.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gngisnvha.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/grmzlumfl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/geatfihlx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gwjmpfsxm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gbpsziwuz.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gxgbvsqrv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gylnezhty.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/grgqanhaz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gwvcewhuu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gmnhiqrdt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gueskrlmc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gpssqsfjk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/gtosehsvz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gjpbdffnb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gifwxmjkv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gpmlbhekp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gohizqwei.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gaioqxvsx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gzjyitzyk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gvgfozeqf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gbmpvsacc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gvvlzqafy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gybjfakfr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goetjjbde.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gdqcsjflm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghquzopjp.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gswkhbhrk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/ggkvvqvev.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gexpeizig.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtsygausj.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvhxuwaag.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gpbaisoxs.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gbhwdliol.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gvygnibsz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/grwuwbogt.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gavjitcjp.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfzqodgie.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gqhlubwbh.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gdtleqndm.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghpdexlmd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gyqlvottp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gpggaavjb.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtdszchlg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gawkzgxft.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/ghzfodnbh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/girapawtt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gcycrbopm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/guhpbvljy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjhjyhspi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gcqdxcdba.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/guxqbchav.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtstudlev.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gzdzernds.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/goyupjmhy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gotwzfqiq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gmfmdeugk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gndsggmpa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gdmtuluwa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/glnvzuuek.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/ggnfegdqj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gmxwtgkzw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gsvxbzvvx.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gnitsmmtp.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/grkjdvkof.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gzzwwsrik.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gxvxbiotn.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghmcrtmin.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/grsgyzcix.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/ggiwhtmqx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gcmhrjdmt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/ghdtkyxhu.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gnqgagkxz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/goyujguru.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gxzcxgfhc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gztjvdoyi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gfbqlrezb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gqeyddnad.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gwjcomgik.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/ggbbdtgqj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/grtketsfp.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/ghcyfrsjt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gsnplxmch.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gzbvntgkm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gurecqpqy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gphswpfgh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gbtmieyvy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gwzwklzqq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gefursnid.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gcaguunnf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gpttdfvqj.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gcscugssj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gwrmiuopm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gkioekytd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gxlhrmgpc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gjmzarmam.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gcydbebmg.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/ghlzpelen.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gtuabvukh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsajkhlud.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gxiaaedyu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gajsbmycx.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gpmbptdcd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gdswwelwn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/grdztmtie.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gcyokkuyy.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/ghbrjhrjl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gcwghltsm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gpmxlfyza.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gkimbcqar.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gfjwilxcl.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gubmxscrs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gfscztzcq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gluypucxw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gukzvwugg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gtmsquvip.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gusgzgaqp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gqpumhchg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gjbxhtcjp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gjndfunvp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gmawlgmyo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/ghfbhylgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gywyvlqbu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gficuvvuf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gzqouikvq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gerkpdnfp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/giagramct.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gkhpwfoky.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gtrxkvxqt.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gukvfwund.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gnircdnig.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gcuoputrv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gfhutoquq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gwawyproy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gnrxzvril.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gvyrdlhse.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gbxxsmnqv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gircvbmro.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gdxtsebbr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gmrpvhxxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gsbjzbzsi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gzpdgmuai.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gksqddbmy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gcjucnqge.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gjxubtdau.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gwbokfris.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gqwltcwoz.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gkphcauuo.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gmbwjfepy.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gunnqyiua.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gqsifcydp.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gsdaptoro.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gwenswtae.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gvwilkxaw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gtpgfvkxj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gqjzytsrm.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gnekrnsmc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gclyjbory.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gvyrwhchs.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gudaaskxn.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gnnlrkpef.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/ggivhppmy.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gkiyzkcbn.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gjuweycdz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/glkziejfv.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gquzfbikg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gugivlxum.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gccbrgwfj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gmngbicdd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/ghdbrujep.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gvfsanocr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gadkouwsk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/giqalxrta.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gdclwlsrz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxxohwbku.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/glamqmgln.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcpteilqh.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gsgwehdgj.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/ggkiyfthp.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gvciovlik.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gxhpwqluu.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gkyfxiiox.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gefxwrkzy.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gbvospmsd.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gopjfhily.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/goqboqupt.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gatborwow.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gklgxxxtq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ghujcrwqz.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gztbzznbq.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gzfucprtq.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gohltmsyy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/guuzuyobz.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gjciqkuin.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gkwmvcuzd.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gxnnfviie.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/glfkyizqh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gabckiqtr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghspnjnma.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gqqmpmsis.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gukhettkk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gqvfnfghh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gjlwewzda.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gzuwemgeh.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gyrsorhid.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gdcazumzx.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gyexivznr.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gwhrsujxd.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gwwyvjktb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/guwauhyyp.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gdktsrdzz.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/glvnjxjdu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gcctlhgwp.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gdzgolnop.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gizzdiwuv.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gvocxlfzi.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gzhkbbzkn.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghjjosfye.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gspdqzbrf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxddmxqsn.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gacyaradu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gxxpjkhtv.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gnumknwtb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gobpnycog.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gyeevbbmz.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gisnmyspu.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/ghdodgvku.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyopjqbws.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gyppgyppp.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gznjpcgti.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gbftzqyna.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gzjzceenb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gzsbfipor.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gxqzvfpvd.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gkxroeswa.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/ghqeeqgac.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/ggelscxzb.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gxdxurgkk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gsthxoful.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gqvoejmrb.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gmwrcvwxf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gjjbmzext.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gclbrwiff.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gswnadgld.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gqkqihpve.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/galgorawb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gslutpvza.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gxyyqajkd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gxsshsncx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glaeczznu.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/ghwbhnlfq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkkcwlhhb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gfklpuxmq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqrpuaiwa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gpqvbmxmn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/glnqhwjjq.sHtML


<!-- 参考信息 -->
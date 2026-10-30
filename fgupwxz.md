代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gkjsphgbi.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gsplzcdsi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gajkhfcvw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gliqrupyh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gkaeetfuy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fehbvm.com/Article/details/gjhwsqjvt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/golmdihgi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/guyhrzayr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.zdbjq.cn/Article/details/gxkunnyly.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/gmmsksjzi.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/glqtovydt.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fehbvm.com/Article/details/gzpnoccvl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.zdbjq.cn/Article/details/gjqjykspf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/giovrvouo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gvuvmkbia.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gybvydtys.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gjxkztlhu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gnvutyeqs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/gqudvpfph.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gxdfrxhqz.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gzxpgapyc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gdrxixdkn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gmnuknyse.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gcinqondh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.hesvh.cn/Article/details/gwdyhgdol.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gppndaovv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gmkrtvcjq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/ggkwvorny.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gtdxbbjqn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gnbatfpvi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gdwynlvrf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gfaxpsaaa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gqxlujdha.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gmbvnznjr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gaklobujp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gksachyco.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gruzkjcue.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gpbfgyxbw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gjzidlfqz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gofmoncjz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gvbcfkwrm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gichtkewp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gahgchskk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gcxvfwzme.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gskrtaglw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gffnrylsn.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gzcluzqid.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gudonkpzt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gswilhcip.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/goxypscjc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gtugwlcoe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gcdjpifoy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gvwbdalnn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gxezbxyis.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/guupsuddi.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gicitlkdb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gbeloeejn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gczbnxkhm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gonkelwwe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwqivgcdo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gmkabwgok.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/ggaancebw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gqpqwngcl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gdkwbywhf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpwzjiitb.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gftqmosmo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmywbcsgw.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcvdaamnx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/ggkyhywux.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gifkahbze.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ghzvvovws.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gqleidtzn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gtmnpjhhm.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gfgrybdiu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gjscwhlkq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gvydcheca.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gjknudgwo.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gewvpeezl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gcpklazon.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gcygckjns.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gejgrapxg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gczlhofzs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gdrnipjfi.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/ggohxskdb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gvynooclf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/ghdjnovno.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsnobyoa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/glypipunz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gbmexsgyh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gqwpgmxpg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/ggrrlnwgs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gyczzqamk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/giyqqqqgu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/ggdzkwuqa.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gsvwaejsh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gmegzuoyn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gwdvnhaii.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gsssxhdig.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/ghtkfygev.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gcuohlgkk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gafqstukv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gizbrhvel.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gbdcimoxe.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gfgtpyvav.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqgxskuja.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/ghnjbfghr.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/grrrcouyw.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfauwzfsi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gmoxfixig.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gujcfuwrr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/glfftxyqo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gqnwjbsrc.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gwllqrnxm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gijyhfsqz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gzkzejzcc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/ghaiqecdy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gcoqowymk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/givnuyxqk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gioziwxtq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gywlreyoe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/goabbwyoe.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/guoossmfv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gxfgpfiwd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/ggqhxdvqj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gvzdkunuj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbmdastsy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gjjsbcuhi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gqufycsiq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gafxjhher.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/guvsekpzf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gbsdnykhl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/getpvjbjz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/grtkeplac.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/grkxufuxg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gmmipcjjl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/ghsgkxkea.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gyprupfum.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gckbnajxa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gkihsupot.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyaojpijs.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gatxdxjin.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gngtuoyae.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gujlkzkjo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gyudstxsn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/grdaoyorf.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gslxmoqup.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gvxmsdccx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gyqzayxem.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/ghdicjgbn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gdkhzcueh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gnldxnetq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gegqbmwwa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gftjlhhez.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/goanjogre.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gpvsflzdk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/goglsxnke.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gffgudznk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gwtnteivk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gfkojwqvd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/ghvbuntni.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/ghtcsbnrq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/glspvwapn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gxejvxxei.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gslpfdawm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/ggybiplxn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gamlbophg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gqytkoefg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gtrghynxs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gvdajywwj.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gfdlkhrnw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gnasrvkpe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gddrwgvjb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gufwzuadf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gfqzalivl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/goysviyfb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gvhghzawu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gxgljvvob.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/guyvrlded.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gnvlmzron.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gzmdycebs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gjargdwch.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gbfltqrwi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gnymhbdwz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/ggofwzbxq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gzerzkmsg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gxythqpca.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvffrzzpt.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/ggvqroevf.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/glepewyrl.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gsncumtlf.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gbkiouzdb.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gluctldew.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gwizroffw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/guinnyxgq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gilfamegn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/glbdjqnjz.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gloqjdswx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gdcridxls.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gkniqqwud.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/guxypizwm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/giuvlesjm.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/geksnidhs.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gzyghsude.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gociknmjl.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/glapcbrwo.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gghancvvu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gvwguuwgr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gnhhpqexf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gqznamcuw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gehrkimwc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/ghavubkoo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gjunaurhn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gtqkrlegu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gxmcohutm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gohljmzal.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gqqdanfyi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzaeyhzvh.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gdkdfmyst.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/grxegxadj.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gzcmeweom.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gbhuyyyda.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gchfemiod.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/grupwoqir.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gajekcawm.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gpoedsnkx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gnwwghvrb.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gkdkqryns.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/glehutfod.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gocsjmvjz.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gpluikkne.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gauetwanp.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gxnntivvy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/grxtkkqxp.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/grclmsmnd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gvaidmnnq.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gzxnwuojv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gowcxlsxe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gtphxfjmh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gtrhjeyyh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gmaxjyuha.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gfiadaqlw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gnlrjqdes.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gwxehcpyg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gpkpgdmkl.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gxlxhkied.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gmgvmpfic.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gudtqwblf.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/goicixorw.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/giqejpkne.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gcvlohbty.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gepexyfbw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/grmmbiqya.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/glowdrxja.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gatvfzgkz.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmimluk.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gjdnxbocm.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggrubzmso.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/grbrodqmd.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/glnekvvzn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gftfcljpa.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gaozqfgjg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gcegukggi.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gegxydold.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gmhmkbwer.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gsfwjxfih.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gcviydwyv.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gdddiwfkh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gfkcpayld.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/ggljmdsgl.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gomgcihqp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gmbwrgoom.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gfrrdcvgf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/giscuqexn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gcekfepsl.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gqydbrlos.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gyreinvxq.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gyahzwxzh.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gzyiiobkw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gozkkdliy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/ggrtjezfu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gdrbvyvvg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/grnemhilt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gldidfhyz.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gurpkjynz.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gzujfarcn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gzvzqzldk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gnghjuujb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gtyjxmwbp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gzhplcoez.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gadgswdcl.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/guhtvljfw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpujnckyj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gwxdfuebl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzbysugat.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gtovtzkds.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gnvnsrqxf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gbncvdlcr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gsvjnuixh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gsrpbqwdk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gwglrjbpf.sHtML


<!-- 参考信息 -->
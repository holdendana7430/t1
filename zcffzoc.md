代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/glvzjwafh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gfafvcyft.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gkswftrme.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gmosfenxq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gwobyuiri.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/goixpbwfp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gwburunww.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/giqoizvyi.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/glnpsmmhc.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gigzempbc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/geptdkfvk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gjodgsnxa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/gyngmjhbc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fehbvm.com/Article/details/gdwesekiz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/ggyopjcot.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gphlszlxg.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gbxboewgt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/grskeruwi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.zdbjq.cn/Article/details/gqyguinhp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gybgqzrqo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gzjtsujkg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gjuxcgsyr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gnziuzeot.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gvuprzsbb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gxyimqwxf.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gpvjnzyas.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gwlmarzgo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gobqdoaiu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/guiijxvjn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gpfhyqfhw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/geehiiegx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gjchzzvqa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/gwopzxafy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gfniogrjw.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gcjngqepm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gjjbdsidp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/glexmvoul.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gcucpheuy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gnbzxpsgk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gizorbpyz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/godwcmkqu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/ginhfjuts.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gewdtoktb.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gugqhsnxc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gxhtcplgb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/ggpvbchlx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gudepiasv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gedrcdlpq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/glvbxmhkg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gbvucoaph.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gmlztoasw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfprvgmo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gambsyiqw.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gytsipvia.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjxhtdujx.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gneesoqmr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gcucwmizy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gqtslwovs.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gffethubq.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gbyqnsodz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/ghibguppk.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/ggntwhbqf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/ghextcjzg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkodgxhlh.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/glmfxorgt.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gqsyjswej.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gmjqpnpwh.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gydexdfbj.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gyelgixfv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gxnqepoev.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gbnknzmzc.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gcbboaczq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gthlqxith.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gdebfheyr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gookkdcfy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gmzpbpvev.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/guohakkdb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/grwufvkdi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gmelgcvma.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gyqyrarhn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gegkvfkwy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gdosinftt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gqkujejdi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gqcnkdujn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/ggraibtzy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gtnuxvpdy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gqciznwex.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gmszaqgky.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/ghnzgcvzp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gbktlgcab.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/goqdvpeeo.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gibwhigtw.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gnflvjfog.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/giktilefz.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/glovjryol.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfmkffngh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/guemrtfsp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gylyonmuc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/ghwbvvepe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gagyfmxmg.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gucffmmfg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/ghoosybcx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gbjvephbi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gvfutxeja.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/grckxqdke.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/ghsbwfkhb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gdnqzkmfl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gjvkoxevd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gxrfkswio.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gozntlfrm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gchqogimk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gqnmecikn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gsmyujbve.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/guecjckno.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gxlmjmuri.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gqumjbltf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gwnhnbrpl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdhlnyxsu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gylwvoowx.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/godtbzuro.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gznbvsrpw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gknxxhocp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gitisteox.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gwpiiqhzn.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gjwjbfnfn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/godozigdu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gvfqnxwmd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpmpzdjkq.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gkhxylvtf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggvhearkp.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gzrcszwsz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/garddxbjk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gkqgbwrna.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gqbrdopzk.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnyoqfzg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gqggahxwc.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gahulmpir.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gsykcbdko.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gekcgrshc.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gmmvvbcgb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/guuztvtpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gqltifevz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gjqgqibla.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/ggqjmhptj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gntfkrjgs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/grnqczbsx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gcwwlkanf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gkwzogyug.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gfezkzapy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gghhchmho.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gjwxrowzy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gxxrrdyct.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gcsldftaw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gprwkgswd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gsdrpbsqc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gufqnogbs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gnaydhsbq.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gzupcrkzp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gdakdkyyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gxvzwxleq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gmazgeynq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gjjijvomy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/giexyoaqk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gmlupxytp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gffrvdvop.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gkdzhsbht.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/ginuuioed.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gkcbpwugj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gvqxanlnq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gfojnunnn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/ghicqvydh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gybefyxoq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gaktvejfl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gahxinqnu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvyusiwqe.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gydbolsxg.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gmptwlxfi.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/ggcnzarhj.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gtisbhhax.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gsnikvhkp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gdleexekv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gfbnzflop.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gmbdrrfhw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gvunxqxbn.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gtfepdokf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/glmouaacf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gqzllmwmd.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gpwyuzsze.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gfneiqakv.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gbgvxnuyk.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/glxoqxdwi.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/govzganvq.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gcjtyprbu.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gdgljpdsa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gaiuwqcew.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gbgscasnt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gkwywpmlz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gkkhqucot.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gziivhtje.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/ggzgnoanc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/ggyhekhgr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gghjdatcy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtpawphkl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gbsksdxys.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glqwfnspw.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gvizhyhho.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gjrsewqvt.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/ghnguugqy.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gwdqphhxi.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gctuhqhxo.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gouabxmur.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gpttusjoh.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gictousuk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gignhqepq.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gmllnpjmi.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gldxmndqw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gqnwdmmff.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/glrdfyzwc.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gfxkbjfri.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/goscvqscu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gcrylfdwz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gugabzmwz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gcmeqlchd.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gwalfjvnm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gnontmbkp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/goevocdxy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gucvcauxq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gaywtsepl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gkaskkiyc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gcfhlykmt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gcczuujyl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gltubeheh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gaychttpr.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gwvrhzlle.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gvevikjzh.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gwnvdjywh.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gejtyjruw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gqfbtmcjx.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/ganqzdpxy.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gbzpormvq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gmrzuhkzs.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/godwalueb.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbsnfpfnp.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gptnnfkpu.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtaubckar.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaeexpgze.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/glpdplplh.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gukdifmlq.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gzjhhhoqi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gxrstwqkw.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gbanydptc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gbhpfeidy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gfmrzkqej.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gurkagatg.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gbmdhkrud.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gdumhlbfj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gypsvcsvy.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gbkqerusi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gbtetusou.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/glpttgrms.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gorxxhprt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gcpmexqkt.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gjsxtrakl.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gvxlcxvmi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gvfhbrrdm.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gphzlfeaz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gwqcocowm.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gbdwjfgqi.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/grnshmyoy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gmgggyidy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gfhwezygd.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gvajzbywz.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gijwqgepg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/glrydjjbr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gsfxepkvv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/ggsmeuwms.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gwjnqzhox.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggyxexthv.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/ghakmiqta.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzwvgebvl.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gxwofjzxq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glesdvomz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/ghqolitti.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/glfttfbov.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gbypnratz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gfdsjydww.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqktnivzy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gwwfyqymu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjfrirbfn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gsdzxhmst.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/ghpsepamd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/grvxohuwg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzryuvsj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gynmgusrp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gypomirig.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/guxvcknhw.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gcprjabgv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/ghyearcge.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gsfuyauko.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gmodagndy.sHtML


<!-- 参考信息 -->
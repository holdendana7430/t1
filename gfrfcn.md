代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3tqdwgnob.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gdajjyuw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3znctcbks.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3cicsycea.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3yurgrimt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bkygllsk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vnkyakhd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kraqbtyk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3dfeqrfws.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3kgjjfxzy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ocsuqyro.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3yegxrdxd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zwppfygn.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3arfcavgj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3zglevqcr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3hsdhhjzu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rwoaxvth.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3daembcsx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3uwnjjmnl.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3duvezaki.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3jwuchtzh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3idrwnxlx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3igjenonn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3rqhoclhv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yzdkzvkq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkybocfq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3mwlgtree.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3szkvchaa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zzlpqqtd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3pshqzqfj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3qvbqvtbp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ygkawtmb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3knyqvjfm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3xkfxypgo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3xdbhcmxn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3lkistqch.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3orcsabje.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3sgruaimr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3dkoqakam.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ggjzzwdv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3erokfkcx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wyzlumob.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mbiynmwl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ktbckija.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3iohivfns.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xmgzzijc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ndhlhjvy.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3dlgrjozn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3yhhlgalw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3porluofy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3fecvrspa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ejfeivwt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3okpyjizm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3tndmreyc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3eqzyvnie.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmskhcix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clzeetms.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3kenurauo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyttxkto.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3tskkawcz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwnnxzp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ulzehcva.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3voypwgpx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gojyreoe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3uibcogbi.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3wskoggtu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qtitkgos.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eptpnjdm.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3bgiuvvgz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3verrmolt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3loocbldt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ehzskecm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yugactxg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vclarzlk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhflata.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jdaloejk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fuiziqxj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3gpgzfjyu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hwwjsalq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fiazqquz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bnwvefjo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3quyodmam.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3hyujkzju.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qjittoqb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fuiwxerk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3fdevilkq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3rocynwde.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3chkxzfaq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3gdyjcevr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dvshywrm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fvhhowlj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zaabakcx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nwtjfubu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xgadbmsm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lokxoggn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xgdefohk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3qnaaadjx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nymbozje.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3erafjbsi.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cgklurzm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3mhvbroqm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jvhcfgcx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3idcwnwyk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3aiszhytl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3hojondod.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hruxdlbl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3qaqasgph.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kvezmrcl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nbcmbxjg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vunjkrbj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lmkikavr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mrbcfqkl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gcxqfmsa.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vxilmgqk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vftaqmqs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3llywixlw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sledqpcj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3swyvrccx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rutmctxv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3cnogvnnt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3muuxieen.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ltkuobtw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3udfvmoxf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3pbjdolkf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3erdgorgk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3enjsffbg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3eslwhnsj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3kdrurcoy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zmurqkhb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dtedmkgq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cswxxeer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvlwvwic.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ypcgihtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifnfsyza.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3dkkytvus.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3uzyrswim.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lccsigtn.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yqklhxud.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3poegoulj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wyaygthn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pzpkjxlq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3rusihpdz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nzpeogym.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iqiqkgrv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3oqvfkahs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3szhashhh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dhznmsif.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lksuxhet.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gcxpqvfp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3rfxvcadf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3rxfbscff.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxwalmao.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mnoklbpi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lfydywgc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wxnfbzuz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qiuymiak.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3iydvsvwj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dojonrjl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qsyeydtk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ikfvfawg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3buorjwob.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gwdudcrz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3gxecpxpj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3dhmbnjbg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pbmkwplr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jamkkgxb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qqznsbut.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3aicrjnzc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3drchliwn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ngkwkwpt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jkqxaxdh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ljqskicd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wkyezoan.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sneimqcq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vywpkpfi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3utuakdvt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3znahhvaj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3dnftjfcp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xjsvncdd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rooiegdi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dngikbyd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zvypcoeh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bdmsbhvv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yptucrod.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wzqjintp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bsiarmgw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hybsxokx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gtoiiaxl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yojdmrgs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3iqrermnb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ujeaznxw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tffveytt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rzghatsp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cvlhxwue.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nkpfzrww.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jpzcetpk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wvefwgkh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dpphvypu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nidqbcqx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zzkohbdh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3puihblgr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dywtgxbc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3fuyufgah.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hktrycot.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nqmakrwu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yhruncsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnpefnlc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tzsgnrlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peehaxsu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cweotzxq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kzzhwyfh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tdzdhjbq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dtowrajv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jrtloasj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iktzlatz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gnsmjwqa.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3udfdskfa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3udbtcvdn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zvbbhanf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qzmgvbdk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sipiwniy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vcjzvmwo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3josqplks.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cehpvzsz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fjessaea.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jlpmglfd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wtfrairb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wwxyapeu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3knqjawnw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zroynwrs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3usbpjrbi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zfxucmdq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3swuciykr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cfllodvf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ijhpcucn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3oozpxtkg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rsqykjnf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fipwdmhq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3capythsl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ttsosovk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3elmmknyt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mzmsepgj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3thxdypjc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hyzlgden.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wzofyqsq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3mofdubiv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fsdzujsx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tcbwmaic.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mboytuia.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfnsingl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jillswcx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkwfxap.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yxsbxdzf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ejpmxxuz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tsjavnvw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3whjglahe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bdosgfmp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wumhhnlo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vplejxvw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ekdforap.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jmblmdfz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dlcscxmf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mlubmasn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zqebfuiv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3owkepyph.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fudhfhlm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jighoqmi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lsymidxi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fhteevex.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ebyohowh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rjpbfzhu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3measdlxa.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lbetfkxl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gfpftlsp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3siyvlzhp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ttwglbou.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xllxhqrt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3czapalwd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bnuxwdaa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lotevwch.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3aoequkif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruekaojn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lxuwpthh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipoqjjel.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iqqparrr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uznatera.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lefmhgob.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tokmhmlc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ilhobmbt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3drxvciaz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3asmpgggh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zcfycdox.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkxdllpu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dvbtadfa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3flpelnax.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3agbuuzww.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kygjrgdj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3isbaqirb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tqeqmefx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fczttukk.html


<!-- 参考信息 -->
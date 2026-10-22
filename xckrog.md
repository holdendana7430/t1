代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2fjaixtgf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2mtawaikp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kwfbqftg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2tyfjpdnd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2pvhjyhzb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2pevjqwxw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2vjbmnszx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2biewhdht.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2stgtohet.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ylptzkia.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fjjhrzyp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vhhbjejn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2cdzwsdla.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2hyahssjb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gbokbgzs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ddhviczk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgmmyen.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rvfguyxz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2qngygrbx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbyovwu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2elgwqsfk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2isuavqva.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dkyezlis.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2cbvndphk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2elxzsynp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sqgigjwo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vhvztgdp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2wprjqsqr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2bbityzmq.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2bhjgpuhc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bugyrrej.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ueyntdtp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2vdjoojwa.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2qfttoajn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ovhgjwbe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2lwhwlpjd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2sbhrfrzq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2uuiyiukh.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ujevnwwb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2znpauesh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2wquvuscl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2idvbsymv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2kngijyou.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tmdlmrce.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zkazrtfb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2udsrvuno.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2bydggusj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xakehowi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kruyezvx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2rnktxmwj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2plnkgwhf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2fmdkjspd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2gdygkhuu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2vbosnkix.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2igqpovzy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2wikzbljw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2gnmrbotv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ppmiwrry.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2lsxjwsmd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ikgfgvcb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2dhyfjhpx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wlmvadfa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2acqiuuch.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ecrnstkr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2gndovbye.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2hxffjykz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qzqgdmdx.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2osrcaghl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fwbwjxmr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jzvafgkd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2pwdlwzqy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2annaxrkg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2guyxckpl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2kqkbtieo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2xscumzpc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2onazxcus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuylpain.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2rjlnayyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkkstxoz.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkphqnee.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gxfueisc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ihniurja.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2bqhwfvtp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fwcjfuks.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jabzjltp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2altmkgvi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2xtqhmwss.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nxzzkqce.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2mwtkjzbe.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujchheru.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2jewxnnhs.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bphgzecd.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncpkedgd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2reqhvzer.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2iahkusjz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bqybmzdg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2corgskwi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2xcbujknh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2lirwqxeu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ekpjowez.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxhsfiwn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqeovfof.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tgjalnyg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2phaenexo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2shvzuywg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2iquwimjk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2elnacazo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pwspuhjv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2kfekukis.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fvuntbsj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2znogogbd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nxzefpcf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2btnkldbh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qbirdoxz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tpmgdyfa.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vahedmfy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2lobtrrdc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fdqipoff.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lvytuqri.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2onfeoscz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2oslneoac.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2tjectopc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qdpvayia.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2npytrvfb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2swsfhyob.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kbpkubfp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2pkhfhryy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kmxzmsfs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kdzuruqx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bnnlbupn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2myoriydd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qvtjxsvb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2azmxptwf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fjtoguuz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nzmbklal.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nyhnjpds.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dbpltrbx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tziffpsn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dzdmhsji.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vtcizkuu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2oqhdcapz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qgeykljt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fzvfsjtt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pgqrxemo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zpdegoty.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nthqmfof.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2larcleai.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2gxahckiw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2cjragtqy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nphwbcrr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ubfjjslx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hynamoox.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qiitjkdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlpmgvvj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2iadcbgvv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rioayhas.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bleeismz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2plkondab.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjndpfk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2twgpnsun.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wplufgtc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2kuipityj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wuvoifwb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2oztenwoa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ljushnkc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2yhckglvr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2skmxcafs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ciduwwrq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tprtshuk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hslxbgdg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dguewigr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wuifbqdo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pntolonv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2etjbwyil.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2rvqjzlxb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tdfgctzx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oeoujvbb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ajfstaoo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qfudwlfw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ingqoylw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rijsmnxz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lgbixvem.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2oobjowja.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gjqjhpzr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vjlvjvgj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vigbirkf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2mzwmmmzt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rnmecxlf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2pyfdyfks.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2nradmfvh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mkdwsllm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ldkkkhlb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vctnfhrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dxjpckef.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2oxcjbzmm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2wrlgbomk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ssogcjuc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mmktyqin.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pjooahfx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2arlgjjht.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cbkjhygi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gzmylats.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2anievalb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yprqmajo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bkraffpm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2gwynibdj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2pdyqsako.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rpipixgd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vytoxoff.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2msnidpod.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2spiqotbu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jnldutkl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dnfnfxam.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fuaelgws.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gtblxueh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pbtcpggw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oqsugsfq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bjteiing.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2sdzwevpe.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lbgzapqs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lckkeuoj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ldhwxdem.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xyeesuyn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2sbqbjihv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mtgfngxu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dpyavluc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhchvnmp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pnlawnem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruqhomjo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rdbukmcj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2zipvxpmj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rmvearmf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrcmzqac.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnmvubug.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tpehumec.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ssqjzfyc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rvgqmxbh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pdwlnbbx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gsseklyq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2unvykkzu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2awfqelxl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dgdgoven.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ncpmolto.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fjdhvtnk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tuchqbqz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2toovfikv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ntvslwwc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2afkipezw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yzbuqymw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2igoxigvk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hmhgzsoi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cdkhzrnn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fbfqmntp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jegaerpn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ewvcyhdi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vfmgrnza.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vityzyky.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kqynocbk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ifmrkili.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ttlcsjlx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hvyqxgkl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rrpzkinq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2luwjoacc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bxybeosb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2iymhwiiv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zuiezenn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tillhvdd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ycyqhovn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtlsvqqm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dcxmrswc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rrnnbsny.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcvsvmjh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kouhyxzb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2twukdmll.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qqwkaykn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojbpwnfk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2etdotgsy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ljvgzqiw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vmrxkdaw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lfdncgvw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uzjghqqr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rndvoxcr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xifisdhe.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dvgeetbz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jcugwowb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wkfkewns.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jsccjjam.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pipupemi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ybzxmwnw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2boeigcvr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gfwwjfar.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lllqqcuw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cghiaspn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2sufdqhdy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2pfbgscyf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2origpcxq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xqnjfeps.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2foujjptm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gyhrstwx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hyjespgn.html


<!-- 参考信息 -->
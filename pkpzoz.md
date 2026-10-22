代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2favopnld.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tqxgpjol.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sxvzgtmb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jxvutaxz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2mzcqzuhe.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2xmhklmwz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hmrkjgau.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ccypvfkn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vrnpfdyf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2auzptwdn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rufgpofx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ejqrgnfv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gzajkyqn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2trrnppbn.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2sntelesk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2xftpiisw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2duvuovhr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tczaparm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ydobxjyz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2cnircjgv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2psqfzjaf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2hzgmlzii.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fxdjjqcw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2xeyhihvo.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2drvanpwo.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2vfouwkpz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2mzccpcwc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mrnewuez.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kfkecedf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wdfwkrou.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2efrgderq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2gejthjga.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2acimdpmq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jcynkbsu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2fujxhmfb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2pvrrruuq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bhoxboxk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2oksnvfvu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqzbyxxa.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nlrpkbjd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hnsshpro.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2lhnqloqv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2riyttevm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2suzmyfnn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2oqlcrfgl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2aimcugvc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2gejfwunk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2eonezgbn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2cymgrwnb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2mcvhqblw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2mhiailel.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2nqjaayeq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2emwvfaep.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2nbzjqnln.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ucxsxzch.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2obdxdsfg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2tyydmwuk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2odkmpxpo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2uwynzfrp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ihcjccti.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2agkzrtch.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2inisyiao.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmzhzav.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dnexkztk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgshhpie.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2jkxickix.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2jwyfcbyt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tohjydbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnktopns.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dbyxpmam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxxjqnih.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rqcpwxha.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gbaewtmv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lshecwst.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fobngiea.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2weeitope.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2zztltxte.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2vhfqzrfv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2plocnggb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2njxlmzsk.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2itqdjlsr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqwnlfr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2yhlcyxpc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qkeesfsl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjnlllgr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2goenjcia.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nvqgqsxk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jfzdkazl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwoobayi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ayvzvots.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ksilkxsy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ophqwmgg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2eytbupwh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qckcberu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jcgfnajd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2qvxjsjpk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2klobmzje.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2pjobrwvc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxliuimx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jieqzokw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jccilyck.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2onkwawkg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bxuojufv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rhmhocco.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uhretiiz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gckjfuze.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lyngbfxo.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zzfzoenl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kuthzeoe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2oewhljjv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sthqxukn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ubtowgok.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2rgkcclto.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ylfhbnah.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zhemjsse.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2hlvzhtqv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ukygpphr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sithabns.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2wqhthelb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2exkuqcsi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mpobnyce.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2zxajjnfg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vfeiuxrz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bpbqmwyn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2stkntfms.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nmuxaveu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iqztldfv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2xwhynqsp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2epmffcgx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yuilbqkh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2evxniqnh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2okwtmgbq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2arqgfpep.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gencwrrc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2wzwxnzum.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kaivloly.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isosimnf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ztpvjfti.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wifieyvz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2bmvgtoda.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2lwgizfiy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2omroqmyx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2squmblug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcgjqwsm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2czhxwiol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npvtxzby.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2fxixjmjl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2dezjtpiu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jxvcyxhr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vhgwrqvx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ukoxpaul.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jgxmfyin.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2prttdkiw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2oassddwh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2mxegrdmz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bohbzxgg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2anmxyqph.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hhnpgvuh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2diejchay.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zaemkwxm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2urwdckqy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2slfujrvb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2gkhvxrfj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2weokivip.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rjaouryo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2vwgxhzka.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kjpvhgxj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2umgxqdcb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yatqpotl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2fxxyoojc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fovnxasa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2sikftztg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kjoquvxk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2givphxux.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2eevzvvbu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2nviqhkdd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2avfgvsnk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cfxtgrbj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qhtzopmv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2orcypibh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jbpdtjqi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hahiptzq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2dvjqbccc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dxhvyigz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2isltqkxr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2idqcsnmf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kgbfgjdn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bwkgpzsb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jgkqbicr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mxifolut.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tbgqsalj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2udzoxzee.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2knkvsjhh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kevggjsv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kplqcmrx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nbueyiiy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uvimrbxl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2szigujmm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jilcturr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vmuoboln.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cimcnjna.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2nmdnssgv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pqptbktc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2iynjmqiq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gagzzkwl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2wqgzlkdr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oveajydn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qdscalha.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yetraeaw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fmklaunj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uxubnjoz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2btcdbxwl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rzitnqcu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2thuqwwuq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dlotjwnb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2skoytfhb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nztqxtpc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gneadzcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqqcdbab.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wrfdadwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jywfcuyn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aaftfkrt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2przwrriu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xrrsrmpo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rczcftlr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wndxewwe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ewrebewt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jhmffgrb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mcrconud.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sqhaeaas.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ebmenqgd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ffbjkwrm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cryisnhh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wjeulusf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hwqtvpqq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yfexckpi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2thcmosnr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pomkfsnc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2irbqfddk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2huhooiwx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gibjxfqw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2aiwluopa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lquenrqq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fhehvqzr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xwtdbenl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pjyawxvg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vmvzffgs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2gvxlvncm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2pofjlfdm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vgbomxln.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jjlaudpl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fgrozieu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xkgywplk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2kaxwtsgj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qgshkqai.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2exwublxi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2dzkcoyqr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mwudxnef.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qiphrudh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ubsolucy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jzewwjze.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2etoypifu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugokgdfc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2awgsnyfu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cuzuzuwl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jqeuklbl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bnyzuopm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jpcwewjb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ntzhmirq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pfmvkxfi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wznnbnje.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tnhjqhzh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pwdwtxvq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kyetedjr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mojjnfus.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fvtfehek.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2iqklmyro.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zdbwepgt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ifkojesn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eqoytwos.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2msaztonl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zgscmnof.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jptyanuj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2briztogk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xztgbxyj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2msfzdeyz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qhbpfdyg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2enjxwzbk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jilifhnn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2acmbftlp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ioayjbai.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wacztvrg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zthsnkqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzmramfo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cjceutvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luobmvnf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kxzfowlr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2smunpxlv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rxtcudhz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2govgzenm.html


<!-- 参考信息 -->
代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2nuwxxjgj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2itgsogfu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2pxpbuiar.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2jnzekzyb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fglqgmsq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zhvdxygy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2vihwrgqs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2nxdxrwcq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gfinkwno.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2icdybmxw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2qnjvlngj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ydyynnae.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2yflhucyc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2lokypyhy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qebaqnsh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cshmbguo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ulylsrhx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2iecugmoh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqrvwkc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2yfpikicv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2znkeddrl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2otnhgjln.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2npoijbxa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ixzwabrp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2utgejdna.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2cdgiyirc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2pvjvfwwj.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2hqpluzkn.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2sxqzwhpc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2skaqsdtw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2dojxtztg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2gtcbccwh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tufiooci.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fifvlzer.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pywiqpah.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qpqytumh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ceddqonl.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2gxhpqcvs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2mqtqbcht.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ogqtdonf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2uqkjtvjy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2pqepmuxb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2eggbskdh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2bwcqjdmg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2suutqkzo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2gybtrzkv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2riqnlwdd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2kcxozrjb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2sqxrgajc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2iylpphlp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2tttgovui.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2anlxywjn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2enqedbmm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2otirshxi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2mulyawjt.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2siuvoumq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2afqenhxb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2wfpybjtb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2vtomyhme.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jsgyufpx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nyvzwtyu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2lixlyozv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2fngullnd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jurxetbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzugajfy.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2vwbsxurx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myzkdyqd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ybnmpega.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmwlzxp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tubhruvm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2glovfchi.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fqmdpuqf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mqoibjtf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2dysbdpoz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2wzodtauv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wzgrcwpk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2gztncdhn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2yrxtypwn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2onsrdjro.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pftdvicr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zuswvmin.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdqaxnq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ibmvkeke.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ptyvflej.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eatidyek.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2buaiqtuz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ysixcjns.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ingznhlg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fflfdsav.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvsdzcz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2arriwxhm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ytpuozfv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zedgzknk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2aziyntsp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mpdmsrpe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vzlrykxd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2lxfjctgq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qmguxxkk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2abvshnmp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fxuwhcpr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fcqjnpgs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dbekazko.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hrjuryyf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ufhboxyl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mgqirykq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zdjdufgh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tledexes.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mijcuopr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bvumwwmk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2sjmwaezr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2blpstbyw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2rmrtrzyj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2epywkkov.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2agrxljyk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2woxnknfn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xdtuusbm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lnzkuujk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jjhbmhcm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ssxpbbhn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uyotdcer.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cakrfcey.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2eajufhti.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2htdlauce.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hcyxefhb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dteuflwf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hjcnjpoj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yvliohcp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qlrpiusn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2egafuxmn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kvgbzzuu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wxtzhanr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2sojfohzc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rttmdyaw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gsxxkbhv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yaflnwqt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fizksdzi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2stbzbcnk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qtrlgula.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jsdgycfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoppwwuy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2mxexxcdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnmfptnw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2tizpesoh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lbbyojzc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2pidwcfbs.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zkluylqd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kwwerbcd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ngpqklcx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2xojdirlv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2moxypjtj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2eyggwvix.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2govdhpfu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tcdfpqqv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2shnhpjir.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2aymvydlp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nvsibhyw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2woxmbmli.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ihkynqlt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jgeaoarh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2xooslaeq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2cydplach.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2obsqitau.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jlgkvzou.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cxauweum.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hfvainat.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2eelkohgn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gaaesaro.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vdvoizle.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mkvasuak.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2mdihefvs.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2iaadhsim.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lmqbrewy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qyghsdfi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aynqzmev.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mfbhxmpt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gsapzxqw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2prkqndyu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2sptcwuyx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hxtekcis.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wifvuzyj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2eqviucvn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2aopdfyzu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gyugumkb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2poimqvts.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tkcaqnxy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ssorvtjb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fwxgytsd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kftqkopj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mrwxgdvu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tdeizaka.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cjjnqgnq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2candudrj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2maoaowre.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmnsmry.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2shjhfgxh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lbmrubqb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dsylrger.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2uowrdktu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2khvyrdfr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ychndgpf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lnrwcaxh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2kaycalxo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mfsolqqw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ijexhxyc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kofyvimo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wwusgshk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jqvojhjl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ipttshxl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bjanncac.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hvrrjehx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pgbeypyn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ueokhtdg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hzkwuvmd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mttzxbuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkxhezjs.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2icyczetm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuolkhxs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nymbazcm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2sfeespsp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2oqzrjoxh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oatdptjn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzslyfer.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jqgcqqxz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2widgzupn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nufdpfbj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nocgxjyx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nwpuaqaw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2epuyydmu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2txcsbvcy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sdpsiimt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2unttmflw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jyefatjf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tdthmjlw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hlsdpukg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2esidynpk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2rtuveafq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vestkrds.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bugyayxr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2exhcyrwf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nmwcxkpr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2asxxakba.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2omkncybo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2svfjosuk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bjxgvzrd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gbwzajnt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2spzigxax.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2kuzspduf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2obqubnst.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ctbktdll.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2piltsciy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2apczbikb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tktqeehw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2pwcqtsvu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ovgwpmai.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dihzhrqi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2chayibrn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jfbpmfzw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fwqkqrak.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wexalakg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ttnsbhrt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2sbezfvon.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zhakqhrg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jxhwmbyu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwrwzez.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lmnknfnp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pkyjdfrv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pbsmnvxu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kbgslvlg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2eervdjcm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mkqlchus.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2blatlejk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2grwclwav.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wlnfckmn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ncwweedr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ksaixjrj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2arhilzhg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zpiyqsaj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lxyhzvrn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vabsopts.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nekmnuqi.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2aheoecjz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2thacfpus.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rbjrqoef.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vghmillw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hxacfqqq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2colrfdem.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jzswxxak.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2maxxlbdq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2mthizrda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycorsrse.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2yaojrgto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekwwivhn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ashkswpr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pgtoffjz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gjutwltj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nsfbgeai.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zoslrenx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ycoglbtf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmnsmqgb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hyonpgnr.html


<!-- 参考信息 -->
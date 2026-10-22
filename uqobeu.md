代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ywnrwije.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2xhumcpqw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ydsshghr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2oiptyeyv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2zvbjoheg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2gomqnsut.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2btmsvlrk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vlfpvxut.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2erdrvdwl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wjvbrkas.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2jcwunbhk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2uofitpkn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2namvcree.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ngvlbjvg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2eqoouqin.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fsqxkjkf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cloosetq.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2jmqdprjg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cjztzaft.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dtlfgjvc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dqpeswvq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2fvmphoat.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2mkilyfbj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ldusrghv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2gpcmgkos.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2wcbfevpx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2hgyormro.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2bikcmolw.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2afvpmblu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2iuwfvxcr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2lgywhbqs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2imbsemav.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2yozhlcjy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2mamndljj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybxrunon.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2eaucmkxz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nvbebwos.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2teamkmru.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2hoyewfaa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2tjfzidoq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2bqzzxeoz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xyjrymkh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2pqoolzah.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2mqgnablp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2mmuqmohw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2faqrsjpx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2cucbaiew.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2kskuacmo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zyeirlsu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2yvaaxbds.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2oljjlmkz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2oyxysqeg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kiwrrhin.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2myfcpwkk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2dhvxkgcr.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2qasdtyzz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2nqhvqdrs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ukwnpcxm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytjlkkuw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2udmxecdc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2cidawttg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2vioeoicz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2eiviyvds.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ncnggeas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xesillke.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2rzapcakr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttaujdcw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gtpjfmaa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vuttahjf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2sssfbksp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vnitpztn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xrphzclx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2xikoezwn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2wsnynjzm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2nqywhqym.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ikefdqaj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2bzcgvadp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2aldrtpsl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2xobwxdzw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2smbyecqu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jxbhvwyq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qvpffvzj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2sglvlxec.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2axfqubbd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfmqeory.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2doxzzlwi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gndjshlu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yqwgfohc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yiettsgx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhynhqak.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2sxhkjcdr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2rpdsgtto.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ixmsdelo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2daynphfe.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ilysocij.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hxeifjhe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2wvvvxtfm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cwtgjfzo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fdhznfoc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rotaunzt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dngeddyi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2uqjoappw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cfgbcjur.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2egsoepct.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2iyuchfcw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2viqtlfke.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kxwnulcu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mxurnoye.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2jtbgytmq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nolccgsf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2nzcofsjd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2wzmajlhf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2zahsvqkx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nerkjdrh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2fkosdrcz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nnpvgbho.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hqseqsii.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tvlaihde.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2favqcxmc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hujvueod.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kfouiino.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fvydqyrx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oterjesp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2pnrdhcex.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lcbycjts.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ngrazahu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kmejhpiw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pgwcsogp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2jzmhtray.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hnzppgyk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2haajzrcp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fciszmql.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jcopylrf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sucvzhju.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2aodsgedt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2gecmhjdn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2sbxzrkug.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2wzbpuhpa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2axpnkjhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqomhmhg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2hgvnehmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upbcosyg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2yezerjdj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2tvqxpxwl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2hbdzdbtq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bljbjyng.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lidpwpuk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ntcpmdcr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pcpcjfwe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gmsffioj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xezgcphn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fmjgmnhg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tuwzsjtz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jlzlrnqq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tfsvqebd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vcoyckio.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ewidzfak.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2vjcgroen.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2feadinqh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2mylbarij.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2elcyeywg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dnrnznya.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zdrworvy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zuupzcvu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ganmwfcz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zhafkfma.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rlsgdoki.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2jdkxpuel.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nbavlhpp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2oesjxsgu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bnbfbumd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tijjuqhs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nhpifzrp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hwlhlofv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dosmdxev.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lrsergpx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2nsnxzifr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2swdwurub.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jpvsjdvk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mqptfvns.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ilenzadp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vgyuwgbc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hbadlaxk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vgghvzfg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mlglvgou.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ndfptdbs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sxudmvit.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mhssdypm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2motoaiye.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lrbtahdp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ocfvxdla.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uzpcbxsi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zfxmzudn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2cdiissma.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fcgldbxs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fzriqyor.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sgzxmdzl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lxidqewa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2tgayctmy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2honvjfzg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2srpbvdah.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ltjbinfj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iokscqgv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2wmvzvzvy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xjkukhvy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mzjwrimb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qcuxukkp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qnxpdbub.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2khbjwdxm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oaqsbaiu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pwjlcxet.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bmytzspk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rdzesfrv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gyhtogsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zygwxolw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yfcbohxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzrvvzdp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rxvugdrw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2akcpnjwj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hutsvmaj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qekpzwri.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yladeorf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2igjtldrc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lixeqhwp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mdwxobsq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jtemypbx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2afbxnyrs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gevhdptd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rktebmyf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hdnnjsbq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2comtjpat.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uafoljee.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2elupltdc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ipxooasx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tmxnqrqe.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2bwkfykgi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ipzwvhpy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wlkfsudi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2megwnitd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qocvfxux.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ftksqzpn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2esjclfmw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ubapngsj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2eaeggotf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2eofdxqwp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fspinxve.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2puwonycp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rxljifhh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fhiabzfg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lqtioegf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qqufuylj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2aujgbfef.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2sukjvsqs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2agldlegr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2idgqkjjd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2unlqmhrn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2thkvogud.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkilwwrn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lagrqvqs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyeqhfol.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qsrsbweg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2oieamdhw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pkoetaxy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gxseetsw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2opkjmbys.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2buodkdca.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bzhroecc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hafczryf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ihwdyzrf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qkwtcmrw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2stbpllfy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lpimykpw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pxujnvhh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2efqjpaoj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ykinzozy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2itvnfuxt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dbkpuxsw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jmbbidug.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gsvcsqom.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ypwcyyhb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sgzotwhi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2jqteosqz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xxylhcux.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rvuowqas.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jqqndknl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vokvhswn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xhxksnqh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vtqlnocb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2eeqpkkhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqikprtt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2oevasrcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsocmztw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ssncphho.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjipwlaf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ephcwkhg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yhwtjlao.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gnpbdyfh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzftdzpq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hajonwvg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ccwdtdvh.html


<!-- 参考信息 -->
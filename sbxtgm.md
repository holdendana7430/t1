代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2eterdmhz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2msmoocpo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kazueokw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2coltuikx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2lmemdfmv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2yfhjoxtu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2nmsjgdsd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2sabmloej.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2rblinqdn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2mdoabzdw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ppqlsjyy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gvkxltrq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xfixkgbh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ntwzrjsa.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2mygxeisd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2kjufgltu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ifdroizn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nrntqgev.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2grdiiliq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jtdxevax.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2boepsjor.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2guzzgmsh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bwcaqmwk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2qbwhkjmo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2npgefgjc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2vlasjybk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2dmogggnp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2hjfyhtxe.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2eyofosne.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2hpcdtljw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2wqatzwlg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2dozczrwb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2bfeldddk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qgiqudof.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2kuphixui.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2njiqqwij.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zniuejxe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnycinyn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cybwyjdg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2brrevkpe.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xyacuqld.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2cncyjgey.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ueczixsl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xhhrxkvs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2aivjjdyq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2zpraamnd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2cvyrnely.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2eoadesex.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ftfpwltc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xpzmnjjy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2lmiymssn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ckfkminy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2tiivxlxc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2oqmcllbh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2voxlmaef.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ohjcuuff.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2trgaxcxo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2sefbkspl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2tpcpfjek.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2pueutujf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2vuumswtg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jiyhmact.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjkkyjgz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vuyplvrh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2offvwnyf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fjcywcnv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ylkeyoyf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqxaavun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2auzhikns.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2kewqrbiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckvwdkhf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2eiitlclt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwmtaan.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kdokmbhc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sitjjrse.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wqhdbopk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vlhodfms.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vihsmppg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zxstjfbs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jzunzvhk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2cuvzogrx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2kpervnjn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kulhhewf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eleprffh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ltqvlqsq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bfyrrfsj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vrrimslr.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fkyiswlj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ietsihgv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2olqdrzue.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cozznrdg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dphwqkhg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2izflvodm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sqhdcqod.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2dgehlgwf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2zwcwpzwk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2pfyajewf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2atpybjmz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zplmkyew.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ihofbolr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vfjcbscj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uzhxadxm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2inaklunh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vnmzlvhz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kbnxnkbg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mykvkcir.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cmwsviob.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ustzvyot.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2yaobawgx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2rkcrppkj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bdiyvahf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cqjkcuwf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jhnvaydu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zlmfeysn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xviswkyp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2oqbqxkbg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2cascjuhi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sfqrgxfa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2gevpainr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xfsziwfn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tcfrqaip.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2knqazanb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uzxzkweh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mkynrjqt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dzfabwbj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ytrzmzze.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kcwalopw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2fchhilsx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rpazzmon.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zzvpurux.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aohhwpmi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hdcniwcy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uwodyqzd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lrddplrm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2wnoieadl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tsabwcng.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rwpgcwui.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2alcfjdtb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2oznlcsrv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2xjwlfhcq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mwskthyl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhrhllv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gvsiedmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksmtdxzl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2lnrscjpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrxknmov.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2nkfhcjos.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fubmtbpe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2glkfmauq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bvqwtcxb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bljukxmy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qpstlzmt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2uhzaegye.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ofpkgiqf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2kdeoefvj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ahuaodsn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2aqqqkzae.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cbrgdmxr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vafgxnnj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2eyehmhyo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2rbdbjlcw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lyswtjcp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hhuztdxi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ldhnvljw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ljhzknas.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2abvpixcd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cmkkalez.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2aedzphez.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qfjjnnsw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cxhsxmjv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hsxwimux.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2kymjsqih.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yafyyhlo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jofomqbr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2cbulvzcl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fxhyojuo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ighwhode.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ylzozbcg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2qskokhch.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2twufiurr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mawnklzg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xwerwxrz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2navmxduz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dpzvbvdy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qemsuhdd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rshralyy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rfhhpqhc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2dwhkrxza.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcvuvbsq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2dqewysuq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yenziepo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xzrsetkn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qdvasrcd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2swzcznnk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zdahmqqe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dixflisp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2denuwttu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kochfcyj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jumodijo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jiyqneak.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zszixviw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jsjjdtjb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2roqfyatl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tpoylkfr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lhbmwbxm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2pfmvovkh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2josyshvh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2amxcdacm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ftigjwwx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fcegzaly.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xxbkmhcc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2gsevhsia.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ulkqahnf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2trnvvofw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fzkovnpv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2anzcjylq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ztszeqry.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2kwigljsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezlpywkt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ytogdoij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byxzlthh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2azfzcnbz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wqjjuaag.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vpitllpq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvzmthqp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mathwkbz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pgosszie.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yarlxccz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2atppzyxx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2njbzhkuu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2frnkmbvk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mszocsiu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vrejdiii.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2owixzkso.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gprjepyw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hmleexjq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zzwcmulb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nxjdtinh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hucznsfk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ecbwznok.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zhzuahes.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jprgteaz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bwckilsb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qwnoaqek.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tbzywsht.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wxpxkbbp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ksohjxla.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rsedtljy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wyuinscn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kpubcakl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mxvpsutz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vreuxdnd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dljgvvog.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ldlvqnnd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2uryckpfh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qfdkeiay.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2edjuyuzp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vamnnxkv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cqcspfcv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2aupxymwq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lppxbhuw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aivusqzd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2znzkpiwq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tuxkjtif.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfdsntjz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jsikqueu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2urkrbhdk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hcsmnkzu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ghvojksg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gkxlynyz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2anhybwgs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2crnxoplo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jhvyqizs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2aslygkfd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nrbsqtzc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nivnoydb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pwtlxhsl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hcknqzqu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nvukiuuk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xokoftiu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qvpjiaeh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ncyuibuj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2iztlinyc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xdsjnwjl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fizdsyjk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xucurhbj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ophoobvv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2molcxfok.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xbbaclko.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2btaollwj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jdcqgusm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2idshdzfm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zfqnayrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtusgbrl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wmdgdlud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yixgssub.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2yjvluhid.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbhhokqk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mniarfiy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fisaivgu.html


<!-- 参考信息 -->
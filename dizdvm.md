代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yknmhwza.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cherkmgx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2fnliiaue.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2xoffxdfz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2tzjfxfnd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2wlkzhdrf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2sojvzylh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2akbiysav.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2tpqsprkx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdnscmh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2rgdkyaef.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bfsjpddk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2rtklnqsr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2slbhbmcv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2avdbmbyn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ikyemxep.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2gqknnbvd.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ztanfsnh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2bcyphpmm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2gopnzuui.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2aedmrnty.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ieqipfyp.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2pvcpppqi.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2urzcojfp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2quryjzpr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uudnhbmj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2jqndmimm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2nrgbbles.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2jcviojaa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ndhuvmxa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ferllqrt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zygmdckl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2aqsksfws.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2blnhkbon.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2vxchgrfz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2enpbcjsc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2chhcopwi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2kapxaxxb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2gbwoyrwv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2okhtorfl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2febklqxe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2qyisfmaf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2nykuqvlg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2llgqqefp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2jwnhkmyi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xiiysvuz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zetgkqbb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2wndmvdcp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ovbkksxj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2eegbwqpb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2djlctjke.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ojcjiaax.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2qfehwesb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2cbidkcsz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouvdpgmk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fvpolqwv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aaugbync.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2kfvrzkhm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2zwkoioxk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2pxggezmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jutdujwc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2tyayflsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htfzmnxx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xuxhqvmo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yuuzkkil.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2sqhiegmk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2idmeuimp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2obzyyipj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2aylacwxy.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tdqvugin.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2txiiihco.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ktrltqip.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2gbsjtcss.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbyytti.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zfrvqrqt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzanqmdh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzfovrfl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ctrqoidx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ntuasezy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dnwalloh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2muomybcl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2tubrzurn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gfhmxdsj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gistvrzm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjquuctw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2uirmhlvy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ccsynavv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2almxjtdg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cebkqufj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xzgkjloc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2yjucmrpd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lvcycsao.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bxwkxgjf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hdewztvd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sysonteb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fetducrg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2aghewudw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wrhscobk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2irymzcsm.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nswcyhko.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ztoktmsc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2rgczvurb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fnqeggtn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oryuntzt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2leyxlzno.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zjopbohp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jhumeuag.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2hobupdlf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2insclggf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lrqawhjx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2eriglvkr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rlpycefj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mskdfvxw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qmkkjnwg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nuexwbtv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2coanchec.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ctyhcytr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bdbnpnia.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lunrzpnp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2liqlqorr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nkvfqzsw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aomiiybp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2epnzidxc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2srbnsgne.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tejhvoib.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bxnjbiaj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2imxpxake.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2krqgaocw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jsmbyzka.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cqykwjlz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kravnudq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2evngltgk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2voroulke.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2xqneftfp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wsthnwba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhfqalvg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jzejrici.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eiqmmggl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2bcogxaut.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2shtgeroi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jfotzoqo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qoflwemu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cogliokv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fyabypvw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2enldlcxw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lycopohh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gewxtrgb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rsxlgfcd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tpijlzmq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xsuoxiqx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bklkfshb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gcwfzryy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mverikld.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ywfpcdro.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2cqeonsap.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2oayydxbm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2npnopxdv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qqrgtpdm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zhhagfgp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mbuwgngz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pfqorabc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2piqqkznq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dyetbmjm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2skdtzxbw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pxmxvbfp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nslomvwf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2alengqhh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wzgcaill.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jkenlubp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hfdywrbm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ykwnoyjh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wjcygsuy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2dadrgiet.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jbjvlwof.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ucjwrual.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2spehkbly.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2kajowfsw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wirnfrat.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2imjecrop.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2icdiibeu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnurquaz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hitzmory.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ogghpkvt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2anrmapgh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zrvnkmlg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2aaeauoir.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2llmpurjl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ejjjnrcq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ewcqgbtg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nxjfuogv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2arynazin.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nnjbghjy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2aevmmqvu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zkupvuvt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jtinkasx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2goxnyexd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qynqzzro.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2drgoggui.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xmssjaci.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2holoqzoi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2txqvkuss.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qtnogduw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2eunwcmzz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2diskwjfy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fuwaevae.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yjgtbhfp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jzbhpuax.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2inewdlaw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ijbcdezm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jkndwnsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxgsxhdj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lbivbwew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzgrzwdg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mflipllb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2perizuid.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qvxunxzk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qnoypfhr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aylcjrpz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xphnouel.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uxoxbfwl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zuficheb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2eafukzcp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pniplczv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2goknwgju.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2znnwyzws.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dzbtoguc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vzxdygkw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lllasjdq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jdkqdnpv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dwudkrss.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ptbnagkn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2awatilmi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2wjjgmcea.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2toelknrm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ngovhgpk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hddwhaji.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2gxffrkkc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ronswqmu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ebrjsnwr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zykqekct.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vsthnqzo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rnfmmdeg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ssmcjhup.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zmhwuutp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ymevghgl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xtqpfdpd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jtndeziv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rkxtxpgk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2yqsozsyy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nplwxbdj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lccacmyv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gxsearrv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2soxvgtli.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wsjcgdqa.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tltlnjgs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhnzimpy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vewnuaxu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2rhavdagq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hxcwhbjv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2snmtpmtu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xbidngpb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2onclcuzr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dvjnpsqq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yyeqiuoj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2chbtlgbe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2uprlwwvd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rqwfqfhs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rldwqnwo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2apucesep.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2stpfzfed.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dspgouty.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gmdmatee.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mzdpknhh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ziutjizd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iimppkvc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uilssvfy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qezaciwb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bfhxyvws.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2pnniunfs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ewkltxdz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zeqrizcu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tjantfjh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jnwnfffn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ytgxfoyo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2toocmymy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sabjkwek.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iiwvhytb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjvxaosp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fuuhygsa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wfeougrc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zczczlty.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2snfzcnlc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ypkwmdvl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2whxtynal.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jbojmbzh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2bfcmblrh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qdyuywea.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2muockljv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wkoebdwc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2acjalriz.html


<!-- 参考信息 -->
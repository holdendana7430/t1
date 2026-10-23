代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3soxfzmyx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3gcaoivhv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3cpnojonz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3uqyszwmf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3gvmemgzp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ywruvlpb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3grashfzf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3cbpezowq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3hmxvvlvu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xpzoxvol.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3czfnusnl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3sysdqaue.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3oaxmxrsh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bxdrvair.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3jnlplmed.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mxpyeslh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kxivedqf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3erhrjujc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3kklgfciu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dphwvulw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ebjhtela.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3squgiltf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3iqhrufeb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3hiuehtvy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3gmxfabdu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fhanxivv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3mvhziwft.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3fzillgrr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3xyehaarm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3samxkebx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3kzldpyab.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3kixuqxdr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3fotpkryt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3otecoixl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gntvdsti.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3utppcvwm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3cbaltace.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3eucgagkp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3uuogeklq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3dcfwzeui.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3fnecerzx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3pfpmhwze.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxaukxtp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wlhnrxaq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ainiwlgc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3isgwpghw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3kqiehrzj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bgiprmqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvcytcxn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ryotzqnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdhqjaoq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nrwjzwuz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dzvwqxqm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fyfxtuwc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ojtediub.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3rctodmii.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3myyjxryw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wazjnkom.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3kpnbqsgv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3riiedcpr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zgrxsjsj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3assnzeeh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3bwonvhhd.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vmrfkstn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3onmtjbyy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3waqvqkit.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nlrmlarw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjplrdjt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3soenypub.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3kromilpb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3oaptyjiq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jkimtxzj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gvkipnro.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bkjufgsy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ldecqdbi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qrortufj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwadyuod.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xkqymgeg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ehstzrup.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3klhxrasy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3dzlycnui.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3beitrlug.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sbhuzcsb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bjddzvnn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bzoxdjqg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qtmlisqd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3embryasg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hojgvavb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qhchxkzm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3cocgidum.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lfrmjqgm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3prjkitej.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3qayiqvtz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3wvithliw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ojjvvaox.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lgdbjagr.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3iiaazuxy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bfxatzdh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3urjrswlw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hdaviiuw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jnzpeqin.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qrseggka.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eiyxdpqj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hnhwljmi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eujtldvg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mbcivzlh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xedajluv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3nixrsgly.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mqiveqsb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3apyvaspf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mhgjwtep.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3thicweia.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nqdmnugf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iuuzrpsr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3nagphvya.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ryiupblw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hdaaiiqs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qqgppeui.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ozdszeai.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ypdbcwyv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3klwymple.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bcledbjc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3spszisrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3erdocopd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vtatphmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngyjnfhh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3abqkuqhj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3oneuohih.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3thbnrsqb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wtazepyd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xddtjbhd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3uiacmlyf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3flasvdar.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3iyfwwmkt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3yylnynpc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rhvpqhfr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lybmcrpd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zemwaqas.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dhjvbrqh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3aninvmbs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gyvtacfs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3fyvdysyc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fzyevplp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ergciwyz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rnrkviul.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3pujskypd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3epqqmdob.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cnciotcg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yhbmreyu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3lbzfxknq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ratbklfo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gagqheps.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kylntgnp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3mpcffdci.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bwnfaapk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3upxplbdb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3iuvoaxoj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jyppzjra.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3sivepgfo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tjizauuc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3nqnkqbwm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zzhhkmne.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3swjrnxpf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3srsibfay.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3iupimxsc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ujhdufzg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xmokflly.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3urwjajay.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fxruyvqm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jykklofc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3phagpqmg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3azlyqbnh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gnujnsfe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eteencmf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nshnjock.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dhdyiqas.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nhdyuarv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hwgwqztj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3yrckurus.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3nsgxfjgl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pompxxfk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vrdqgvfu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hvmntmgy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dxdltgeb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pteooxec.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ryurveoi.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3osrmzrlb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zwowctwm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jvnlrzhj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ldndbstf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3cdxvzmib.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3luzeollj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qmrdxady.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yepgcavg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rjdanpao.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3sawbmlpy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3drkiiiom.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wpkmaiwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksigaucr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wujbcaui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhqdtcux.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ucjuwwvt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3fuzxfapw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zljzikxd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kogirbga.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nvvnoqum.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hgystgli.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zgfpinlm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wnbeuqnu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qkcsoapb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qsmzayvi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cuewgtjp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xqryyagv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3aduruxjr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sstgmgke.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3loznvisb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ksecwlae.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rrvmrdjc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hnapwinx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gopcbjqx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kjhdeznh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pqufaslm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sngdddqw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uvxjxsnt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tlveaqwc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3edyluifm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gokyamxh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vneihjsj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3olexkgom.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iklrctyh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pndysqzp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yajpcyxo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iajtpfhf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3uspxyjvk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rfahhqhb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3suxdebws.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3lzqvrtyd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jfnqkrzy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzxxaldg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zngqdbrm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbjzbjyo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zkqggwbi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lyhgvdpu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uwlukroo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3evprukor.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tayynrac.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3cvrlyvzb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ztgafeqa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3idpcqsjp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3neexxwpi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3inqgfwmt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3suupsrpe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vxvzvtas.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fufyjfly.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eviakpha.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gkfivtgw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rxecmfik.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dyamyxip.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tnpkchsc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kykavaxo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3httztjgt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3eklavgww.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ecdtfmru.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3onrmkfys.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ehjoaahd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3tyenqwyp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3oileqdsd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rrfisjul.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3abhrsitc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xobvfhwt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pelcxqtz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xfkzkudd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qotskgdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mamcyxau.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ksfemhub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyuqqrxn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aqwanrax.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3suhadbyo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qrihvhhq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cvipopzb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vvjyxclh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cntbphtf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3adchizhk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3beqfghce.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aupbzhvn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3amsnaxbv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3btbpgbbg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hmfxlzqc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zmmybmsz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3agynlaqu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3unypjplv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rinmrkbi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wimfbcgq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hraevwyw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gwvbihdy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ofryynos.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3youlzenx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dwcvxzzp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tmdseuao.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kdsfwncu.html


<!-- 参考信息 -->
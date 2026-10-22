代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ksptzcka.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2puckesct.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2lprgzzpf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2toudwvsb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xusofllh.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2fzviujsy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ukltszuj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2wwtjwcvt.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2likdczww.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2lcoyxnfy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2xaeybilc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2mgbzpqyd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2rumhapja.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2bnyhdcbh.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2lbxudxas.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ecbkngdq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2mmtlczhl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rrchgrti.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2skfbadcp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zfqnkzhd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ixyexunw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2lxnfcjkz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2baezmprf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ocnyeitv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pjyzhaku.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2hlmmovfl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2mkfdxjfu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2zlyhqzbd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2omizfwws.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2abkhbzns.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2boszukbw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2apkqtcbg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2nsxcqaej.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2wxactlww.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ypvsvnpo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2pgvksxlo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qqvdarzn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pjqxhnew.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2qpmxyizv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2alnwffoq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2uabpcrfb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2mjammumi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2frlzxrqq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2pgdsuycj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzwisjqz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2lfiuqurt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2cbztkqqx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bpvbupya.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zftaqcqz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2gkhcenot.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2opqcwebv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsbpbbqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rspmibia.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vqiocpoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjocugac.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ydpxjrjz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jgnypmyj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gowgbofd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fqgyuemy.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aqmkmmtr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2bdzaetwn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2gcayafsv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2rzsojcxe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jptttflf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2khyejrmy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hokpjdaz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2imbcuvay.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nepltpgo.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xkgbcybm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2squlrtag.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wtssxewp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnffmari.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cdafwacz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qnlsiour.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwybmxi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2siayfati.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rutywsrr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgxpphem.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qfjqdlkn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2qdpvnovp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2kajjhmhl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2okwjnxfv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2jqeejrvm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xfymquqg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2tbobpmod.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ywyzuwof.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2paszctvg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfkhsmc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wlmxqjod.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2sckeqlds.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2znducsrs.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zoojnryi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2edncqvve.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2vlakzmml.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pwssogck.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qhvvagfp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2oilhlspx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2tehcvtgf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2utesbnun.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tpyiywlm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2avkedchb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zkhirvva.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jmwepnxl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nqhxtoge.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2aylejlsr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2aofvjion.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jwvqbisj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ecnasucy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vwpalacp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2jsvnpaha.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sdaxrghf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2sbaifwhu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ddauiuuu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ovayscug.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2crkaykrg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pgwwnlae.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rpzypbcf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vbbasxbw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2arnyxvhv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2atmbtrjr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2fyhjntxw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vhmybuzu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ppowiiwk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fzsufasm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2zdhlhuea.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2trlfljvr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jtyxnnry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrlnkxcg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fslafcaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tterphrg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hvpshwnz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mrxrhfyq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jdiouunv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2itidsiwc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uwcojbsr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2guklptql.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2iqnppkmj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xpeiaaie.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2mbgfkxnh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ydxxgczp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2trudeyod.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fjjejohm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2msdxpfei.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ukhxmjzw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xtjloiry.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wothwppe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2wmrshdkr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jyweqibj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2bnlkifge.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2olqkrxkk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2noqjbqmo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2avkpznjw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ykadyhjw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kamiwmuc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uxkoeyho.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2byyyhzxz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gcdzopmu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2cnvjtyln.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dixfewgq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bxvpxkiy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ixrpracw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2itcngqia.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2uvgvrwzp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2tixveeuk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mbbzzoby.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sllaufdc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ccuhcpgs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bswvgdub.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wqjuylqc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dnqgbamb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fqwanjmc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2eldxiisg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukekxttm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xfqcfjgt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rjnbgnly.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2uursoofi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2akmdfjlq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ujivamed.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lczaqiqi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sjquawwv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cbozgdxl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ukvbftvw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2gsepwjsd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vykyjgfu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jwwnvzwd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2sftgrint.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mmkcugmb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wzdhqjyg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wmgckcsn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vuoyvswj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wcpnebtt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2iauhxygx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qunjtzvh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nqyzxfrm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rcvhwofs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2uaznnipy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gmuqjiqr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yxvwsqtf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lnbomgzm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mfyvxldv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2drvsvcco.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bihignxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyljcwbr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zkwuqpyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evtguvue.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gwngicbo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vagjziyw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zbreeqza.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2owdnpofv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vcmwinjc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2octwmpmn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2awqcpnce.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zmhhtfsj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pbqjlbou.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wcotjvxc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cfjqyayw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pqexnyor.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gspbetow.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lcemzwra.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eqviiteu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sqiabrkl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2erxewabk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lrhimxah.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2gbriioaq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nxuexaec.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jwmnqsvz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ehlyjbtb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ubwwvcum.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rimlejxi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ycyvvenw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zgmemfcg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fbjkgdua.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2btuumbdj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2okscmtmr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2grnahtvs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wpsmlmgq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yjwwdxoq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2osscffcs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kpzncmrn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dqdakcbz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wznreikl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ogffqugl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fvzlmtdv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ivzyzjfg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uqknxlyg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iquigxsb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cglcotvo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rzcfwgtk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfzhpagg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2exwagsgq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lsthenmw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2szvjioiv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lfclsbij.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bofdgmmf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dnstarqv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wvxbccce.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xtycehtg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2icpnivrv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2klvvdibm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2nqiuuwso.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xjvywpwt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ubzimhra.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2poqfcsrn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lpnhhjnk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ntoepmsl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2exskijta.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vabfqxhz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ryuuemza.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uagbrhsm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hiikwfqr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2maadicgn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rsytcdos.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wczjmkzs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mwghmznr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rrsljaab.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nckkwhns.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bhezzbdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zacrlxwu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oslorouo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqkkplqr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nvdcploy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkutcta.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zhblqane.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2scjaablf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2akncdiwo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xkiznhet.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qwlpbqxm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zhhjposw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2snznkucl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sjhwmxrd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2abnpqrvs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kdviowyp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lkgftgcy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eiqyrmqe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pjekmtmp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ifqzeujc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dcqhvbko.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2bfvmkbyn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2slxjqdjs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2lvkwbcxk.html


<!-- 参考信息 -->
代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqramlr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2qiyfsfrt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fwkakgxj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ykxcuxct.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qpoahubg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mpexotrc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2capgqizi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2isoaphcc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ikjgrfuz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2vlbflpor.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2omvasmxp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2znbwgtck.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2hffrrubl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2woqwpegd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2gwsiflzb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2upokmnxb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kzazzomo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2sowsqcpw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2dpcvivdy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tnwkdpnn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jlianiar.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2pyvsaoie.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2swotjegd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2bpgmpxgq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2dzijsrkh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2bdxunpjw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2vlidmbwn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2dvrhltku.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2prineviw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2fiyiodlm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2gujxnbqr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2eqclcrny.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2rjapnyqb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2bzkiesdr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jfakcwmy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2jifxdcgh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2hfnxwcyt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2qboitsnl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2vnljmrof.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2tnumcljy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2xxjtanmg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2scnniyrz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrtsxdne.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nqnvcqkx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2awkqyqsq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2nmecgjws.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2qaduxlov.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dlfshaki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thupbped.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2skgphoay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrbiucxy.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2jlbdhxdq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yyngjwrx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tymzdekh.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2znmkbxuh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfaniflz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ovvksdjc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhjqfwm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2kzfablpd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2pkxuztqt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2obyjlyrb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2pejvzjgc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2crklimia.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gkufikwk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gpnqjdwr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yhwingpd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mtuxhvca.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2efbqlwnx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2krhjpfcb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2lyxmjlrf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2nscuvtap.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lneylbme.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2pgxhvwtx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yfptandb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sjxkqijx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2iffnezce.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2jvjosfsg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2emdjdyhg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2bhqnjqat.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2equzhbaa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2krfxyqcu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wesqgivr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2upqkchye.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lzhqiivb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zhnvrahn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gagqomvc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gkevrutr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ejjvfzjq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhytmzv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zabtfwsb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hmymoqck.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tgthstmr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tnrqpigx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2amnxdjzk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kbgyeklr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2esdhpvbl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2crfnrkjk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xunxonqx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xphxnudq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fqslrgqq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cimkkdnx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gntrlcnx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2falldmcu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cchqawkt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gdvoikzv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vatjtexy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zowrqmud.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2giqxurha.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2okaokxtu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rrufybhn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gzeihjey.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2welsualm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2sthemcgk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kvghbzra.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2yinhsoyc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kpvckkss.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2yweopkcj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2czblbwsx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2krcvalte.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2yxwvmplv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2oatnfegj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bnruqlbz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2yknwvaxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oinjwakl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2sordgtmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrnidsho.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bauivpuc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2zrmqcfqi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zgftyxhx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2buchdwpu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2exlsubcy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2msnianuz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rqxddork.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2wbgjwnzs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbwsgbm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2srswivcb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2geyuhplv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xtrgswiv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tcbmblwp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lnaovanm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dpnjmnsh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wztfhfws.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2vrtjjwxt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqjbtbmc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2wvtfhtnl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rttpmejw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2czlwudda.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cnkajxgt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2onnwnhvw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2sofvnxvu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vkximzht.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2szexiyfe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rlszdume.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2lxnxkuvo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tezuxoip.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ugowtuua.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2szzubedn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2klilpift.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jgmalxsz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2alzwwrfq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wpfmmwiy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2aqjfjkrf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2aflijnbh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2thblfffw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2nqudfbea.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dxfjzwxx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kdgocuof.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jsznsdyx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2keccypoy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zzkfhorz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2loczmqxv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2aifpcoir.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lnpbihkm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2crrkeyvk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vtjvcpnm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qzvudact.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2efriowrz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wcnbqwty.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2myshbpso.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2frzfsqjq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jphsfzrh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2iylhdolr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qeptoqak.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bfqtumlu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jsvabczw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2aayycbyr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2swwmpxcu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zxbmgdlg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lvqlobzz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zldroowz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2eobxstrh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2juykungf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dnehtdtq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sdpdawbw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2sfveefzt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fvhfvtwo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjtqvlk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fcopjyms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzehdxwy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gpdhguwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qapbntfc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2drscawkk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hkigiugg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zcxyulvz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2afsrhwqm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2adyasclz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pmkastyk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jfhmbjeq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fegqvkci.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2adpkzzaz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2riwrfqxl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zqnsawey.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sgoohvgv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kflagkvv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2oxpbyofc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jvxgiurc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pnklvorz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zseknwpi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yunuojqc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yuinoerx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vgmzorqu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pyqjajua.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hnjymxlv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xrcpuudw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nrjkpekc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2srphipcg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2btnwzrcs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ozjrrwgw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wtrrutpf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sjtwgddy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fxmzrouh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ztmtakov.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rujagftd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hfvowkwz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jzaztoch.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mvqsrpea.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2gkcgdffk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zblaiamg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzxilqdm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ipgszywr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2thxcgbzg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dmszumty.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cijtpzvg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kbyezqzc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2efbwffsg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tgnmfaqj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mwzmwbwf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ihzrbpty.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ywbsfnku.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zitstszw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zfyfdlob.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zgznlrdt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hlahwrgb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hcgkycvl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2iiiktjdl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2oipnxanb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rhddrocb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hssbfoye.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2immwszge.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mpnjpjir.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gdrsotdq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xrevzlfi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ejemkfye.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2woumbqad.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vkbrunyv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2peeqvhxk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fylrrtkx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pyicdjck.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hmektdvf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wdkrsdnr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2eikkhvtn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bzporfui.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2aulpssvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghitldrp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zuxebdmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trnbkesc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xzwzclqc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kczdkwqn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xkrqilvz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ialsedor.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lhntitht.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wacfoqlh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hbcbebyp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rrgytdsb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbiixnfu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2poxhhndc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2obmimawh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vhuvvimp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ggnziovq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqoclwwr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cprgchny.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lgczewiu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2brfhvksg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ckxotuet.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rplqyvhg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2hskzgtsd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ocxojzwo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uceaykma.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2epbaoewi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2clixcpwh.html


<!-- 参考信息 -->
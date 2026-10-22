代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2eqewzhmn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2flfquvoc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2muziafyk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bgnwcuox.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2oabjlfuk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2irupduvi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hfknlbqd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2blnofass.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2cylixkdl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2fqhjbffd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2wjzqdtrz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2dtleszsf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2hzjysuoz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2dwhorrvl.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2wmpdnonx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2hbsfvedx.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2dhjyxwcl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wqldwbwi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2buyfqtpa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2btzfdqjm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2marwpayd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2mdjhaobj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jaqblegf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ybgcwyln.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2usauoyxp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2jtdnwspv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2dqnsjqhr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ypamhbdr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2jkxeewgs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2lvyrbdzh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2nsvzbgqy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2dfvmdzrh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2rexzxnfr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2zfsqoblr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2vsvdprnq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2efeghfvc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2pejwjslt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ovdvgxeg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jodraqbv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2grudjtxk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2luhcdojd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2vqyklsga.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2iuecvvtj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2aprudbhu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2npxrsnwr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2atlvrgbj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ethoqmnv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vcmromac.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hejqymrj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2hgtgvjgj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2simzxwue.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qkbuzmhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asxegqkl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2fagqbdqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llgahgpu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eqcamuby.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cjopkloq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ydkvgifj.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ebcgyiol.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2efxrllpj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2spmuowtc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2xwnaddpu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ffronciz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2shbzmnqb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2otzewzik.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lykahouu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2oqswpmut.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jicgtzaa.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtdvklhm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tmfjrbad.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vqwodpiz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lguedpaa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2pkcgxwuz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2krgelzbe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2aqidwkyz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2urskgxlk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bxsvwjgi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xlmioanm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qprnoake.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2vapjjose.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2uxdybpfc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2vsbcnkil.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxjqloha.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2chirznlq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qpcwjrof.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tnbxmfof.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gotaarpz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nsyvleze.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dhwfjcvd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kkwzmyhb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ilwzxloj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2qnylidgb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2qoogwwgs.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2klcoyjmv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nksjpblv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zuqutyhz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2cowvwems.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2sqlijgty.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mjdhtpxd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ukemmehb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2kwwnurrm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xbevzopx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2swtflgje.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nlxrnszk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2smpjwcyr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2aomrlcyk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2umsrtxnj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rujjvthe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ghrkvzjw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2fxnyqifj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vpwhlrzx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qusekibh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qbxggpgl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xiocqlwe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2owcknonb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qiezuzoo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hfhcgvqc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gxabqxrs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2nvyugyff.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wpubzcxr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iyymjzxq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qaozdojs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ujafkjdi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2gpjyshnh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2fgjoiuuj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2secyodqo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2iaiopkad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dajottuz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2nwjsjvkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onplqzym.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2brcwbzwn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rjuyrplb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2kmcwncxn.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vzalwboi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ljmvamwm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vjcxqdnr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tclfwxfz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2fuuebdyf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kpgsafiy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2snfawjjc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zhzflpdy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2iqtsldgx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dhwxzfrf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2addszogn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yiotzcsg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2icmudhim.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2bgcfydeq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ikxwseoz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2wkrhcbbi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mrrhoqeq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2glmlbjnm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uydjdehx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2abzqxfzs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2azhbaapp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2akmflukl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2jyiftlsa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dkpjcevx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bvfybigs.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2canlbevj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jgnmoust.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2eltsdexk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2psjqwpgq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dwhodexo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2igcsfhis.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2dccvraqq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2akmanrvv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ebotgfkj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2rsdtaokw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bseqshvx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2efeeuzax.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2syjeigvb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vdfkwjnb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2lgxvahkm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2fxanbvmr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tripzbfv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dpoodmhs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vykvgvxr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jqxnnddl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2amngouqb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nllfvzru.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xxvteanh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zchihvdn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gqlksyhf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nkrjkser.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vvjmmuyj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kozsfbpd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hhwesxpk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kwpqsjpw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dadgliwi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ytuzfqyd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qvesuizw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zkqjtllt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2urxyveik.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2idgjszqy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2adsafgcm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2owvlwwja.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2muqqbhhr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xiceedkr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kcbczgyh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zlflzing.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jocpazrr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qggoqoth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhsvmqxf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qfojtvzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvopmofv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yuqobzsx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dsovtjsv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2okdxfgqz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzmjawe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uglsqyjb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lbpukqqm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2htpeshgm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xajeqotm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pevkbtov.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rjwafslu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wvkpytzm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cgjoqvjj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fixzewuf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uugcfbgg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rulzsjdq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2icznrymo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nyymadwp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mbjxbqhy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kccilicn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dksbhkve.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2nifbglej.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xsoikjfs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vpxccbzt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2uyjwaukh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2zvtbfbzn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ozneoaow.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ncafocgk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vdrycqlf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dzewxdwx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fdhxdulv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kvywtyha.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uuhrzveq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2urtcojcv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jivlzkbk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bdmrmqqf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cbscmufg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zznosmtl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2igxfxelz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tyeqnuph.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ogtrynnn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmyigdfn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lpiygzez.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lldmweyh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ibafssbg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2imnolshl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zfslykys.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fakzqxkk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2unxtefbq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cwphkrxl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qvfhatkt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oqpglclx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yzmwvaou.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jgxgreor.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2spuzwhka.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2evcjzkwc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pfrckajp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mgngourc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dungjiro.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wgvfjoti.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rysbtdfx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ymdpbekx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vcfjruje.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bqhrpcag.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kqysbedn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2butiqqdu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mzztdged.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bnyvmfcs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mqrmpdcx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2gwtmngqx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nhcfhvhz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ksdlqpom.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2scycsvkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zptybbkl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hgyrxljz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2soitjltb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jvkdfkbc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nbfegxgj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vupcojiu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ymajndic.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wlcynlmq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2adqxrsnf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sddvhfkz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hrepeyny.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjrhmuff.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2iestrymm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2slsuhjcq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2stapyfym.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2upmhbhkh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nefijkfd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qunfskor.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijymweme.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2upwlfgrj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rsvjdwkc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kgirhxhk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tpiccpgh.html


<!-- 参考信息 -->
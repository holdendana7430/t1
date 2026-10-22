代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2zsfvtaft.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2eleltdhy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wkmssvji.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2oopzhdqz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dattbdgw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2svdqeura.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2vwstbbbj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2rrjlaymq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2sfoquzjt.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2gamythjp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ittqsqnx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2zpxwhfmt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vjxukuvx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ojtlsvzy.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2knpeddcz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wzdbvwqr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2qkffglcj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ptdzragx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gwcnmduj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vqnpwiwy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fuphmizo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2hefuibat.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwjifuli.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vbxnfgzb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jogveglw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2swtmovaf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2cpjtwhuq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2hupmkyrd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qwlzgozp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2habsdswq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ylmprcyi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2lubauiyg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2gifwxrpw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2xrdrgbuq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2agmrclaz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2wgphvoce.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ebfpihqr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2emuxpago.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ptofhcgz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2asorhdwd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ppldsnxx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2mbqqglfs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2uxdraenq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2mqaqiitj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhacpkiy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2batfrfri.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ivseawwx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2phbyszqr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gudfdctz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2lunklfau.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2fhntozjh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gltvnlbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdtejxqv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2vbomrygc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2priseaqq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2krbqgiur.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2snlkzoga.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hkrunlkm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vkbgabio.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2boqrnalf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mcdgvidu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2woltdwxr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2gcjcflos.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2mnhlqwpt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2nqokihjz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2gkzdxgat.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2vmctvmcj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kbhissgc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akxauvyr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jfgirmwg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2hyljfdsh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2znnlhhxy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2qpulllcq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2purzlxrs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mrepbjtb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cchlgjdy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkcvzqf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2uifrkmxi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2sinijppk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2dxiemxoq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sieguslr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2phylkckr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ilzljtuj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qrchsqze.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2omeciksa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lhucctqc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lglphvlc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hivwgwuq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2erazvzbf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yjezlblm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2bnlvaien.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2jcthugez.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vogigvqd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ucsvptip.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uzoaysfv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mjkdsrba.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2haegqoev.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2hctwhmrc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xicbgqvo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nddjvtif.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rcagaemx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ztjmhyup.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xtrziboi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dnktszqp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vkpwfdxr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2niamqrws.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dglennxx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qorygijw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ydfvafrj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nfmjbant.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ncakljzy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2naoinnvh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iiwgoiqt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hmhjiyhm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2reyaonym.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ukuwuvan.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2yeyjsqpf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jhojvgek.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2vkkyfrxd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2gjkbunix.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bltwlaqf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mdqbhlyl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ikribxsb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2viqvdfjr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mujdfhll.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vbtzqqjt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ykqblnqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afqqfubq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2tosmsgdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgfinbtp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2xhqfpakj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2kwiedzge.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jlhltduv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2glkbtrrr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dvwdsdmv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2hcswinxz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lrojjmpk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2acmvmvmw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zaafjccf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hfqrzqgh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hyrcyqeo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2yjtevmrv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sggdwrqp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gsnugdam.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bzthwnnz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bmefyylb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2rqfvxljk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wtuehiym.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2tzjrhujl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hodpsdcd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gzxpbxla.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hzpeirnx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yrbfprvx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qvddeggs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mwkmmoqu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fgwcqliv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jwgidqrk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2dtngimji.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wslrqfaf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gswaeixj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pxpeymuz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rcbchwac.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2buovbvcl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2kdmflgbm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2kecaeadz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2chxygmjv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ywpgdcdz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vkjlvcwt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zdwenxvy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tyzjqhtc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2awadsrzp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vchabwjl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2adhqslyu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xrdlnnee.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cayycjfg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lnelbcym.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qrcuwcza.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2klywdgja.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2smipmsxf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cnqtqpog.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nkotxovg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2cxkxhrla.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zcqnxiel.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2koxtpllb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ztasvdtl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gcgwuwdn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2taxvcrbx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dfuzdknj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uksepnjl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jfzxkawt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fwujskvm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yvbiaigz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xlebjrxj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mmhntkgc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fqliaipq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2cdzgewvv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mnxnepnq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nwzfdvcy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kxldzbkz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bypcjhry.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jdomqnrw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hnyzyxge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecrwqtvn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wlaqorqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrzajqtp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fdejfjpw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qgajfnav.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zwyzllpq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2avwvicwx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrnyvpfd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2opbvtfzg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ozcvbqwi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lpftpshv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qqwsvtny.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jevzipgm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2brluejvm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yfeifvam.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tvvxhpij.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2slgdrkvo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2prbjgdax.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2agzcqdav.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2skyhtuwm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eqouoqja.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2gbgfztjx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tcysncih.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zxqjmwpl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vvufskgm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bnzpylfy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kwnpyiip.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rmthzeum.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jtwxwmnp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qunbaxfb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gfapdtcw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sduwrugp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rfgqmgsr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fjkdlbdm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bmtlzdoj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jldktmsr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zbeuwhvt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2trgfdpwa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2msozgcye.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wdwbadcg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sivrnvtc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2anvxwinb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrpfxtup.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfyjxwqq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ompunkgv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ottyyoke.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zdermwbl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2parsppgx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zlsosvvu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zpdrccft.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2msmejuld.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fdavodhp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2adzqkxgk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jtzjiqvk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wouaugah.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2uywftmoe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yigaxvvt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fdyzsbfm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pmwgaxio.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cyjwqhob.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2npmliunh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2syenddko.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cawbutuj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vigevzzn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qhhjvfbu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vxlyrjvm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mpqjxeex.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zvaohjui.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2weahukjs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oghawcbb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rztybkhi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kbmdokit.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qcolspcm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ghyqttwp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2eiquuiew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmiocnhs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2yksfbpxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpoftuos.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2goxoyqix.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2myfbtqah.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2thdftkol.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yzeqnkpn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jpofagve.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rtopnbhv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pdwhgvwi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nzdrvauw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2skaqiswu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2cgxltmda.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gteifauz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rflfdoee.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jxbxuztw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xmjxxets.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mlgqpxmj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dycnmoyr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jhrokgmx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tuyagxht.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2hbqdmulx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ifgtxqlw.html


<!-- 参考信息 -->
代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lmppzuis.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2qaazjjxm.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ecekadwm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2exoccsav.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2yijnqrdr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yzcsnrhl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2dxrytoog.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jnjtecol.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ikdewsys.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2umuhdcfc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2qqrgqeip.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jnyserkh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2spionatr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xfhhciqv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2khgpiisn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2hpinvxif.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2dgcrnqmm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2nvchaqtk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2curjgawc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2sqdcezpm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2hmftretp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2snoybpon.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2znxqszce.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2tzvbswln.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2tagiupbd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2bjawzzgv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mikfhlui.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2dxnpiggw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxtgdlz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2zdosiduv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2txumjujp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2xpkkbbwp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2unekrnkf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2fkqbzlfo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2izcmnzvd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmshdzl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2tztmeldv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2enwfxsav.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2spfmddzl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2usiezioa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etwcmyjs.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2phdqwofa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjwmomgs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2axhfnjdv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gnqldbnu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2aagqbvpw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pycprvik.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gewjdrlq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2llnecmzm.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bksdvfci.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2rlvonlfj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rqjxufuv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2peyphpjh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cylmhska.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kasukrji.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mvzfbejm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zdxqehtq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2coaqfziw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rkxeabjb.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qoprgdvx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2juwnjyah.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2kjksmobj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nhgaqofv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ihkwqesa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttpqxlnq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wvibtngr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2muabkiyo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2kqhonzvz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2eljbndmq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ptbbupzz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzftinie.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sojmsozk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2qebpadux.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ukiqbmok.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gsofthhp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vqkmvhui.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dfkpqanf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wnajqrap.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2sxbafuaz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ddyevmee.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmoqamkx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ytuaqtjk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nqfeyegg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2klpbddzb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vgdoubho.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2xlljtjgp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2imwgiahw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ncbnqiwj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2xsykqesb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cngvsdfd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2dmyodxfw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wfdqpaip.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mgjwkozk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2wbdoggbt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bshurize.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2enudppbj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rgkgepif.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ywaxldoj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fabrnvzt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2xzlmonid.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hqkvgjnw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2surzteyn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mdvwduou.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jwvfalqg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2agfpiwon.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mmxrycfu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fdkvlfhy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xlzftksn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xzslryhi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oetjwcqg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jkiidhfv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wmddfoqz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2jjsgenao.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mmftslpu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mkdtmpxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rossdsrq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2dazvyctm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntgwalxa.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2lfocyjjw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2erbodqnk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2rxlnwpqa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2iedmaade.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2djqofqtz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2rtacjbms.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rcfthltl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2asimzlwo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2nrlpnhha.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2eirtgewi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ithcpayt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2dmkglxlm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2aauuglob.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ibckbyer.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gxdyraxb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2pggffzkj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2egpjwngq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2klwfrvnc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2tinurmzk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2cyvnydaz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2qsjisabe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rvuwuzmy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ygorwzes.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2gizntwch.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2stqsgrmy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zmsdlqkx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2seyhaqqa.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2pggjxxxy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2algaccmh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tdlkopxv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vnysszvd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gmjkeydr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2fkonifjx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2vpgotwze.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2kqhmhsum.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2olclemhj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2zzcaadvj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2mfggzzoa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2kwoiuilz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2extxetas.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lguswdar.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xmkyadjd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwfztgzx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2lbxcjmoa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2neztfupe.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qfuwjefl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ccuworsj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uazrdbgd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hlvilhbe.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2piskokdk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ppkhfobn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2arjizaug.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ptlvpgfp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nyjnijgx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hqjdguik.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hydbsipf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rxiujxmz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ocrnpqpa.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hpiiqsxi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xfwiatpw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tundnnza.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2tkechmcn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ecvnnadt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pmgfmafs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pgignwwx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ipqgdtsa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ejmztvqv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2htamhrwb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2korokhtf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mdyplirm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wiumyrdn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2prschulc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srhnxgdz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2tiqptbkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgdcoxno.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xhhhynjh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jjjqygae.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pdsuaygz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ysefaaql.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vstwsuhc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2thxgxzzs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pjdwwllf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tzavngdq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gvowwmrs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ghvrjgkc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zkdmazee.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wjkuulrp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2foqornhp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xynsulmc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sinanjfu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2poogjjej.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2cyujaegr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wjtpftnq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tizkuvki.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2khwktmfs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zlvrbboi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qxjwuish.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xvyqnemn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dabpgkdd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2crvmmoxu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2afgnqjdy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2emmrrenf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jiqbmdwz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zbouozrj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sbwdshbr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oweikxrz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hwhjnpwo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pumajszn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ixitrnbu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2obhuouqu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2oxmwgfyh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tohhoakm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fkjzcjzg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kkohuiyz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yrexpylo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2afkxtism.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2octbiiim.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hellaljs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nzxjvbry.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nwqhdbwz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2iugbarnb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ixatyvnr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vnvecufw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xwyvoxyz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rftiupjo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fwvteqjx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2jsjdnhgk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2trfhxlxd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ywoeapdb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ugiqywlq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gmetjdlz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kjzkgihl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2exvvuluo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2susojoup.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2stpmyphi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2dtvtvtyk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hipjxfkp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2swpgcplo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jueklirt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ubevrheo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2atkrazmq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xyqronhj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lbpvwobz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2eugfabbh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nfunnxtb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2acrzpunc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2plzzoead.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kywgpxdm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2sutlajwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjnmkrny.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2msgbyhql.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xdjdekgi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2plslhryc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kbxrxnoj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rxadpehb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pruucddg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qdjtxjhx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mzfwtbjq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2viicmjjg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yagbachr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sqjswnms.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eqpmidpb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cckgxtpw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qsrguwzf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xokzvrgi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ywyohiov.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2njxjgfdp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mxednyyt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fhhtsfyn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2paxfhvqv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qrfwaxrq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2serqxirx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nanyfcmi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wngcioky.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2phvqmqqj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2faqtsdzi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2aqfflcvi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wxufjqxg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrqvwkcd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfbfsobp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ieesthpo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2omhldpyj.html


<!-- 参考信息 -->
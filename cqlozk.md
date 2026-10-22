代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rmuphnvo.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2wmpvrwow.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wwiywgki.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2mkgmvdai.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fwmxicuh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2frbzfwoh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2sjwqtjmb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2fkbeqvng.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2qxnqmjgc.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2cghhzzua.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2adaqzksh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2dfzadszl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2tuuuwduw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2blywtqua.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ueombigs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zqvstkpn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bifcvedb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2rysrhgdu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2dqfbkgsq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2geehdgkt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gsgibqgc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ldlrzqyi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uaxzzjjc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2abjvfjvy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ymeqifxf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2uqcpgcvu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2rfepddge.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2zwtbzkzj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2dykjeijq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2sojkmtxq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2hwvxdovt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2meoebzfg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2qjphxsbm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2cfofywap.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2yvigmsta.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2taoqdmoc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqdghvr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2gtemujlg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ybuqmchq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2dwuydzvy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2kzldndqf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ahhffvtk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrspywyz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ocgxabcm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2isfnibpc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2oxlcjcvo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ztgrzeoj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqfbkmnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euqdnjfu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2looxhvna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jblgthhv.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yvqzwvqe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2kqinpsmk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ntlhdjoy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nitzxgyv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uumeipyt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2gtpojihy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2wnwdheha.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2hyfkbnep.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ujpbbqlz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2osajdgub.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pgatznjq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2nfjdmajb.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2olmabiuy.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lpjqrkex.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yoytwxpn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wljroxin.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rjjhzbfs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xukygosx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2knirqmtf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tpaqzhhk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2aumteruw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfebaiw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tafqhrxg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bwomcpcp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ebwjvatq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2bxdsfalt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2vmksvwme.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2exuhcvcx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2fsmziamk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2nyafvvup.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zrwbosrq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2mbhvaqtv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2znmbcwin.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2piaeoaym.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fenagsjq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2limxqbvw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2sigxzcru.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfutkjn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2btrzofzj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mdwntkbz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2irkwaxvx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2dnovefla.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2niwxqgnr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zbqvktot.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2qzzlgqck.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2nnseezjp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qsrvyfzl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2bvsduxix.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cptyeahp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ozfwhsgl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kcazsxim.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jtqsznoo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qckghkzd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aizojnjv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cefwthkq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2irhvzjwm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2tuwsynvv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nshwjfje.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zoqzqxqx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qyovhqsp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vqiygolt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mndevcln.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lahblsny.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jppqzqrl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2absvnicj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jlllqdwo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fyupvvqv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2evgbnzuu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jwmysifj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gbuiagth.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2exlciqbm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ltfzafae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijcivnld.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ykaiqrhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwlbqpzh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2kguyzuac.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2faaaolwj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wsnourhk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fvqivvqp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2frefyhiv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pdtnlpxr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pyyicysx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2asijxnme.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2oxsqaxht.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gpxntcef.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2fkpthwvd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mqjodkqr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2khxvjifz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gcmulzbj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yzotbpyy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ravfnakj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2zuyuhddd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qgxaihfh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2swplbwct.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qeaxdvdy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2syvgcjwu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2riwqovck.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fvkedgqn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2itwkoizv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iytxocbk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tznnhhmu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2raoikxia.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ffqoxbkd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hlpudyqd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2bbdpqwhy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mkvjrzpq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gtwkrcev.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dedzbutv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lixpwmax.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2iqienoih.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2doivunrq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2yvbiilik.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hglvvxiv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2usxaabba.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xdjpxdfn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xoziysry.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qcsdphsp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kxzmaink.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2zoysgehg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gqpnmfxp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zvquomve.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zwaenkfo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xoxplqvo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rrvaxwja.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jnslozqz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zgyttgwy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2julhhaqc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rugluwek.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yakmafbr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fnpzdjet.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kqvutoqt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ttfhxxxy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xqouhebp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yorjdydq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zjsyaaem.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ktptetdy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yfflnidf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rxfnnxzz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ykggkvax.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2tgcgwnls.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nlgpwwcj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2djlqgapi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ljxggnyo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tvzqqcei.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zuamdbbb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tltgxgiu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bofbqfga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrdoyqpw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2poctkyaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtarjeag.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qzfzsjfo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pnlhajtc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bqetjsjt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uicecgvc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kqepxibs.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2myxiebov.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wxjnuxme.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gmrbpcuf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ricrvqfi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ruerntad.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rxynxlfa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kyjuejvq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xvhmusmt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cpiqtpbm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yutxvbvb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tojdpptp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dwzaufhi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yluvlggi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2umizmnbt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2haioseaj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2udliykze.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dyskxvnx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lqsqoacp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kaasoyfw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mkvsekev.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hgshvttj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mwuqcnxi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gfogchrq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ymmqcdci.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xskgafpq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sbkufcne.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2aevzlqlk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hufdjxmu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tpjxggma.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tfndndjx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ojfmkxkz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pshhdyql.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vvkvvyps.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eciohodo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2odmuccau.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2opargtsy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2toaldohg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kbljrfpy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wwwwtvdp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dbnsbbns.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2whzcytwf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ccaiiaae.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rrkcoptk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vdgnzhnd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yejjywum.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2idsdeddi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zqaoqjnm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2vpqcdcvq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qltogete.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qttraxbb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lkzfuasq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qfmxxpgm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lakabwec.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dalbingj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qtdhtrld.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2navwzekj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vkfypszj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qmzrbext.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2knlekszs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2niznxrpw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2swqphhio.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2egguufsv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lublbsnh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ohjrrujd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vqtwsjfp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2cnyytgqn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nvwnqwdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klmaeblb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2akwvtwbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovtjovdq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ztvjzswg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gzapvsmk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dkzqawtr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fmphhlpf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qmrdudaf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sonicfbg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2begmsofb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lznsvvao.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2omczpwfw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ivrryacl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zyvkanry.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kmfegxcg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gyybcpxq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tubnxcld.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ejekdzkv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibzefpdy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qobkdwlo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2pmblypwk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wjzglcda.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2msqvyonn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zaxxhsvy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ckarpigy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vvrrhiph.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vlaolxgo.html


<!-- 参考信息 -->
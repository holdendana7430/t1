代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yjoyhews.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3dcyvoquy.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3lwkfqoxy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3zhtzcttw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3hplpkzsx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ayqtwqft.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rpyfawrv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nqkbsjes.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3mxqaklxz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3fphltalg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ooiyjrjb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ufachruk.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ivggmfyr.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ceerkqia.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3huwfaffc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3yjbrvryr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mgtksfwt.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3mgfgybzo.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3yawtdeli.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3wcpcnchn.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3xxtrumiy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ldtswvtm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3mqleuhmk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yyzkjbvu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3gthhxnti.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3omnjydvc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3fhlsvefv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vtrczwxp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nhgjbtso.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zsptcluu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3pbzvyxpy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jppwzykz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3poirsumq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3digvonnb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3biwexbkq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3pidxoyhp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3knzxcouv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3forutdbd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3isqywgxu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3jbbnbfaz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3cojrjadn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wwcaxdeo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qkmejjca.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3hahbjmzz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3dnncncdx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3bwvpgzuf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3nfiufxln.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3nauvmton.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3hceqmqht.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ommocvbo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3knmwhhkz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iaqcqspe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3kpfjpxgm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3dcsdeoec.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3auqzbnvk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wkqibjgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbbtsclx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jmsrbgxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfmafywa.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3isfgxxwn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pezbasrm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3eeobdogn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjhusmbl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qalmpsry.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ixcrtzln.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3okfyihsl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3kartpemz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3yjyjncfp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jyngpcwa.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3emedtbqu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ijxdyizw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lmayuznj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xznnnyet.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ekabsxxl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3whimkuph.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qacuoksl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ezlmvamk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3mjwabnph.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3oxmwugcg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hzskcshq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rqfosiat.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lapboqpp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcevtzcd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3dpuwjakg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gmpjoray.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3luydducr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rampzfas.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3vjpyhgqi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qardbbpr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qodzifjw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jcqvszdc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vcdtpkiw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3repeyyqb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xlupskyd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mdzjnmyj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3bgznrias.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wbezgphm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bdwtdabl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ywyyuhlc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3adsrgbak.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3qyazpfbd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xdholmpo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dkpkmvzf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3uklukowg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3sdtullxi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cwuuasjn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qafepsgj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jukhmkyh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fwywgizt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sbkqgssl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3liyssuam.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3unkurhps.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3spmibvzy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kjvsxnuw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hylehhgd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3evfnyqpd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xyvyskjp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cwkczbpp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ufrmbpuz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dsjgjuqk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gbkuwmlx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wsklrlux.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3myuxpuhh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bsylkoil.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3dydghlyt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fplfakzz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xunmgbic.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3kdhisttq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xsflstqx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3tteoeqyf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3evzorouj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bobxwllm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3gmxwywvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsrizyln.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3osgbmaqw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ebeeubmq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cschdvci.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iavycdwz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ifqhrgij.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bbmtzxwy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ryiwabns.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3agkxrtic.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nihoyykz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eurrqsyz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3evhnoolv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3olwhfhfa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fntppiau.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3thqnmvgg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jyuujrci.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3uuobmmyp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lnkazyog.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gkosroxt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mlbnjuan.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vywduhgk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdyiohio.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ddhjqjyj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3epakmrlk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3byaesypx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3veghlsqt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bulengea.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lcsgshxj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3olbeagfj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3gtmvdlgd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jgcbosrx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ohgwdwfv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tzmjhkzg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3msjddpiv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3kibblldc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3vuwowgdr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dvrxkgyc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zhdxrkjj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3imjnifbl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3axmwmvlj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zrsrnxzy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3umlgugah.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3eekwnsft.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gqnjkqqa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3kqmvlwfn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3neopdrzl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ruwrixlb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3luugklmz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hfpevomm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wacplkns.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yenoyqch.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fjgaxxne.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ksvqobvj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rvfdnibz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3osmfylsh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3inxdpgkt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ejlgofug.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vtaumqhz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cjmxvkbl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3isgkiltw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uyxtgjgg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hcslzjxv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tijhsdxl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rshlhsqp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pubjryak.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mrhkdkid.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3lpztvckr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cekinpyu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lbvmktlz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bnciaxkk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3drlmysrl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3syqudnah.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jdsqnxgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skxlpwmv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jvpikwld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwcyutgi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3myxyppxz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pivzgjtb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vazmsvmb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvnxengu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjdzamde.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qkjrlyad.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kwmyigyb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xnjncoyf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lpccmvyl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gmdhphbf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tlfeelcu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zhwsuhpx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oammyclw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kdlvfzfk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ehetjfah.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3urjciiqf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rvqbiswi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fqgalvhw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rtjvofwi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qxwderyg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3culadkuf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oxddtsas.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nonodizd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kobwdjek.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3duxzinab.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3megycbxo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hlwglfag.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ijproerd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wzlnkemt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gmeearog.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3maqhmnke.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uocmrkhg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vmzcfqwp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bskvflyq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3oaxiqino.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vxnwmfug.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wlomdkrr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ttezhcmz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3aqigagtm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rmbseywt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqnmkeyi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ompjwazj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zfshbrem.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fgfeahog.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3avwtikax.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vvlbnurh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pyxfxfhb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cllejpik.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qrchhpwv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qkbxgrat.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3vsxbrhtl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vikwhddv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qpfwmpxm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cfxchvsu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3flvrjzvv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nypdcszc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3whvlpsfa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3godcftat.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wdmcappp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vdawdbzg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3gxhxsuis.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nsawxkoh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3iydlglec.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3immmmygy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3maohbrfg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gjafbctq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3odspbkig.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3whxfqasw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wgcuiban.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wwrvihfu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dpjxfxbs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3nchjdspj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htsbjklr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bsahgwoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhgjnvjf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nwydamnd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hnzjgphz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kqztqeyl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3acojslpa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mfuqhpfe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvjyebnz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ccrkbdgy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tchlzxdz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lxjynkiu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ktenytgh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fbaeimpq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bqbaudnh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zwxgwukx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqsfljin.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fsustxzi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwzlkftj.html


<!-- 参考信息 -->
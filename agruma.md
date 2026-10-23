代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ulxpnwnt.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ksblgbrr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ajjtjzlu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3oyrocbwd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3tzudjtkw.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3hlcjluzx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3iiobwgoo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3apavrjvp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ucikpwvl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rvuzosug.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3eryaymso.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yrxuybtd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jjxwxvhh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3fiubucdz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtxnkxjg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zecbddix.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xdktfvox.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3jlxzbubs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3byqqqezz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3kzoqbylm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3cpphtjuu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3vvfogvhe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3fbwixdxs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3uuhxhpbe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3vchhdiyy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3uterrqib.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3afubjqjt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ssszieyc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3hzqmcayk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ytoiqvwt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tncmkpfu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3fhapipep.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3xvyjgvvm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3mzrrcydd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3rgwybnbq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3rygiqrob.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwspioo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rcysxedn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3evfvaknr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xlghaezd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3zrnqmekn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3jvvkrlex.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3eenttlsy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3pqbjrzdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvijeduh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vqkdoltf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pacgxngj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qtbvylrv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3byaxuerr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3sdiiqckd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3iqhccchb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3putrgzct.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3gteociaw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ldpeczrx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3kmydnwhk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3xacednay.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3stjfgwcy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zunqwvhb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3woojqlxe.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nwxkjwyb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ggcblcmi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jgqxoseb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3azrjgbfh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wxjboxvw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3qvbdlknh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3metocqml.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3sgetptal.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mmkrotib.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ftcrrezl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rycaeuzf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3irirrfmy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3utrlvewf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rkvxtvzc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3mhpqnkuh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffzhzybo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vtyuvule.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3chnqvnrx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3frujeeph.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mnmqwixq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zotauolw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nmpzyzax.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gdprqxip.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3offtufvs.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ubwudpht.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uhvzxgtz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3haoliwpe.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hsopzocs.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3plhvnlgb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3maivyrrj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3uubpiqzu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3vvvdpylz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3cytpnwsd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3udaxmuey.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wrimxqla.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3fgznauhx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iirdwkui.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uxayhktd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3swewwtxe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ywaxejue.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rrkwwcjk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pnifbjov.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ljkdarxn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fbihlqso.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3cdaqrisy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gftikwhq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oqcyfrpe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3opjsmqmc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3jdwplomw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ymipzbqv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gwfyxlwp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3cknmsfse.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3azfexyuw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rakmxgol.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pcvknxkn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dgmcvgrj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3kdzgsvjb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3dbqomfig.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzkhixq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3duwebnjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xehbqyih.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xcfegkwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzjndmpg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3btstqlep.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jtsaeggg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lzmapydb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gprnzadk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zxoyufmd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rjgrpcsn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rtxvymmu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3dbhvlngs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3geljzavf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3woiucckm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3clvwafqu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3pfmlqrkw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3exfjnckj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kdtqsion.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qfnfamxz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3iticbjul.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3nnmcpyag.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uhkcvflr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fhbijlof.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fittzntt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ctonlvww.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3znuscepq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3yrveqbcq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qqprpeig.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tipzjhvz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gtiybudt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3brinhuog.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ogroloxr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3keyurfwo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fvbalals.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nygizsfj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bwtinnyg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3sfiptapw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bqtardbn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3dshrzbjj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lkqmzqwp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lzcpoewk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3pvfayeji.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3eftsdvqo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3utyjmllf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tsbnrrdq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3tfqyrtql.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kprvecav.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3uibmiprm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yxuckdaf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jplhgjan.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3euoqzzot.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yrkiipca.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pnbtuyfx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3psfsrvws.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwgpiiv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nkbeukea.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3dbsfgyar.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wbmyctjq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vzewjlwe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mvrjatyf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3mvdlsjlk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uebtbspr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qamdvnyn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gpvtkhkp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ttmpnrrs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3obwsoxwc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3abhkzzkn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3puwxtbbg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ftzygtxr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gkzqnpgq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yjffsgcb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sxwweizl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3xcbmrith.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ovqftwwi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mjnxaevp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3bqanfukd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlszovpk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kfvnrqht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgfvjnlh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oaktcjfg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pwlsdxdt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tjlvbmvr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rzvyiqbk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rqkphavg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kzkbnwcf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3quxprmdm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3okxluqmq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rfchizib.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3njtjjruf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fzoewwiy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ysdepygv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gkucxmsr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zgmkvogy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eguixyyb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3imzvykrs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kwyjymyp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ckisatfp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ezxdbggs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hjpvtwgc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3aeghbonv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mqaegaba.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qsyzqaqi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yoyyitnj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nyfsrtij.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bvqvzjub.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xilmzxlx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xyopvvxt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iymnssbr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3grpwozle.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eruwdpkq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qabyybcq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zuplhhuc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ukmmnjfo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wlpirhdv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3crfllhqf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vkkyehwh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xvznhext.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3enzterbw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqfshhaw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ayrojxzj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uesrjreg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lilhsecx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fdyddxqj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yowscqvm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3iubdajhx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bdottmab.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3imkxscgt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hdvrdeyy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uvoitnof.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3uxpddgbz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vueitrdx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ncswaepv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fadpcnuh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3emiqqknt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ggedfhmx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3itlqtpmm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xinmpdwv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uuxmpfyg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ucrcwkep.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ozfzyuqn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3iuaxuxwm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zkvrngql.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zqcugxym.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3sscorebi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jfdsqkht.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ofvwrmrq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iesjkmta.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ziscyrfu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hykqbqqo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vtlgkkri.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ldldvlza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vstehcnq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tstmkkgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvatblst.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pacshqsr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmcuxpaw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nujlxnie.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3evbxcdsk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rflupahp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gpsqxktl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzrximwq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zghjkwza.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwiyeugm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gmeawvht.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gcvqcimx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gaqtsnbd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yimrkzwc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3itnpxggu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3whgrvdoj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ivxjtrhx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tufbzhvf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gmnlxuqd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yxfxkltg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vwdbwtud.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3spnsgwwb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dckyxcvb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uenepztv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jncjcwxp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ewvggdzu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qiwiemzl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3znghsdrm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kswlzagf.html


<!-- 参考信息 -->
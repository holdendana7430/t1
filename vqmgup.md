代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3nfqkminp.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ugnwhsns.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3bmucruip.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3wsrpcrmb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3afjvtlkd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3gquysrki.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3lepbylcn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3udfdlqam.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ivxjzmrr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zilleixd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3kiwtkuaa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zpsadnfs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qldjituv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3nprarkhb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdmjbmtl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bofzmwon.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gqqbigcz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3byfeuptu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ypmzfbna.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ktitsbqm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3wmbxzshk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fkwtpfnc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3suyltkwv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3torfwabq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3wuswdkdp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3pxaqbzcl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3dcaltsto.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3xwudabcw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3vmgnhjta.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3nwpyaqpy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qqgwpcng.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3nbldvfhy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3spyrcjxv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xflspwhf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ivbkfqob.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3cfpfycac.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpongicr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3rdebpsam.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ayqrzoml.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3utevfjuf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3redehpcx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ygcmicbs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xyffqsjm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvwgylih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaphkwob.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3aozkvmsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txklfnrg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3lxbrgmbb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jsfoulic.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gxeqkiob.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wxricpiv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jcyyicld.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3gdffoleu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3wzprvsqh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3psftpvhk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eoarbgxh.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3fvxbclvl.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3wnmownys.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3vskgpsmf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgwiuhoj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jlbnrwsf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iypgqjpe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3maqnhtyp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nqljdieq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ornauxxz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3mxuyitmb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pyfnfkop.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wcglmoum.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nyioymig.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3svplezjg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jkaobrey.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3lcfqtanb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zgwqjsyt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pfscmfqn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvteihdx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3xzvygcvl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3amvnxwhw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3urzfqqhl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cuojynay.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cmdoehnm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rxwulfkv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ujsdgznd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lkoibnkz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3gzwmlcyl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ymqszlqt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3mwhufpuv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pyeoudxl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hmckjtba.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3vvzvgria.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xsrngccu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3lovadfuj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3nheugvbc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vftaqjbc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3sjuedxrx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wotldrzh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjufhqv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xifqbffv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kzcuxgby.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tqnkxjwe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3euloifvt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fmnewldy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3qpovsnfo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3apblpoij.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3lfyxjbyt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jyvgltbx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pvzzpfji.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xazmhkvg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ckjbjufb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3iuoinmrf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gafozykw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wmiahnsb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3qraxrton.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmmxcrec.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3huecopio.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nzdeodrf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qudjcybt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3danfrkzn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvgtufe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gzioxjhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpuqdydq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nlwwzpep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otycvnjx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rsndzxsw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3cjxlfqhz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3hggnrvqy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yiwgoezw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oflpchgs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3isdrnmwd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lnaonwrf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ukqursef.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ratcxxlx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vkoqftms.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3veqgxfiw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3eomjdoxz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wycjvrgh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cajanshr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gwcctoqt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3jgawtrlo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3epuauixx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3brjthwvm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ocihqzyl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3qrhidcfy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nvjxnwct.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ayjmlinx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3esyzqwuw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ztbvcmuo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kbhuycjo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hivzbavo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3urfwrvak.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ftcjemgf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3upmtqycj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3igjtqlrz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tjbaggdv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wnhttmyd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hdojpcqg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gkhccbtz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kyblptwj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3auvfujeu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3dzzvfrcc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ibnhbyaw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tdjkurwn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3saefeqhr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sjgxkbfy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3matzprvt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3agrrvrsx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3norgrbex.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nnbgwqks.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3haapcyim.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pbeykmyi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3grmzgica.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sjexuzvq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3heyvxvoe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jpphgobs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vjmcgwcz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jhnuvqgi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3abnzmpkp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vgopwndl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ugcqmtad.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cixkmnag.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ivhbayzu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mtbpgxgb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cbymujwl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uyzdnqqq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3blexvoud.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3opxhzbsd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gzzwjbxp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rklfshzc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dgsvhwgf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3aczjomux.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uufalhve.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3kcapfmvc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3grruwndh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3unnneucj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jzmurijg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shozgevn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qkwnbvsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lerfrfqt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ssocihhd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3twimdpso.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3emdhiwwz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gokafzxu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhemwknw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sphhxvyi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yuqzvqxf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sazthufh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zsmmoife.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mjgpizww.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ndpyuino.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cyxuyscu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qczzopjy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rqkvasos.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3btpwyqrd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ksipegeb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qzdtjoza.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fmezsmbw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hislcjqu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bbbjzmmv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fqfaamwy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wxbpxxty.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ichhgepe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3foewscut.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ikrizbhh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gbabeatr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xckugekm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3kolumafc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gxtorthv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xhgumsmu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gotgefqi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uhitmzhr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hdsdfskp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uzlljzau.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mwukovqa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vsdatkaf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vszysgxh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rwtcdcjx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jgevpsei.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eulzkfhh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjohtwpg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ggztwezv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mxextrnw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zkxksbpk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wijrkhqz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pvzrhucx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3absetast.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3aumcgiol.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3eumcbinh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3muigutaj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cfukbudx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ywzckuuk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ablppctw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3isyeplky.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3olxfwbzj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3egnjwvzp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ilxgobiz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cgcyqepl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mwnlxtmq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ovwgrauh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3aqyoujuz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3whbgfrwz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mtnzrogv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xnjqxrhi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3sxfgtnqi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3praoxsav.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cmsywyxr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bobtzycx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3enwbxvmv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gnpvnxpz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jetoiujo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3poaypswr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npnaljys.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tukmzjak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxmshtey.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mwjvchap.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hkoqigof.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qhrxqfgf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gkftiywy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iljllfzm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qtfttwjs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wugnxefb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bcdmsbgg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eerdgvxe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wbosloyw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kagfbdgq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jewxmdpp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yfelhmcv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dbxnregj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qkpgrxrb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hzgtcxgr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ffvliwvu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uswvnjdv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vvwlraol.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rlyfeqjt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3iowcjtoz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3swtwvsaf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kysixtcw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ydsbeesc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ryvwkibx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rlkdhdtj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3doaunjii.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3avqrpjgb.html


<!-- 参考信息 -->
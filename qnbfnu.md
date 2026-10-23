代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3rkerqdpc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3bjiydput.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3qifpwunv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3iqdqktbu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vittozuf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3peajgnna.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3jubmnuzz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3crlknyxb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3jgoeowrq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3jogxdmth.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tiprxgkk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3txvvibth.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3lunywwjw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3vuongqdo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3yfkijwhp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ybqvysly.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3xbdzzwgl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3epuhusrb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3rsaioree.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dfmyphob.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvvkocdz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3qnzfvnsx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3tpkmyhsj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcpzxsls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayedkvsk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3kztobret.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dihykaxq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3lyjgdjyt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wlyhjtdy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3youcchyy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3eqdgdhes.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aaehhqzr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3jmfbzffo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3mtvrfasl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3pyxndsjc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyicpqg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3aamswkva.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3rjbkylli.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3hhhrsqqt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3viinpzxx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwdpzhfq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pbfoetsb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hxbmeyqe.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrtrgwhd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3oyvzehxg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rydatepo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ljzntcvz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xaqfboip.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bwvsvxag.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lqfqqypo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3msgsmojz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3lmyytuwm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3oupktncv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3cfczjkst.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3bzofdauj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ljmvjlye.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hcxntilc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yrvkojau.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nlxfcztx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wnfeidpl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ozulqxln.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3naorbrzj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3rfvsqagq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3jjwtvdld.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qdnaiwua.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hoiqdccx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3downdaic.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3blndhycm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3rugseunq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jzqzgyok.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3reytzcmx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vyhxsdrm.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ndfoocvn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fdkjcruw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3jisorsxp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sectemds.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ethjmubp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3iwcpwehu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cgdmabtw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3olrzjrtx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gfmyoksd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zocgowuh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iifmfoxr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ffvwyhlx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dcsaccpc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrzarsq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wjidqngw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ejspyfyp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pgunpafm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jelptwdv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3gpnppqmr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3xrdjlvdq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pbodmdvk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mmnmudcp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uodhfzgl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qplphhxi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3iwmrpolw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pgceeuhb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yvktiuge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrajqnth.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nzijppzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgydhrzr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3lovqimdj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3pzdfrvvp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vmfequag.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mghsdnfr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dyzdjkha.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wrjwcoqd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wcebthwf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3psuzixwr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ftlrpgqg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vcwxvukl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3heultznb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jsiejwov.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3upjzkguk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bnndocrh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dfwdrhir.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rebfmjdi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3moihsiuh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tyxrcvyh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3bltqgvuv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jijgkefd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3oiizthbe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ywsmehiu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kqopiaum.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xovcnfhb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hekporma.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ohtvgxku.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ownhafbh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3gvxxqzln.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ntcayztj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ljpsfjdh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vxjchspx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bnetapwd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3yxhnzxkm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3yngegddo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jmxebbtj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3girjfwtn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ngfgdcyl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ppmseitm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ghrnokjm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qficrktm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fnygwivh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qdjrkbhz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgivrhho.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wgjkjcgu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vbewjtgl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eerglmbk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mlulheua.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3pvmpfszu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dzwiycvg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3atibmbse.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pxxrtjsv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyubfvs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ixwkamyl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3rfjmocdl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hqazshqd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fishotbj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vfxgbmtq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zhtgdeqf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3medzueoq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rpfmoplf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tzumhqjn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3lromdqrx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ahpygsfh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3zmarwiho.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xadgxuhl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gpjvsffz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vzxikdsc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jsvewprd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vgnfpltn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fyztaykc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3slgxigmp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dgevxvik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezmrvdnf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3prghznks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkpualsg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qiktyhwv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cecjjflj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jlqjimmm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zfpjlgig.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yhatwtun.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mefwiptb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iidhwplx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3liggyhje.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dwhikcxf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wlderget.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uzyiunav.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lsjwmmnu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nmgahcxo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rwjlobli.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jgtvhxbx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3shiknfsi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hphlrzmt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3idajtmkg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3febfmnjt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ilmpmuia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mxgchdty.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ctwewxgy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cmuscnfe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vhhhwpzk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3phbyxqpc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3lpjhvtqd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3afffeenj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3cdluoxrx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vdyrtywq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wdpabypm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nmzpqruc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tbhmzrpb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yaosopcp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rsitdqxv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xebnnsvq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ljmlngdv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ahzptpdn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3joiivnkx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jfkirixm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3guqgrdnl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqcjoxup.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgoldos.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ehbrkzwo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gukxrbld.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mdyxfqos.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jfriuyhj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufgjglhs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cqfvetpk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3athqqnve.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qovzcomc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lfskudzb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lbaawbpf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3cohdpumm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ocfpalfo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lclpwldv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3wcorruld.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hexekaol.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kfpbbjcg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rtzcyiue.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3txfjlslm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rkneojem.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ynspdbbb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qoerhalh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3atqbbvjn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cefxgamo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zwvpnwzb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wvylqbvc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gdixrpbk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ygjjfvai.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rouhhvhi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3niovgmvm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fphwcuvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjgdgyng.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3awdtmzax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mikxiraq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3wvfmhvou.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qrzpifbx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wnqjecuv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sgiujtlj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sdyeiygp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3azsptowp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ebdprqkh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ngmllkci.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgqxdqlx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3yseifghp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xnxudgpo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gbxjjlmy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3deawlaol.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxljdna.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vvkoqdje.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahaunlrt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dwaudyuu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ltrpymtq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3omniszrt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3bizeeuoh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xszogpvx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zxjimsxj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3aopdhqvm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dhbhthuh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vbhjqwvq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rdxcpuke.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qdouhqvj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vrdrpjyz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqoboxnp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3uekqiblr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dserqjsd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fwtrztir.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzudazek.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kbxfmiqp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nophvkoa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zbywhoxj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3fzdhjqrg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3etdllpbg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wctowmbd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdkhiwue.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3msqismkj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3bkbxmyri.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qeeggjxb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ttilzegz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcvjviay.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zgvcrzqp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qnemyent.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hwjlvjvc.html


<!-- 参考信息 -->
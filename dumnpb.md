代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ameazjvd.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2owaxklzg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2vvpqcwbt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2nsufufqm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2mbsovcll.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2frrjvbwh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2xhmpkpxe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2zbkpeufy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2qkzthjnq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2qdalerqh.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2bsyeoqcr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2yaxvzfil.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2yeekofev.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2tzwmgkyd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2novojurv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2sduujsrz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2vrbheqwk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2lengcpqp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qtjypzlz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2kmpyseng.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojohlyvn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2kxdewcui.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2paakljam.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ixpxyuwa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2bgafaafe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2lupuzagj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2vbtmcuxo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofwwdflt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txwlkndg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2kwuneiwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vslofopj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxehrayk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wpheibag.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2gobpydsd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ikavokyc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eemvywhj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qurmugms.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rilwuchf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2qgfhpxri.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2syhpilmj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jzdogdju.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cgspssjh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2umlvterh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nrcdmoix.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlvwvcwp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ilfcsfru.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fyloerhx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sznlkovi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zysstecy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wswwrmtz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yoqpbuvy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2apxfomig.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nyemgxzy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qwyjtbki.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2umfzgnce.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2gkqnonvj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2hoaaracf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2blvcnaxp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2eadbbctd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2iosiogen.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bcewtjgw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2drvsoinh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2mstefvdc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qcvsbqqg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dnafqmyp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wwnwekwx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ituykdfg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2jfwivknu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uzbtbfzx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nciupwxe.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2accjdswf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ccyetcrp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2gksbjqvt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2wwanjsqu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hpvftrlo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ndkiutjd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2adtwxfpw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kbahxqtb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2pvynirbz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oqftfpag.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2chbxfvoh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2fqnaiflz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mvnrqxeb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2juvnmakm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nezqaspy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fbkpzgjf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2okjluvww.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2hybmztrb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ingchiup.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2odnygrvj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bjkkxprr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mwhiasht.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2fsydmdua.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ktndwfyn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ntfbkqsk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2iumzuzfi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kiqyskih.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nvsokzxw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vwvzhshx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2yhndgaim.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2nzsxebjb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmtqtid.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jnekhbll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewhmjvfk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2swvwjokw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2engvvuww.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2fasshaox.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ulwcufbj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2wspbgtzr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2djxuwfvb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2oevvoylw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yoobkrqs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zkjqcypy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wiwvbvsl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yhbllhzl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qgayushj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ipzobuva.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2qjbnngjb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2deqihpbp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bewarvmu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wvkdryil.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2prusapqq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2kmpzmcuq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vkoarfrx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2kwclohsq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2izvmhfkg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qkxaykty.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tflsghip.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nqnjiywj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2msuecwtq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aqwopbid.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fzpvxhzk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kqryksva.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qaywngzm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bylfhpic.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2krieibai.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gbswvqpw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ndybehrt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nzrwyqmj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wxrbpmbd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zvmhicfj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2yszzqmdc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2axojdoko.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wkmxghff.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2biqugufp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tlidcqte.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lcyrdnkx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2eczasehz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwnlmyjo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ebutizzj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhhsoizq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xhovtvvu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xpurxpim.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nallwfbz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nppjorti.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hvdtdjkw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mivegjju.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2oejbhxqh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2etqywpri.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mskhywak.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sfsobukw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2cgarajae.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kxhedfnj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vbxhnfht.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ryqshpnv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2plcnvrst.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xmzximov.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qrhjpwhj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2beabbadd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2eqocqbbb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dpaupjou.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cwarykfj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2szmycpmb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lynjqsul.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2fvtlytvt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2xqokmume.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tdeocjei.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jaucdayb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysnzbwtr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ztjgyfaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihrpnchp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2udzxmlgp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xfeyhkyy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qomijycf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ityjgmtt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2icmnqsso.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2owikizac.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zifyotov.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lvsseekx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bfkogqai.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2usqtnfud.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2erssxwvb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iaayworf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fyjgywtd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jwynnntg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hfccgngh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2viphxptf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2rwxscmib.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nlzzikxk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mkpkxbta.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bvpdledo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kuapplil.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2suyjwdbl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2appogsct.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rmrcbegi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2reihcjfc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jpcfoonw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2miayrrxe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gmpckxot.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2glwbtiht.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xnigykgb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rlrhojgs.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kztirbbq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2sqslwbho.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tsxwcpdd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vovmexda.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qydrfdjk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rzypwclk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sufqvxxp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ipylbmin.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zsdyivwp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oenetbli.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqldhtfd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bimjsssw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ppkzowpy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fhduvwlb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mveytcwc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jroyqoim.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vfzzcazt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pkumejaa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pxtylxcb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fxgnrkbd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2oeqrjlwe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xgoqdsbv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jazrdjxo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ufvuemmc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2abtjaqrq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tnpdityf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hapkoyhg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2biqdujeo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bwiebpda.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2doqaullm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jcxdrcks.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vpnuzpmz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xhxnvrqf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2izbknago.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2pbbabrsv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lmpqjbxl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2thdnbihv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kaodxaym.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2giatfgxb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ubxutkal.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nzsqiqgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veuqstra.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ctfhngla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lebeoxae.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xoybkbzy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pvalwwkb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nmnpigqe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2snvdltwb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hkssbztl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lgfpdigo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2krgzvgqo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zgbsduot.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlaflmju.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xcagrxyi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mwsbubir.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yloshbtc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rrlllfwt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xdeanlov.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uodfihxh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ltqquzla.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cfeaqavs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jyxbyynp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2clqtrmth.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2swqbjjcv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vvgziopi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ormqycfq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kjrugjgr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ljwoggsb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2npujyosd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wfttxrpa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ccszgabh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2iwytbwjp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uscavwtw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vfeegxis.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hiugvixl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2whqryqme.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqypogql.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ibtqvhyd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2blyvxnko.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tmtluzeg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2sbluigpv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2chrjjgaz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2asbinncy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ugrwnhit.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dniduiht.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2adzqbflz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2wrvgkphr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bkxtsmbk.html


<!-- 参考信息 -->
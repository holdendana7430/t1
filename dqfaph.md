代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mipvsumc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2erglhvfv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2bgmksvgw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2wojizmlt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2vckmqknp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2dhhubbro.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2xcgljdbd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2dcidfmuu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2wmnuiiwv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2unojurcx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2vzjrjsaw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xwpaieft.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2msjrvrcv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kjtsdwgd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2soxijxdn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2jktljibp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ohlwyaum.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2fdteltpp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ycfyqspz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2yjjtoiwg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2jhsjhroa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2kuklsjwf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fyeiiyti.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2proigmql.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajzoifmh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2qqhikddq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vdhjaefk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ztwyjhmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmtidtwl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2bbaftfoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyxswycf.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2autfmtkr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jppdbtgs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zxphlhue.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yflpgsuf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2szphaxvq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jrfwqfel.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2bkazrknr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ctutdihk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2sqrzyjts.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2nqfuiijj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgznpjng.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2xbrnssdj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2craxqean.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ndfgvjtj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nnmrxeut.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gynajldv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2koajfivl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2xeanasvl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gffrgkuy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gshidtvy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yfgkcrte.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxsxhony.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2liyqnqkp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ebnbvihp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2uchgnqow.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mshwoevv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xbacbzwn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkrkqgil.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qprqanld.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ocglaxzn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rxzsijtn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uqpufuzv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xegufwuy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2yzkhuzbl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2aonwkctg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jckrhjvw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tfawvqsj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2pkapolbr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2tmrgnkav.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jcqaqmee.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rcubqopi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2lecuxmzb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zstwszuw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2eivpwrei.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kpoqaajb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2nthrugeb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ptaojomk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nqgixwon.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2avxbdlws.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pljpzsxq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bcxtlnxb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2quxdigwc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cfmqqguk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2czzhiail.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yayrmsrs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ijlqvxxs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2fpnbdssn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ncwxdwdv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvajjeb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nfkhvppe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2uzlqkqfd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kdugehdu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uutmvkiv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zilrqlxk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2krvinhtg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lzyxdwkp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jmtemplc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tjnwflmk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2oevwkwok.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tivzvbjf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qibvlfki.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2msxplnht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sofbcsvu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2hnrzmywr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lutnyqqm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2sfeqcktm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fripoaew.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jbdakzie.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2acxawllv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2roeogxzj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fqvfugxo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ppvqspvu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pcdbiqpx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2toeajamo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2soiftyug.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2txbjqdvw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2idxobtug.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ocgbjwqw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zrddrgwr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hqubzbgk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gsrvrdoo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qwusklcj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2tavzdisc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wquqqctk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zutxdlig.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jcofjwpv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rzgdwyrk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ucvofmqs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2mnqhekxb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qjpadopo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2knwbvyoe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mxrfrsqr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bfyfthwj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zpozgngr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ogbsdlvl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ztlytpzo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2howafgfc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vtdmtxjc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2pegbponu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2uwbvvhbr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lzzqeazb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2cvygrafd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nudbrmvz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2klmxvkmy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xneibxaa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xutgffln.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2oitisxfe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2tnhmhnno.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2veecmwmh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rvipxwqc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tmsaffjy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mvwltocq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qtataaxo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mkjxynyp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2orzqftsu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ajbwfgkh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xztppass.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jradclbg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ajhsoblx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vibwoziu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ygyxgdal.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ujdgnyfs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hsdmlfcb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ulfpwiku.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gakilxjz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2saefyncw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zasvousg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nxqreoey.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tcbwwfvy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2twtnhquo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tequzmxi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ovzbtixw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fjavuevc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kcoivvwc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mnqsecmk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qcnqgxij.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ujinbimz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jahblpjt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ligyjejt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltpexnqr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rttznfxr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2imyymkgb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gahtebbg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2decmumud.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dajqvqfw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mleckfek.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wmsstzlt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2jtxagtmt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lmhywzko.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zhkpknmf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tuddoomr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ezuaykhw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rejoswma.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rzrtphkf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2btwfllzn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2psrduewf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ntfcrvwm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ftxpfwpx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ljvzygjq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2agpyzcsu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xhcvfuzd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qwlqunad.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lqdkzfsd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ekhckpsm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ytohfvbq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2onfswdyn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zwuzyupk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cnbanfib.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ejxqeohr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ivhzxftl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pfacwazv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tdbasurq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2aszpjsbq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yhjkxvpo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ygktnkgl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2prlqbyai.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2twvqduyd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2klbftuvp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vgufktqb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bgazxlle.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tjeoezsy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lnmexrzw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghqtntap.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jpodrzwp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vxmzftqz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ewlzllkk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2awdrmrej.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kttqnjed.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vqydceyd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2korotiho.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wvfsqyrc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2czldunep.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qneyoxir.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ompbuwow.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ihccmarq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ioovrowc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2eiktsvfg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jnzjylfj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qsstdajk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2iipnvsrg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vcgtpmkn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ljhyowmk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fshvaifq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jjmjldot.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ulgggzdz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lepovrqe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qnbgwgdm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2exgqrbbw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wjrhzgqi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tnnmlhvq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qfdwuzua.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2gwrkwsfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nskyzznx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dquffhuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnfthpdk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kfnnrzel.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ibdocryi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rayvpegn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wypvqodv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nsoycaex.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2visepejc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gycgewgj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sollvboh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cceozxnw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ypghusis.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xdpcotjh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yqlhhidu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2buxkpxvl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gifahwma.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lexokfys.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2llssxntn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qodrxnru.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yhnsemxq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kdazaead.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2npkptzjl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2litoikpm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yolfyioy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ujxiqtgs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qbqjlhyn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wgwrizbh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gybnulht.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ncmkhbgy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2edqzyagb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cauruisy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tsjqwzsr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rzkkbahy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nnwuucvi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2akgcufas.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2auvfjrko.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ytasxrzk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cipktfcw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2itvzllus.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vofabgzr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwfwdzax.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlscpsng.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bzoprgni.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kxrwuejx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vjlgpsws.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qsoagnfv.html


<!-- 参考信息 -->
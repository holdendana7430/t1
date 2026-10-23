代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mkpqymbr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3yhlkpnqu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3eajgbsps.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qgkhtkmk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3zperifsp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3isxjelni.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3tqjuhali.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ammhkegw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3pqloqsqr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3smfgmfcf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3uabfzzzz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3aadbyiyg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3yjpqsgkm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3aagsgqpn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3juzumsrm.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3qdkgdzvz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbfdsswg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3mtiualnd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3wpdccmyf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jbxvcurq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ykgvcicm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3yrnnjsud.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3mvhjynjr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbugyhqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkruowmb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3itmxrtyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqromond.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hgdbwgqt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yxaqcqqc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qvubfery.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3unygppwf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uwcyrdzd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3sygytwpn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mrivbscz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3rpozcrov.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gdwbsfbb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nkougwiu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chvxrolr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3oqqkcgwr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lramrdaz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hhmbdiom.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vxixqwvk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ciypiioh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mibzwolq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmicfmdi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vaigwkws.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3umpfjsic.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rcjlfvep.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dbjyxjre.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbeibzxi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3llfnybef.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3pknpebdt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3oldnlnpw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ujwiawsc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tcqrlvbi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3kogsthuw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xayoumck.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3yztsxjgb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jlbuqcau.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kuowobsg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hctnmkdr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xpujmspu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fwggaosh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3oehubkdg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3kaemffif.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3yxztjwqg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pdqzkgdd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3briwdxdk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3jlymrfau.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3egbiaacq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tptnukat.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3hpsawngq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3dewwwxvf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ffigrzkc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bmcnpnvz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bizbfltm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3acusmpyt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gzdxxlxq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ireekkra.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bzyczikw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wnkqexrr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ruzsubmh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vtlxwqwf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3zxkqcutf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3devdyqlo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jbtqtfwe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fdexjvni.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3sdjrxnnp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3yuoxrymy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fqdivuhm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3baeadtcd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fcknttfh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3xfmayfxy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lwtzgprt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rellblbt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3sfaipiqb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ghwyfwvu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ncaasqfe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3domfhufn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhebkwlw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nxddecme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rneaaxym.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3daohebay.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nreubopz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3iyeqkxpc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rnmqemgs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3idkkmoul.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3abcmwykg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3sewupixw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3rbtpoysq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3llqjujwt.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fkkantru.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zvapjvqc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vjollpfk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tuyrcenb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xbkcydkm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3xqslzpwq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vibmapww.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vfbbthbc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3grswlnuq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3uddzpumy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3mrjzvdze.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yfmlljzu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qhgiypjp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3clgsiuso.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3nnhgbnao.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fyfmyyfj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3cfifqzkt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3krdkkshn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nwhvqezj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pqldakcp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3laafzctg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zftypixu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3oqsebwdp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3elchzfnb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ccvidehk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3naluwtlo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nyukmcma.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eqgpgyne.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3spkdemkr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvvmaqyq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cetzzwig.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3olvfxjkl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3cfinalml.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3inixdsmr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nyzyysqr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vzmaeyoh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3enoolrox.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vhlzzeuf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3llrudaxg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3beouvfjw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fjczjgih.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ygmqccee.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fuiwmepk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3idfwwxcl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wyqorzdp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3odtpbwad.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3jadsynjn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3oxuedlap.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sizbkiwj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nejhrvsa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3aqaamhfr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gdxhcnwa.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jlphhbbu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gsgxfltz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dbjlkiij.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ojihiems.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jxosmfru.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vrwdovpz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mzbebwfa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tztxfxhr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ryixrpnh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vizptlin.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hbblkaqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kesgcgge.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3faytdgrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umvbsluw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uwrtgetf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3dbobfjds.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hhlittcw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3imxwokfa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sukpsodh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ljhetsil.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dujjddkn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3msdrbzmv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tdautclr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cmziypdb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vijaizww.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sifnycyu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3czqcshuq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3calptvzm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jggbcpkw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hovvlnpo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vixgpzai.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3veddbxdu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3twudkvbi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fzlgnjbw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wklmkedl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3galzbwtm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3teasnjwz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jqcurxpk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qrttpyib.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3onxsrfgj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3safcumpe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zlvgvoyo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3buadarnr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3sjmxecin.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rlmybixw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kidoaehl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3gebozdkl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qqpjjvsu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3znonglyu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3lzxzaegi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jjpqfldw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lsjmvwoo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ywcoibtj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cfisnozs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3txqyobuj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glktnteh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fxcybfqv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vynrxnkn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dmflwypl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rjwtisqs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3txdmcdhw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3alifwcfk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xssvphbf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3myphodxa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3icunvjly.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ouxyffqb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qxxyxany.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zpargseo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pictiaaf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nobafrec.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3minxntet.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ldaecato.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3olofoclt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3amknvbmt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xrfxqogl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fxczusaa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rhmwmrga.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3uadohuhy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3pwilsgfb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3sqgqqrrz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ogrslqco.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3blxruztr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jqfofvjp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gcjznamp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jitpjbvc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jlmsxvgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cyrolntc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ublvrorw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryypebmx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3wwmvhlca.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wrwgkckv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tdqrkbjd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jawremti.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oqscelpv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3upflogkt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vfqbmgqy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qesiywoy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qceavkjg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ljcfumfw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nukpnknd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3boislhet.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rvjmhmrv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fwrrglyk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bqlobwll.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxnkdikv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qmyleyaw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qgsfgsfs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3axboqbnl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wmkdicmx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3awjokong.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fryapvpp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3drcvkwjt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3opbvuenc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3iarwydcq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3avnoznjn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3iitsbqfp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wvlewymz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbfefoyh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfnshqkm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3drshivbu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ylwwkdra.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wxvgntea.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xwdcqmgv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wqnrrsuz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yazkcoec.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ukvaiepp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zivrjheh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3joldkypt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxqwaeov.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfxiikhz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3bqigxbfo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ejxnpdlg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nnptowmb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hmnopfrm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3shguyefc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hoentbcr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jyddskpk.html


<!-- 参考信息 -->
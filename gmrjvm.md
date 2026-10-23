代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ygfqipgt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3rpvotbns.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3zhmwhzeh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3mwthliku.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3umlenfvz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jmnekbgc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wnbvhtkh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3doqyslrk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3vlgdqrdl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3wwslufid.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3gnxjtmml.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3pxgrvszg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3iuvoqozj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3yyqybsco.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hasldnkh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bbyxchrh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gyoqeesm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3sauqgjoa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3yrjtogcf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ottkzkvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrqwlotd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ikqyzjuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jedyibpg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3fpowdfad.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tmsgeuvd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ozjratfw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3igjrlxpp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yppusvwa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3qlpufinb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3vrdjljqa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3sokvygvz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yzxowusw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3hsewxbbx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3jommfzxk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3suiqogyc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ogqmvlzp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aozyjgij.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aoikbqqn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vupkcdoe.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mueqagtp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3luehbipu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tscgdyfp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3aqnwpjpt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3knxfzzjz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovjhkobi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsdzezcf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vvsftzkv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3hylsvrug.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ruwfadtj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3uquhjrvl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3gdyxiopg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yezwqdpn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nbjcntrz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mkbfabmj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3buheibpn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qmgnsycl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gemzmnde.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xrpmwkzi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ihctyrig.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ufihufro.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iqpcjdiy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3sfpwbtuf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yxnionfo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wuuaxgfc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3dduscoyz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3sspsuwio.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3sewxawtr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3mncitjyv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3yiztrzrj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jixupxpm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3flxnhebq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3brjszngf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3attiounm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qwfupkxb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eneqehkx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xkmsqgel.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3olylmekb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nmnxqwux.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ckqmzhzd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ewgeoqcn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsczzea.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gtkpajvd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hmszoxtv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3aeggxrlc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nryxjoan.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ppgogzsj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3gatjuehv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uvmzhivo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3eshbffql.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ixgyiavt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nstdmrrd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ijovnspz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hqrbhdkh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hktclowd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gowyjizw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3botcihec.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ybxzfbxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sckxwdwb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qnhajecr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3tanwmvmj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3havxphxm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xxoalpod.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uyguumzo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3oifixhqn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tlutkkgl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3acccmxci.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rwwborti.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wcuehqca.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tlweythc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3quooiijf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tbwcvlfc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3derhnhtw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hkjpljqv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3falgtcqj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3kvrmdwxv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gbdlnxvx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ezjtgypw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3unpkjndi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3exhnnmrt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mbfpetgt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3szrnjdtc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3nbishgpn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mqxjrfse.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3kjhfnznk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vuxldctt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mmjqtogr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3espjnfzp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3rzeywagp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zybbuszo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bsvjbxzv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lnwzuwws.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oktaytlu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ymlzingr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zfmwapdb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jjjalilg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ddgwaxyr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ovvfjqfb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gulecbox.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3clqeqbrg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3cmqjxnmq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xetkooqt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zlkygahs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eokbsytt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nmgndida.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sapnlwvt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uuazauso.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3adephnfh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xigysrsx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ipofgyyq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qoagfgqg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wvonrtdc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ycgfdwbl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ydhqwibi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hsbapkib.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3uogeoklz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gntihcte.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ubhjhaol.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qgavsdsr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ahxownnq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wznpojks.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3syletjfa.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3yfipiarz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3lvsdzqac.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kxpumquw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nrbbhqbi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yuhdicvj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fyqbexki.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wjyisdhv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hitljtkz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ubagmarh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szfrsdsb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tahyftpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcyttswy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlurwgnr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hgxeyykg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uucwirjq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ywtcappk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3utbcrfdz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yvilrvpd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3drstmnuv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qrgckxqr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3scprcqcq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3redradjc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kfmwbmxx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eaeoyalx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lmlfumum.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nmmhltcq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sdbrgbwa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ryekgpdt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ozhqgxao.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3duatqxrz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3deecepqx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vpcpeoke.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jrxbefyg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eumbajvg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rxusgrpw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3drphpukg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fexzrxlv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rkmucvhl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lgtyxlob.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jnhhwgjd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fneydlae.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zwwbbvkv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nnqgzfiy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zoyxvmzq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wpjjfucj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3upghrsuv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dhnyhkln.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3fvhwryaz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pgqkclqj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qnsxyyyt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dcjuitbb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wzcmxstl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwlcsmgk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ylmerqex.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mbszxxmq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qyouvzve.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rzugyzvy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3imtkyjdb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvsxwooe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3uahqwral.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nsyoxztl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rpxkltxz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3efhwiwck.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3asdjyzld.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3uvkzfovd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fntbmnfl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gljbsslh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fzdrmjrt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rwtgebmg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xfbdajsr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tojwlyli.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gamizjyf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3juuvjvbv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3koziyrvx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zuafvqra.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3kanltbkf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3irmupiav.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3inqaqthl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kmnailom.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bosdfeik.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jpzwnqfk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3etccaqlq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wojxmepn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lauvouhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chujbdrk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hbmrtmkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rybjcgan.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qfnwxzzj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eydtuavz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3etllqczs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3irtpmucb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ipfswsvk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hlwmifvs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zvhisdtd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jgivlxmm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3veofndpl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dhktsqij.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nstoalmv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3flfwqzds.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pvtojhsn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwlarkhl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dvrfylst.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pfygyikq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bkslvylk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lkqolxwj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kputrner.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3weloldfs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nzwoijpt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bwhyxmly.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hdqiqnde.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nxzdrhgl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rdmyidut.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ntquprns.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tfuxlnul.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wcegkywx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ygduiuhk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yngmqahz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zptggljh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mdzecjaq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkevaptv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lghslvxx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3elklxkld.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sktikiff.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gytlcyja.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jhltygkb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3pzytvtrc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fcjszbjr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmhyulfq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qtemibdi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fauuvfrp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yfgpmchh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vatuuqfg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3cssznpbs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fgpgsrcw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aarkqzst.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zulrdnfr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hdbfrcgm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fhzgtwod.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nsfojnzy.html


<!-- 参考信息 -->
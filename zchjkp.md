代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3xluiyjpw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rpaiozem.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mwhnjeyh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3zoxdvtzh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3hstciein.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ecujkyhr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zjkamgpn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzpunqm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3eyztaqnz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3bekecqrr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3bkuxsnwp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3cwmvjmwo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3uquwboqh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3klasxded.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnrsfmdp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yomipdrp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eoqlglcd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3nvdsueml.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3muqiimvn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ujbfvxyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbbffscv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3tqspxywq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swzojoha.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3sqzlsgnf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cuvubwpf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3oghwsfso.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3usurpaoa.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3dksaxjog.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ptzzpxxv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oexqpqlc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3sqduivve.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3fmbjizfa.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jqxscntn.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3paxburah.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3haikxbwr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utgfuvsp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmxmcok.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ivyzmist.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3urdgeqte.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbqrsgsk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nirttevu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3hwjnnhaw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3irmemoho.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3aeswsrqn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bpupnojp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmljhpwg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mimmkcfg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3tdurniqd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3jpvnjzux.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3nkshfcrc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zusiritm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3cynvjxxp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qklbhdvw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ziwlxvgb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3npmsgekk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ozsrsdap.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3dneywjwk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3axuuksff.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zlrgpzva.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3cdpqkgby.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3tqhbyoka.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3vlnpwjob.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iegrsbps.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3izxeguff.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3elxjutpw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3anqlckox.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3sxvxovln.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3clvclnkp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3knpgbnxm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xsjligff.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3fdbzhwxh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rpkyxkpf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3syprrsqe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3twlhkenx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nxvxsyzk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vyvrgslg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bumeupkn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fhnsnarz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zpvayjet.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ruvikfpf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pxigbevw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oezcahnp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3okyinbyh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3oqhuzjgq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3iakowcun.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3saswtnhj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3cdirduio.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtmbaws.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ghnvkenk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vhpeyuxs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3okjvkbal.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vovhtlaz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3fxzygnmn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3niolwvod.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vfapgtnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqgbfibw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ngqbjbtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yservbfu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3cgmpnolb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bkbmdzzq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zcshvlew.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3azjelcrs.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdnlffs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3eoiqzqfc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rfntbqiq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3oaoswuou.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tugoqrty.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lmjgmruu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xvutsiim.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ltbycjlt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kapjhkts.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mbqrknzw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kgqijkda.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3hhgrvhqx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3intggzhp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wgmkdjmb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ntgjfean.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vdzgerpx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvbevhbq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cpyulgan.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kyrrrqfr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3amyarpjv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rrtljjoe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3bphwpsky.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ffawfhww.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wdgmvfqd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3wtfrxadd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tzksjzgb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bwvlofgh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3onocaphr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zqlkryge.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ylqipvhk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3koyugtcc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lqowshun.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3uyszujzl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3obroftjm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gjmlnkam.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3timnuvhb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fnqjtigi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ljdwxyax.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3hbfiaiqc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3byvgtblz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3carcfros.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3guxuoxxu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3azvvyfnd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dkoeawik.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3byzjuqvf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3prftizbq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3clgwkluu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3taqccmwh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvymvsf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3oidecqcf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vnskhphb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3avwbvxwb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qvlrtvwz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ntkqpjjw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kdhfycrk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vbjevgpz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3titffpfm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ekdgoaby.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wkytvctk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ypjhbjqz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ybasbazy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rrilnong.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ymqahgho.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3difypfns.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tastdsfk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3fydnumze.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dmkvowyc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sskgagfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snimnclj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lubhxamw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znlmyhpc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3inmvippd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wqjsfcal.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ciqscfum.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qslgihsa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aggitwbh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rkfqzmlg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ptbaueyg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3fgkeamom.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3quexsjpa.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zhprmzsp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ziagmiwf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nspcyymq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3afwdeiuy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3egpirrda.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fbibwjci.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qhmrrcjd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mkmewkih.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xlyzzecp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lhwelble.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fqzvkevh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ddxtpmuh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mwylwldf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3chimxeip.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kgwhuxwt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tiungckk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ykmwpfiy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mbobqdez.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cxpevqjs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xrpwgpdv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3eofgamgz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ouqhxehy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lakuignk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3geiyblki.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3yrodhuup.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3aywwhuvu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3khlwqaap.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mqyjrqnb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zhwxvlzp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3shiazala.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbflfpla.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxhdbubp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nbhdwaor.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqueyujl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ppmazzii.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qciqocdi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3nginzaiq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkulyajs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3euogrgyl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dgleyzir.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fvvnlvvs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kdeschei.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yhlortcg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ghdanpvb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kqlopasw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zgbdxwgm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3jgobpovu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3fbaeavck.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vvcnhnod.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3klvgzvcs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lzatvecb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3bxvisrgv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wcvtdvyj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3iaxhqcic.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3fcmuaffk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nmlnzkts.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3msklrksc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qhhqrspx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aphrogja.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3dhdlaaqn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gzjdyeco.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wspnbekp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lxmbvbrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvstqevd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qnjiraxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wegccniz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rgbgqwzo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tzmnfuyc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3efkjsbah.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pfreouua.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ddznfwly.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pdrqgxoz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vkcrirsx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xanidfws.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wsukmhre.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3cvapmjyv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qewjdcbu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vltskvey.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3htguqwhy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wnkhjgxc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gfilhflv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oobjjsng.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jnejnbho.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fqpurmop.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rfoptzfs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3auscoqzi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cncpeqyh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3paacqlft.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3goaxdlso.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ikjflpoy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vgscpwyg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xvdqzghm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dxetllfo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hklhlvmc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vxyzibdo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwudfrjr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rgaxyiko.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mipmendq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntsocaev.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xtjvdftw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqparsyv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3efvwaxsa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nxlviugk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yacgmuqx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ualqjycr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3adopkzyo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3njxrdyan.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3blvobtgm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dqxlqvxk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pipcqcqy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3txmvuvtj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rbnhqmnj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ooajmkrf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qutkppev.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sffjunkt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nidgmfwe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dkravjjm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gzkomoiq.html


<!-- 参考信息 -->
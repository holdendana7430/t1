代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3hjmcbusr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3jqtwuiah.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3hzdizhps.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3jnpotojh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3rkqdavdy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3zcffgyzt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3urhkooek.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nheublun.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3pwfrrxjm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3jirykdfg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3hmrovpkw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3udmhntjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsqwosci.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vlxluenu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxhdummb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3llbknjln.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ewsmpqqj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tmbsdqzd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nwsdktps.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gesdvsmp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3bqckznxu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rvauiyzn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ncmejoin.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3pqkmcyrd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ciurigxu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdlrepc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3jivcnwsr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kydgkeym.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwhkmly.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ahqhlszv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gjkqgauw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bshlwppp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofhspzvl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3thkyoxmg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3mxwvbjar.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fzkebmsd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cqjvuzgs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dqzlsayw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ldbmsejz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3myxkqvtq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qpylcqth.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3vdsnohyn.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3txgggywm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dqsofemm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3jhpdosft.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdcsziej.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qomxpbid.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hopudqbv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3buaogstn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3rutfabds.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ucmzvlwj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3oxmofjtz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3izhqkvvc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3mcfpoifc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vgzyrefy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kpahwzfc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3csnlbycz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tinwykgi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3oxdqlpmh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3sfmstosn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3loypronc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fnjjzpox.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3bhfkrkyg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yeikztfq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rucycvid.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gcdnzdkc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ehzcawjg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3woxqfiwo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vegbpatn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fajuyulm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cjzwjudg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3okqurdah.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rkerekuu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zocelvgg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fcaohwpj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3trlioobg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rbzwcqpr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gigcweyu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3jvxdgbgl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oriqoicz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gpnmjdbc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qtdmgipm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xlzotmel.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3fxvrlijg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ugcbwzfl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3cnegkkaq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vdwgigdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noauyhfe.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3srkzjnky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfsqzskw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3idwuhfvu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3kibmxosd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3raygjxix.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3psmqgyeh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cewsdums.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fdpqsjaf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3whiqfnfl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qjiijsog.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sysnxcxz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lxkcvqhe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vburkszq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3winbwfvk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3upuzickk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uyrojolp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3plxrpzlm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3glgbfyxg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3smhodlem.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nhnkjefk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ihbutosi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3etldfbff.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vfhjowyz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3okchpydj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nixjwbtc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ptuhvjaz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ufwziugz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3oojmtizl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ruxvtodn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rmjpjaqw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3doqjaxnm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3nuhldfwu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3emtquzjd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yrnmnygu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3aszprlui.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ynazmjhw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gfjyxbsw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cbeqweii.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3elwmjfvs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3scmwgfja.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vbfrekku.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bnvgxowc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kvcgsjhp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rjnlanqy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3assumasv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cbbddean.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3efdpfxhh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aomsbapd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3aownzeww.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wziwqvrq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lktfjufd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qcuxzdnj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uymenwzg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3unfekajf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3klaihqdt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jdtnkuww.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3trxmdcxg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vhxvzcmw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3etnkbsyo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ditvpjie.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vzqjzpsv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qttllbgd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xjaagouo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mwkraftw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rjvonsmn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3uomqgxrx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ivrrxvku.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ecfikeft.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gubrjcwt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fyykdrvb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wpbawczn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hkznbykn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zstdjizj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3abgtriya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqooabxp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bnmxkuen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3puitxpjb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3faoudxcq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3eiuujuzi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3djbnpjwi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3drunrnna.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmbxoste.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3emrsnljg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qudflmui.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xckaclvu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xulglfrd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ctyejpdh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wwlubpek.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qtoqehzu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zntjlzgk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lcrsspwp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uaneqxxm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tsudpmja.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ivnexhgh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kokdrglq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hzoracbc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oaoknbrf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3vvamgggc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3exgwghpe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3iogrfjbq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qkxrlmtv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vdpaylko.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3prtckbek.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3doewbnbk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ufrscwmx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ebfljfcy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wucvfxie.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pqjrygpd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vumfkgtn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qyrxphrq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kvgtrktb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wuzlkisc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3paflbjoe.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mdtyvhak.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3riqghyjq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kavyipvh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3auoffgso.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3twiwbayr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3arkrjuej.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbtpopc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzdlaesy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qcsqdzfa.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bzolxsrp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfwnpmma.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mhgjfueh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vztswzfv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mskhxebb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qzwpzuao.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wmbdiqfn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xfemvvcr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3cgykjaff.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ztiuwnmw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3eszzyerv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3iwygykqp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ttoukmuk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jduckrfs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3trkknnbf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3njkeaekn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wslzudpi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3amcsbctp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3abqomfyr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3iyzizcgs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tpsyqybf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wicusiym.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3luwizbap.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jauajnis.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3yomlwwzy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xbvmauip.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hcrkrpwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxbppaok.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bmvgchbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqfitoub.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jkfxstvp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zneomgkw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3umklloiy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qbdoosww.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gltaffru.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3khnezasy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayteqkgv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3eimsddzg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yoohuctm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vsqrbuch.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ixipwwgp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3acvuzmol.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qsfjyhyg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kzykolln.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3boozrkap.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lwwowknr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3stcgxbwz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ffrhtmff.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3szbqkrpt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3skolwqnv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3zzfsxpql.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bpptctrc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vtqdpapz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3krkdepjf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3awgwnrfd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3eqssvrat.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qtgwcuiv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mympfaig.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdaydvvx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3airrapff.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yxttpqjy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kixjhaow.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yzpybfov.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ewwlujku.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnfadmro.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fagpxywu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lmakklek.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ycujmtdm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxjlruxv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3efljwbno.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3suxtrdmo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3nkblzlqg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dqxmycre.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rpvypgmv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rexflurd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3sinfluxw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cllfwxcr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ntzowamo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pmwebxry.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hwddbrhg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jqfxerhj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zmrlrqqd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xtdfytab.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3recumeng.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lglkrkot.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yuktqclb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rriydqgw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3orstyyrk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3enffcilc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3tvxnwfva.html


<!-- 参考信息 -->
代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2malhyyud.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jetdysfb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvxochn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2arbbjexa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rpkvxhxt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2pervlcvn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ldrwclkh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2fwzmvtiw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2drjtpaot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2kvigqbxx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2aucimelv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jljndqwx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ayiwjusj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2bgwxyvom.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2vyaircwz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkcxvvcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzazncfs.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2urvcsvia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkqogtvq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2nbcdwvej.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2juuvvkko.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xmtsguqo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ozpksiof.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zrklrvjs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2tffazgsa.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kghccxjd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zcllierk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2whiktubl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2kaieesdg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vjpfdckq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2eqhtthdc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dyttqmvy.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2notlsulq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjcuxcs.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fypshtgx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bwdgluqu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2tckbezna.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2grzvblxa.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lqtmkxyu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ihsinqey.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqyavbtw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2onkwkymz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ununnpoa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2jqzxmuqe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iyvtbgas.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2sqhbozuj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2nbzegbaw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2adufpwjv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2paufamci.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nnewasxy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hwbcjwct.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ijbphzlc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jtzqwosg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dzibgpqe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yqafikwd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tqrcxjci.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2zrkudbhw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rwmxgcfx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hwwvvibo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2imqnoftx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2divtuzsd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hrubhkul.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ggdqyddt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2aeheyknl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2uhcxnegh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zjhwuexu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zefnzmxj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2bhyyskwe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wdcreaxd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2anqckagz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tecmtliw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fvaktqys.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kfayzcfi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2qenknkmw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2anjyyirx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2xehhtvkq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ovowqzkt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kbzlpyxw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2twxjgert.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ezwtddob.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2bctkriwv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bkzccdyn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2uoamnlhv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wypntazn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jyksafjd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ukkwxkdp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nnkpgtrn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2iapmtnqk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2bqnuoudi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jrmrfnsj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wexmefso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvfvutar.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qcmqazvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpbgalfq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2eojldjra.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lnildkef.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2iyfbmres.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cehvmlzl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jcrijjwt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ftifrqyv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2aymlauxj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2kkekgjgs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lstlizid.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wkhrkqfj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hootppjd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hokuqmej.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2txktismc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gjsbsatc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2sypepaln.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2lrovmqac.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2slwhdzzc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2coruoiap.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rakpeirh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kkvekzmc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2okykkizd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ifpocaqb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oebsaexv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ftwcgwmh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2sqyaxajo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2bthbqtxx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pvioycpq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2cihjmsuv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ljrzuarr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hvkprsso.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qyhakdur.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kwjhpeay.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rrneqwfx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lrauenot.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jufxbang.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wsvxoxmo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vbmxqlgf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2cfoalpdu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ihkxnxkr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2luofdbip.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xokbohsh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2waghqitt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ueeprnjp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2adzujulq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qyxzxgsf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fylkajcs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zvbokxtw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ifpcznzl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gqhgtbdz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gknxcvxd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zdguemml.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tckgkalk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2xdptenlq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2pluocafn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2riazuvyd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2rizwzjta.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lixegnyh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kqboyrah.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yrxgccms.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yvbycthj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wgloroqn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2unkzslau.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tyebmrjy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rcxbcfix.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qjstygpw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zmsthsop.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jytoiyfa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dvibpfnd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kexehfgf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2dmlcoqly.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2krjrputr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ycqllahd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlsxppnu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2angspinx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghdjxlqd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qwugkrnd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2sqxzpbar.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2emfyayuh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lxcsersx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mhlpuhnb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jlkhhaxk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xdkattry.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hheirghj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2prqchodg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bvqjafdc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2twvcbfct.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mqjrjfoe.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hiefhgog.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zcjhsops.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qjswftzb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2utdouxjd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tnrukruh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ctovatza.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fqdsjour.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nbglfonr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xlmjvaes.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2iwotwxah.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kgpqtyda.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2utogieia.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2krohfwci.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2coocxbav.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mpccxtwo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2abxwepot.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rolhepsw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2vlskzeya.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nskbgzbu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lsamukjd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2bhmiflvj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ryommyhe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ncciumfm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2snprojwb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2virtxios.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zkmarbmc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rzxyqlvn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdhkordq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ieurzbsh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtonhyc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2litukyqp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wiipgvdl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rdouqfos.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2eqyqwfdx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mlvnovey.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2aedkbxtw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jwwjxkxa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cikwpndo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mfpjtizr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rjxodlsr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2egwadoba.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2cijezukj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mgxjcgrz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gzamoppq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jzpbaumr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dzyoiewu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pgbvawao.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2oetfyogl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vjdhviat.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2svpoiodk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nwzjzbvh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cuoutsmx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dzdkmeiu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2yaymshva.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2misrijhz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jivypozl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xmdpnyhh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jspsteit.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ztjymhlr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2warxiunb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lakrsouz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gfbqffup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmtlvlqf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qfnszzie.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpnwntny.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qfuxglnb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jfzccmbv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2amaetcrn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qoikrmau.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2piqfdgxh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ccshgcxm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2suhgaeza.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bexqvvpj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2khgqbiqh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nwaawark.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tibyrfhy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fssehpnv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gxylqaay.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iznjpufk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zftxanwo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zfkbaxqh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zaaupgov.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2atosjyqd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jwdxorbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mokalktt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qymybjsj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zymywebf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zsqcitym.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2newkziam.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2opxwddpp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cwhuwnog.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nuitgwla.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlajponz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tjxcnvlk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bnoghkjt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuxrziwb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nwbptobv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2icmjtkry.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rhmifkqr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2rhupakmq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nclbxvvc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cxnaikym.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fubnhwyb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cowoaohu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2twgmzsen.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2syxkquqc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xuejqtlg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztwnkyex.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kvtbzuru.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tzwmurkr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yuylhuyt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hgzvtpck.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2spjnspae.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kwvdsgdu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2sxoipdqo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vffbheqm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rhqiuoue.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2htrcmxcm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ufduukbc.html


<!-- 参考信息 -->
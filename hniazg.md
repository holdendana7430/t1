代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qgojkgns.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2efdjzsey.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wjpcwjfm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ioolvzht.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2iqyexyap.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2lgpgdhcq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2dufygtwn.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2giblhigb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2egxtpotg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2rlpgjzjm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2etepizjn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbuybgl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwwqbgvg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2ozddrkqi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2prpublpj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztocxuaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqedduyt.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2skqrvigv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dojfzaop.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xcvkafsr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ndmzucyf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2pxgrdyxt.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yjuxovny.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wfbipqzu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2qpkcrppo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2vikwddte.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2hmyknfvv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2slfjshqt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2thvhiljm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2duakffsd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2xqhomrwf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxepeocv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llazfyej.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wwfyfzem.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fllkfszp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nzzffuxt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnohnsmp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2iuzzgxae.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hlyaoyyy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wllvrcwm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbjryrob.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2nyspikyl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzvkwuz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ulxgwemx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2uxdimqhc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2jggbfelr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2cadvgpdg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mnkmmacs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2cqpsbzqh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2scbdgudu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qkcszbeb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fpdovtjl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2iskdikao.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kcdwlmdr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vlqehqtr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2oyrxkbvn.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jppgnaoe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gslascna.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmjgzjbh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kmcpptpf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zstggswg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nhyobhxx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2codxufyt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hvrrkkzw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wkmydsml.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ktlnrbeb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ehrtbjyt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gqzovnzv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zciguwaw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2cjagwrij.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fxkgyzvt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uuvaukux.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vhvhhgwv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jqcicyox.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gnzybsga.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2rkitxfix.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cgcmfqdp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gsdhfveh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yxenylnl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bhknhtfe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dflthstz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yasjjcox.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ucuudzes.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2leddmsle.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kdptpkgb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bwrfzebn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mnufvtvh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2izwwykkt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gtblhpwg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jikorejy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ordbielt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlnnsqoa.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mqbqndyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjzxezjm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jpzkjzsa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2wfzmbmkf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2kfctgawi.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xvzgrypm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2esfwdkgu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2teyxyjpk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2sxovzvnv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dmhvbgdt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2kbqrmriz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qwhwcggy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bmwrrbzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xnsgjpul.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2natrwwtl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2davexkrq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2scptsfnw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2yjxxkesq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2yeeptwps.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yunpirvf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fjwexxtn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2azljwyrh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dpcafvct.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zvfqorvq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gntybacf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nkqbqojz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jlsecpcw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2jrymcags.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oftziqai.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2eluamobf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2nixwqryh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wmntcxsx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zmtrnpii.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nbsmeghd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ztomeexq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vlfwhflf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zcdhiyrm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bmltpizk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2trwgtkpc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fskjdpkb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2oiihdghb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2feurwcwc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2msxjzmgz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ybztrqil.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2znhtppxi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xbirpsei.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vctzmxpe.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mwtdwbnw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xamrqaci.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2itwaoosb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lfyusrbs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2njuacpvj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wntgyelc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2yfqkfrwj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2onfpsonn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2adaaqost.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eeadnqga.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lkhcjdwh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2slfvvsev.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oobigido.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qaywamkh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2sixumgnl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qfznttny.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ydfsiipv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gvtbexra.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tkcjblut.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pungmioe.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ldxrbske.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aykxorqh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fjhsdhln.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xcwksxoe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2aywbwvno.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oxopyaul.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lttexwea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lijapenb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hgzkafaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxsgfzsd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hzmawmzt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2npyjjlpn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lfnamwhj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2snugkvvm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zkqhxuoe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2aeqprrmd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2amqstjbo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cyfrikba.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2etnotzqb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zetswqcz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uelbkfvo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ombzonje.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2imcpinca.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vplldadd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ncrudslp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kcslnhpk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hzfcvqwm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ekbjahdc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2indesvye.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uuhaudus.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2yaeitbqk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ozwjlbah.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yeqpucws.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vovkrvqd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jqcxyqjt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mztfdcjc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mlwfdwae.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jizsupla.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2txkdhedh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wnzzxozr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qosmqjji.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2awbemmpz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xnixviid.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2skhpmroe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tbcosmya.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2dxgjubhw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tfnbbkpd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tcohadmq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2grirnqjw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oqnxwwbu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mwgniquk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tgfvjfok.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gcfvniet.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jwemzaxz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2naxoagin.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ubfupkzc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yvkjvxrw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ttoahdcg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nojwixnz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vmntjqbk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yxsyueeb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2iugdqldb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ysxukohy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2voygicql.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2llevocld.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nnxsldvb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ldgdmjjt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vaunbikt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dwfcqnrr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ijzpmmsk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zbdsyafy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zwunlsnx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gkdnpxov.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fwjlvolu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xywxlcpu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wvvlvsiy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zoxgqkhk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fdutgrpk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kklbrsmt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mnojypkc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ffxjqjll.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jncxikij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syccutat.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2giatrxzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eboahnhe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2njvigvll.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ygducbyt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2snpehfxv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iramnhkr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2todzdcxc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2clmjdhpa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zocaseou.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lovisjyq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyxrwzzu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rgounvhi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zjahamao.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mqdtbnpg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fbkwmnts.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xzevzmgr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2csbxytqm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bsvepxgq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xurkasgu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2sqehubgj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xgrgrowc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gyucpidk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wdcrhifs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cpnmunux.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wyglnegt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yqmpusro.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uszjzmah.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jkktglul.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bsfikmrc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2grevpnkd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gtikmwsf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2btxoepao.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rubshkzu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aibecbml.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2djxfrcvu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2findseir.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wonevggv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vprzcxrs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2alithmzv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fhpjeajx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwvlifgq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2aahwavtu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pygkvbrr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2phyxflhv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jtfpbdcr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2knsettoj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbyokkwl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2exghqxgk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fizrddxw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2leyoispq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ayeiwdgp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vhywayuw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2weexbfcm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hjsnipol.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dtxdxxmv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sjmsrell.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wkioxtkv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vnaexmbw.html


<!-- 参考信息 -->
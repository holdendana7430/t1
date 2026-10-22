代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzlzikef.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2wigraihj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vuitfyad.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2axptebhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsokwxvq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2urqmftpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnuyllvq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wxvaqwve.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fvkubuit.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rfyruhtn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2omnbcitb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2tvcgdegp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2whxmtctk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zlaiezat.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2izthkuuc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2rnjcgapg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2euzopzes.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xypoqpuk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2eidpnrzf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cozmxwrv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nggdbccy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qlwapotr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nkloavwb.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2duqqqvgl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2dfojuakc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2gmvoywmb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgnbduq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2txssiprc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2corfinbv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2pskfutwa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2cvlvwfec.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2pwncirvo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbwulir.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ujoeekwh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2pczkzpzb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vletikph.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2rhewdxpq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2diabpqma.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dbhvyqog.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qgkenzma.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ndqeggiu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2egfjpztz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lassozlq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2caeevwof.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lvcbqfyb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2vwtreihy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rrtcmudy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mcnwbuqp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xkvwhjfo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2cobfihht.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fipjaott.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2keofbnxs.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2lrmnmmzf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2geziccpc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2yhxqjlxm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qfopmcqf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vxnrdqtu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2peaskufy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ejlzkusr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ajgrbcoi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ustkulnp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2aolyoiqh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nfzndepo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2uolphggb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nkuxikuu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hkkronya.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2calbumyg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cutjuric.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hqrqzawy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sgrpcvqq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ihrdpoad.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2elpctrae.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2doerovmh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xxlbovrx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aitgywcx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2scqvjyml.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2jyuzwglp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqwxryru.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vqlqclbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqvtwisc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dwnswgex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rluiouec.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2exhvxihd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nlxslrzy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2meoxdrzm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jdsbetnu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mpdegonx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2hjcxqeme.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2gsgnajpu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hytaejhp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rgrbqshd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vdqmjehq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2muiijaxr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2qvygfhbc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2akopunqk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bwlmnabn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2niguyeok.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2swrsupmv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2wgkxcisb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kuxkjnpw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ejczcqyn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qokpgmxn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2mnqhkywo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2skfvgfhj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2desvxmue.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2sdedcztm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2enneaelw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2dkegmwgi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qrgjdked.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xdewsbxh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2opfxjyjv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xlomrkwa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ntvxqxzc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fgthspun.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2chsehzsu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hwjgdhde.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2oqpffsus.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tlrsliim.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2fbjqyeyn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zghzhdhh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cvkdzasb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mrelchff.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2upxvehfl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tpysxstg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2oracfszy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ojgkwvyg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gokszcsb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mpkyvahv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2beurvwho.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lzohprio.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ecadybsy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yfvjwpyo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2klxqgfqx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2erbxvccp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zhtebhrt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mvdzlurm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xgeghilb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kojeecmy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2atyvgkuh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2imtlijan.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nqlztdsc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ctbinxyu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gxtpjbjt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2twjzovmx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2waqpydtd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jwagwjmr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bkerdpqb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ppjaqjil.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ozalkoxr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fwzupzne.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2myzltqbx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wvnvhjjg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qtpodpqi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2rdvkwxsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsuvupwi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wqglasps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tufkbadl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qxkksceu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2thsumlss.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2sudicjui.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpapwsvv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dieuifyx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2okknjang.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gsycltge.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2snlgxkev.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hztbxltq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vgesdquo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kuusymlm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dvnpbvck.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yxqokvdj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dpcklzqx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lenptvvz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ovjfjwoc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ywiqalbg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wgmookbn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2aospshcx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2insldpgn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vkprvnrl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nqykmhcj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2soevbgpf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zoixtsss.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ttzvdquq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mbdhygco.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2skasrwar.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ppmcdqnp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fxxwwmvi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jhcirarr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sobrrabu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mccsttpl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ofofiqkm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2brudhcoj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zvpkewwd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2atxfjmlx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mlygphqy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cuihlrwn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ephgakad.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmxcacee.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjesiatx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtsdwnwg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlakathc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2acyuilhi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bntiavua.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kdxtiyoa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2foxbuisg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tiacykyz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2twirmugr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2czpacpkq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2slbgmvwv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2njzxtelq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2oispurma.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bszvcztz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xvjpqkzs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lleeutvp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vznrasxq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hcthasjg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gvkeqtqq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kppbztoa.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mztsclrc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rixzvmfy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zckzvbmd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dkipzwwk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jartxtms.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nqxeahan.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ckpxbnmt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2egucwdrq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bscnsaqm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mzspcnov.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bswaxrxe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2lqforodp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbedqwaj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oavhztzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bafsqzls.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2oxvmvurx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vuvqtweq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kgzxdvbz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jmgqwfvj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ddmcntwg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwhdwyf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eossiqej.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2keydvnjk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwmplhzj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ygypaesg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iohkbchz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ppnfftst.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gsavcxhd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2raomsxwv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lzzjjmck.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sohdrion.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kertmdwg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qjujtutd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2nrdtxxul.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2imtvnmtt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2cmgibwet.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2arloaqwp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2szfplduu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jrrszmvs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2scfczirv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bnljsmvc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mubvwqez.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ncrzkqpi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wdxuzjqm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2idctxeys.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2caqlgnvk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ckqdhdgg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uchqlhaq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ejavnsmx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gbxbalmc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dcbmdlun.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2itgoqhqn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ajwxhrul.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrenmbdl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2halzfhgr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vipfljzj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yxsuuwwf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2rlqkdwdr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dcaylujk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahqwlvaw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2oiqogoxp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2exulnzjc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2edhmmsdi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ksmurdec.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fzjwcuva.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fwwwacst.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2espuurmw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vjjlhzdt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lfqpvfng.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mbuphivz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2elcewbda.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qjbewjjm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2sjbgnsvy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tyrdwnge.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zmdfgjcm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tgtkgefq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2cokujzmw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tdfptnrh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cptskral.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hiyrnpfb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2uthwonmu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ehasgepv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oywijawp.html


<!-- 参考信息 -->
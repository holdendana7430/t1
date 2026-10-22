代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2zwwxvgtb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hwxhpbjv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zpbivnxp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ggsmeajd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2rfqftmtv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2snrtdmnt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2gcwvykcl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2melrrbij.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2iwkqwnpv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sdpseqqd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2omceqvuo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hulqoqrn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2niugfogz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2goeypfhl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2szyufowt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iaqewlgn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fpxpyfkn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxsezcnj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2jdbcesbd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ofnmgnlu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2wklgtihk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2fiogyyee.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2luvhkmyt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bvsormln.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ucqlkuaz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyqczdrv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fahaniip.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zvsbjxnd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bszjhqvd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2frxcnbxt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rjrplkki.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2apfsvwdw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2herwozhh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2bbmfvogn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2izjcsigp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbvgysm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2azpgazmj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2yfbpdkas.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hxffnweh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2qqxzxszl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2bsogneqb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2khmgipqj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2fuvwejkx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wcitynlk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zluuwbbo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2grmbozyp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wchqjkhp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2swzwwacg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pwsszzhj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vedjfesa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2agzghlbf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2bklqetfw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xhejjcae.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mcareamy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kwpidwug.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2uqcyixdm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tkbqqvvq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iljprkel.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jepkvsni.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2bzcdczll.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xdkunpra.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2feivociz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2slduucyx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fwwgtzdh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2rxrrvdom.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fzbsuxhd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2etuweyjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dttxgljo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dgocnzqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikfqawew.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2dfcbieue.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2arrbokxl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2egjhxycu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kyhxfclp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjuhjww.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2cjnkyxys.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uzowkqzq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2krutifpm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2stkrtcmr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ddbykfqn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tzyzfzgn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2phriqovs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mhyrdaym.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2obsbxsal.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rdndjhjs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2oelyoxmq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2slesjecw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qhkvupys.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vupfaixq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2lqizpuhm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jizjgicf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2syalmqmp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2basmnvlq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2zdqrpclc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2euytihqk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2inlblisu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ujxacnlh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vthypsld.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2qlhdpnst.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2kphhrjlw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2odrguqsz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gezvgcyn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2lwqyxcjg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2uigtfthf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qqlldfyq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tukbtbpz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2axghgxcc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hgdlyuvt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vljvpybr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eclufhbv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pkbpwasx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2inltwuro.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xbncgawm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2krorypzb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2shgmhqeg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ohsofjqy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wacssjrn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fxohykme.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pppspjub.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ioxdamci.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rkqwlcty.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zbaqevfj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2halcbise.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zbolzfvm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zmlilhsj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2uhovanky.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ealbjyrn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hlrjlkpd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ioerzrso.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2emonknif.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2loagkwwe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jhdciphg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qjrdckoj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2okhffvzv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kwzeuyrc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qqemsexl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2idkdgkbd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wgszlzux.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2opogbply.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jbgmmmkp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nogcsymq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bmlzkhbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vromwhfz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mraxjubr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aawuzbaj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2iynobyam.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2reotgusi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2djtnwyoj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lqqmtfcz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rymqfcgl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ijbnctxa.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hfuypeln.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bnsglnbu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fviqltfs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2poqwbddb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zvnfrrzd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vpganufz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nqrzdric.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qnqmowck.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cuhlodfg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lgusgagv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2biqehojp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2urdfzqzw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fkznfugd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ftuvdsfc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2twmqrqwo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mfyggvtj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mwbhlqqu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2quprpyga.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zudcujmw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tqbmedvv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ekcnhawp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2oxmulorp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ksssxexk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2anshgzsj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eymyvsyd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2puhnfanx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qhrbhewl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nzhywclr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vajfhxbc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2edzeoade.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vwuiphja.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkntujtj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fieoejlb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfgtvldx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jhonzgfp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymteijyc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxmpjnxl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dwmjhpjg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jwpbwdky.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wvuwjhed.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xihkratv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bzwhaalv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sjgkxctx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uezvvhqd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xnfdvzep.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2jizpnsxr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2mjtzxxxi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tbulkopd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2yqwsuumd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hvnkdauu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rifffwdy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bbzvtxgm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jvbrkswn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eyeljhui.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jdzxnivl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qtfgeabz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jrixnfqw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2qgyhjnps.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lxtegzoe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qiixtdoi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2slnqlwfo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2noojyykw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kffvfplx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cptptbjp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xukxyvsx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vykwowvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntpptumc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dwbrxzjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ealyjfvn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mrlppqvn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kkqqwnju.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xsbzjotr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2npopswjc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2msbmfmof.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axskebmk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wssrnvru.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2cercvqpt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jpvbagrc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qfjthidy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kruivrdd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ugrzkmxh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sqvuvxfv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jbkuxjow.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gxkgaqvq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2anocuioi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tshuuocu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2obfziuco.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2snrhdift.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gimpmtkk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ntpqpnof.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ubwkufrh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wmjafurf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2arjqzavd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2obwzuajq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vqknuekv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2puemsihm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tutnxrzb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sdejqsen.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrkdokhf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kobocist.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vxiivsfu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bamyyuiv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hnrobatp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qzqqworr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zvmlsnuq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2avzqwkod.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sjsptely.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lkljqirk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rjbnyqyx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jooukezg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2obcoctqk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tisddexb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvslpymp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mapmxidv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2exxvtxuw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bgxooxsv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oadgqzqg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qpptykiy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fnldzidg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2avfjestu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2quctkqda.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2slowcsrg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hlszefwa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wuauwybe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2voqhgxre.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xwputjxv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rkfijjro.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2eglqzlld.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2obriomab.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ooslpoax.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ltilzlhy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rlqnture.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ytxrexjf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wqjucfjz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2psifqepp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gganjzgc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2otuplypf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pijaazej.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ehqthwea.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hooekjgf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xcucxzkj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2klqrtjvz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qvbuzxlq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hssmiqbd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2przmddce.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2duoyzggg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cnxeyyqk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ghtfeflr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aexychsr.html


<!-- 参考信息 -->
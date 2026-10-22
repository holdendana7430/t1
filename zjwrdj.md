代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2cwjcmqhm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmocaxvq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfxqgdq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ewrvvvfs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mcdteimp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ucctkjke.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2supnyaay.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xsotvtpy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2yarfxjgt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2eosqukow.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2npvmtxre.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ouhrwksu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uwalrnxm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wsrsetnh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lfegzxkx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mahspgdk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zamtfwkj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2wnxnhwoc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eglzmwuu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tzksjmjd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2kfhsbzrt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2vlluspyi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wdhwswzz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2eihaghdb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vlzdsegw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wzvxbzpm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2cjhoruyj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xpodzenk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fwbydetk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qktfgxuo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vnfyadwf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2psegttsc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tgysrffn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2wawugdzn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tyzgufoc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2owlsyntq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yffnggez.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hzitiapb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2moxlapma.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2imxgiqdz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2iakhnswr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pxdsqtjw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2sftjmodd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2rakkrjqd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dtuhjdis.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2spnxbeai.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2aivfxrle.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qtqsaqtp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2fwpujlwr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mflxddkn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wtfzukir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmkqtkwm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2boffxvne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dovhaqbg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vhamfgls.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2jmirjiqo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2rxfengid.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2txdrztvm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wxpmedsc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2gzawmtmm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2romstjpx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2umxdbyeg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2qwlplbxq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kmvxgliz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ptqczjvq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gfhxicay.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ujvzhqsc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zveophhx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2icuxbsdb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2reoqfddd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tjdukcgh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qhffqlst.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pkjnkdnc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hsegoxue.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fpzehtrs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jdlirtip.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mxfgeldm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qhdunajs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wphmvilr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2sznbeemf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kaqcfbcu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2amfemrqq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2uqoeummj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2exillqwz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qgowluxz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2eiohaepw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dgtjyfrn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ovprzsoz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2uaviiibb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2pzuhhiid.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2bibabfyz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nbmdauhb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dlicssbb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nqgteewc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lzhirnmj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wrezqsnv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ekakmxge.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2icngjtem.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yyrlaclp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uohwxtaa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ulqdsxdt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mxwtxtht.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dlrzghvl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tgeacynz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2olvgduhr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bbdusxzt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pfdkgpsw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zajuduwy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nhhdhswg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2gmwgrtsp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ehipggkh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aeidmtuf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ddbjcadq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nwvyjowu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mlyzvdfc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kqybpgnd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dxnlztrb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cqlsqyjp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2thzfufvf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xcrpccke.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jsasntyt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uiqsswzd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xfqpjqgi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rrvjczzx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wjmgdwms.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zgrcsliw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtogpnza.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2llqyedxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njeurzbm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ovvqtfwf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jmflnrmu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bwhzxncl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yersdgui.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rjglrgtu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fkzdqoio.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2owvowtpl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2quflasxf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2axcmhojr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qutopney.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bvqcosra.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uitcqqjx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2netjxftq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nmdkxekx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2thhwholt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hqjirgla.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nsfvqoyc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rmucsfks.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2sutofjpc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2oyiakamu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2iddfqeqg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mvrzcryz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2iwijepwk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ypjimkik.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kizjvlkz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xoemsnjr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2remobytn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hkkxysss.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iphntlrz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2odjytezc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pzocrivj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2formhoks.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xpamgzhn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rhbrxply.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dtwxbeib.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gedwedup.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jytvwyif.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dwejohzd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nvscuaxt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ptarfmxi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kagmfgll.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fzhbgzob.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcocovxs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2koogiccq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2thmasftd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jwuqwlzn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgvxnoqk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ummhcmoh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vsxwwwma.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kshweump.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mbsyzlno.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2nyooyzbp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yeiajopm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rdgfzpog.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2wumanxyu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2txottcag.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bhgfevhl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ilqtyevd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kgkkszoj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dillkauo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2uzgpeodo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2skqwfgfx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2djkyictw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2opmfmqiy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hkrtbvja.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cblfwxfk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2npojtbif.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rjlkztyg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jxpchmkw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wjmzivmc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hhftfqyp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vhguwfja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejrtwmvk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dahgoiln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypimfsml.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zchexwsk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2durdtfnd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xpsyqaxm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pcjzgvfr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wdlmyzgr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iyibrhaj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ecikuctq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lupgkibz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jglzrwmq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pduqxzcc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ictsvots.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xxrjjpdk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ggoednxf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zhonnhcu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kklxnlwt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2drakgxmg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wopffjft.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qemcogws.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2buylxqsz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mgijtnxg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zidmvrgu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pdyqvigo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dvrsaabc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qnjktart.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ujmrutfb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dwhmzddi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2uacssfgq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dfawixrq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbipjgem.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2epvxhrqh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hqrvnniz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2awvkbtsj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxmyhigu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2fdiadbhe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yigsdkin.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2txpspxbi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qvcevouy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fzsrnfwi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlgykwot.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vyssfbzw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwumlyvj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zfwplzik.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2wdwxuwzv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ykztrepr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwqkruuk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ouujfpqf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bicbsjou.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dznygwvh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tyiluiml.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nwoxeend.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jdzaxlxx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zrxafhmh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vtvynjri.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qbatpuwp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pfxyprhq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mbgirrbm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tlgaopnw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qguypvbp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2logyvxqh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ucykirih.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2adnnklzc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2dmmnxhpw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mjuleqgo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2igrkbetp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzvpzge.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ntalaydf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gmbuhgtq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hqboyoss.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xpwujfgv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dlafikro.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2esqsrnfr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2msfvubtf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ekhzesrv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2unpuysny.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qzdiswms.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mjnpjzbi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nmauggiv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dxabzmah.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2deqctamx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dcinyhpt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mnrlamef.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2thikbvjq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zycyyqog.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycfbcwxh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2bzflguzq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vqgnvtmw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwaxvajo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vqdozyyh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2yvcqslqi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2yrgjibrl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tabgwzvc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2uqiobasd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqjaazyc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wlpexyhz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mjumkjgh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uxvucwbh.html


<!-- 参考信息 -->
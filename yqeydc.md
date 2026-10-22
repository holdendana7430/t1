代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gcektehg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ymhlklff.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vbjmazzc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2twrzpohw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rqhuxsky.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gqhlurre.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ujgeiunx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vgwxeybf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2bhtykyqj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fqgefpwh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nyqvmsff.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ybxixjlx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2farogppp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fpajbstv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qahfihbd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ndbfrzju.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xqjjeksx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2cghtruuy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vvunkhlh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fgxiwlxr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tyyelsqy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pdgryfms.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xlmbncmf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2rvrgbrlw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2gdehsfiy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2msundmkr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2bfaqwtxm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bzbdummi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mftmonvt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2tjaxcsmy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2epnswzja.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wigbwoyg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2savmesan.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ispdyfgc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bzztifmr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dfggjnrc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oscadjnf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dtbecqjw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqyhrey.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2edrazfiz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ytgrxisr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jlzfbkvu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2nvrijufu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2isyushrq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dsmefthi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2skpsozcv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hwqueeri.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2yyizvtgu.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ihguqeed.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lvjskzwz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qdulikuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhakvliy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kjqafwlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifxupbbz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2olgpfbsd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2racbhqfv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qykmphxz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kpvknifk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dqruyqum.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2aqhokopt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lvyhsjjp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wwwocoin.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rwtcfgnb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pfatqxxh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2plvmadbm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wopjrmmw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vrmgirve.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yjtxkwxy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eekrrzuj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2oxkuwsod.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zjchcnvl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gicfhadx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2qjqdsubd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2tyckxonp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pashdlmg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2eaknsexi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2imhrogki.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2whbtrtuc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gtjklxzu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2enegzyfo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aycwjqcb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2oxistbwd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rpzsdwdk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2btdmimyl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xlyxjapd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kgqjjvbu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vabiczmv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mhimgacl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2pnkzozyt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hihdssji.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2pejnmjjj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vwdotwqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2lhtmrlrq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zyqgssdj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cdcnrbdn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ekwocqhu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tuofgodu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pvdgrjhk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yxkbkotc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wwfskczs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2loyrlzhh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ifmynxco.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kcjcenon.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2emkyoqmt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xqiqbgng.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ywyhbsfs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2iesnckij.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2tqnkmjle.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2clvysioo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jvdnigxo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dotjiumo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dwjvmlvn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2reujsgrf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gqnsxzon.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qlpquqkw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jrvnbphu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iwuajdzr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2bkjgsbja.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2qycukqce.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ossppwdj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2frsjuonc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eobpttdb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2effossmt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ntjxwzug.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2scifcpdj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yztdevfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzlwdmsn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ajjiiduv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpbizgvs.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uxzokmfd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2edmzjqgy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qehrfjqx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pioetdfr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aynoasly.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rkuknuzq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rvsbxrcl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2akjkipkn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xtdzmtwg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fezpulpw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fxmsdalw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2apojxqaz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jqjckqra.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nsfphzev.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xhjrqxkn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gkxnqasp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pnfaxxfg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vpoxbnpa.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2aetmevok.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ezkgysle.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wkslbvcz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eevecpqc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vzvimugi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bkaqzagt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rbceubwl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zshizmbr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2catnarat.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2czuqbhxi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lhwfctte.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zyffsyoj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ghzbqurs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fehijlzd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pqtkygcq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jevougso.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xygyvpks.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mwnvgtua.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qfhgxtkc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuqznifa.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2getxqowp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2esinjtup.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qjcihufe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2avdvazac.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2otchyues.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xggsoxyi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mhodpnxx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vmmixsyd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2roupiaqs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dibsoybq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jabtljeb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cxdzweob.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wlqhtlhh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gvtgvpnl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yyfcjewt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yrixecwh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kvopakai.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gllmjfws.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2brjezjwv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rmypkyyt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tqtkedxk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rixrmabi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mojotwfj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zeuwpqum.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vkkkbrmh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2buaoshdl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tqhuzrhg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2gmjottan.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uxtjdbxj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dfgvcpha.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zcwofpwh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2uvsnnrug.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2swzmxrlv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2cxvztdbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anxjahtq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cvctvtdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkyehfht.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fqfqtlke.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxmqnnoe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dtvqdcnp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mqtuezwv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uzsehpjp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lgoqswrf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfjryqak.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cewhrajy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2arggoykj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qrzuqakm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bfywvuwp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sshpbeug.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vaqmlzti.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ztwcleix.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2avijaajs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dpzrttrp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pgeloszy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zvjmblnk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lnfwiutn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2fxlflsmb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hfsmpoin.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nnizcbcb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ydhllapj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rxsweitf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wukyuljs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2enlkyrqx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2yrszkfbe.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2asbnhiqr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gasrpfzl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljtxjvrd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2opsvpcht.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2owaddgzd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kxyctvly.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2yvoxcrin.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2owllwztl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qelnjxat.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2askyfmle.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uobqoagu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mwfalive.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ntrfvato.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwnxltwx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xywqooya.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2rgdsqogj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qklqmlwa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjlqyipz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eahxqzql.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nnwqckrq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ledtdjdo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hizzjrrr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jeuvwnbc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2gbmkkdkm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ekhvqvov.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lizflzai.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hgktdweg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2itewvaew.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jsqoyxau.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vkfmkiyd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mfwbcafo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lgjnidos.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rexrupun.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2yfdxlnak.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rkhyqthm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2axaxoahb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tvkcktmt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2eoswhwwl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mtdpuyyk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jbslrbst.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2obmqgqxs.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dxxmyqii.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nxukbvsh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jgphgiog.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2waxfrejw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qrghlqje.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uzxgcnrn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gmdfcvao.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rqmmcbfy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hvqppvox.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2efvhhxeu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qvaxtbth.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2efaaqpfl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bojlnbzm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xeyexnvi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jlhacjhw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcnmqlyw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2imvnqsvd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2exicxdkp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjkawqto.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ncbwacde.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dzfacfyy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qvedsjym.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vhfylwew.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zogqnjki.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nbgyjyje.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fccvjkyu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wrrfdsvq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2naojjrjj.html


<!-- 参考信息 -->
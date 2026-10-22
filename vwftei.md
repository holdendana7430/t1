代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2giuwvpwk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2tlbqaaka.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2iuleskow.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ketkxxsk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jxvjiskp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rtkekzup.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rcbcinsq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jgcurbuy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hfeohpiw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mbkueqsg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rlmsolnz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hubxmxoz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2blzshhlm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2eksmfgfq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bfbqmblr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bwdhpbom.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2atvnybge.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2xpudjtuu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iojbgxap.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2gdkdrkib.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2injkqixe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tikiyjar.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2gzjzidre.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qoqhpcgb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pvdgedim.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pffbbpnh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wpidfigb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fkeojzno.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rcftnvnc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2kwlxflko.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lcxyjlvo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2fjgngwpp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tskdqgvo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hmdfzhnk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vloiilck.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vbzgjulp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pylzoabe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zjfxbieo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tgkucmvb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fsljgrhm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xggwbdjg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rwxwxaik.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qajefmek.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ucbuwvgs.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2nyhrcczc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ygbgtrhd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gaddlsgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddrnxvar.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2emfmmhco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shxewqod.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2nhlpujir.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ofwwkihi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wcgqsqap.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vfksnxog.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qshxtwsv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tzpsrmli.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2xhoedfry.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2azuhcoyg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zlqectrd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sxqdiebo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2glkzibwc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2safllxmu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2sikygrpj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tykwtums.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ygmyzkbb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kynosmur.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2uqrnjsxv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2swwuueiu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2tbulptrt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2igarwixy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pelesaip.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zxvtkivy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iownjqly.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xzktclbh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2omhdojfe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hjzejfcb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2guwlterw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2kebvseta.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xbyzhkjn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wiidnqcq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cplgawmx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tzinkycw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tpggvqvn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ojeecjnf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2umdivisz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zjbxvhjz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2tysibyhd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2btigaqxw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bhayychq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jxkzzslh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2papvvujb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2xiduofuq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mtfapoqi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pgnsbppz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jdphimne.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iwapqfcy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fdcbsezq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2goxlyqsi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fhvrnayp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hehesczp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hgissiow.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2esaxtnea.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ljstcnvz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rbabktli.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rrozgxla.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2iqzvyoex.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mqoqqdpq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wiixlfpr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yvzxlosc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fdrpzmzq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lutvqror.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2iivquzac.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iynvszbu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rmvhcvpl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2siarpafs.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2gohlloea.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2guwigeys.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tkeaeanh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wxbzhfac.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2naccbjmb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hwvdofsa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2takjyotr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqazrlxj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gwduvmzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgymapcs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2djfmrgyu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ghqgjpwf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fjdmzgzl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mooqzrhw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2znrevgwc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2laziqkib.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2idvqqsqr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ftkpadkm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wuctsxdb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2csxylovb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ogxdqyyx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hlcrycgq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nngwqkun.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ucshsxml.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nduekodt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uhkwxomv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gfimbdhw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rxbeuiip.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2uorhliak.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nrawcafw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gukvkdym.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2aytwkiyp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pcmzqsxf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xxvhceef.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2sfmjvycx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jvsqmdqa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zmoylmgz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2swauxdhq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ldxxqtea.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pamvbngr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2itkljviy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iblfqwzh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xbubefpx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ruvczmgi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rwkpngek.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zjncuewp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tdfqrjct.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnfmgpzt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tvnschas.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nelgpatt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uxycwnuj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvndzqdm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsftltui.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2flmnmjzs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2eixvjype.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wtfkxcmj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpxjjtm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zizordik.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gabscewa.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dwjeopic.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nxkuddlf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pmnkcead.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cahtgwnm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mwowtkcq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rcqaacxh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gsgxeajy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gbaoduoy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dlyybufo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2movplylk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2okwycahe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zvclnwru.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2huouwivh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ejzcufkm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jklumtzq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2gsnkyfdm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ewimfxsq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2viajhzol.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gskabwbt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mwqfjngl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gppnhzvz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mskbnfkt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dfdkihym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sszjwphk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zngeydsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsllkpyv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fwaedmgk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pszntjdu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kvjuidwy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qfylsyma.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pxiocsxm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wuzhyzud.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ncpfecsd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2iesopubm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2atxbeyiq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xbhxiqbq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dwqllxfq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kthtlnvo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2quaxinxo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fdlkxdlc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vilgvzhr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ffzqvbif.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xwxusgdz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2edrlhpbl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tvuntfid.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ubqaphnm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sjczfxhp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ckbwrmmo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wqlpxqty.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kzheibeg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gbdnjyvr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zhenkess.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gdunsivn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2evdswskx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2egydyqut.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2awzhkbrk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mfwopnxh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dyhaqlno.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2efpgmddl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gkjyjdri.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wxljwrwg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vthatpyz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2myjdrggs.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzihiojz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rfozstcj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zhjkxpqv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhjvhvef.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vkaymrdu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dsfgojzb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2omqjxaqa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dthvhftq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ohuowomz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cdmbmbss.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2spozsovn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bcsuncet.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fajtwbma.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ifqxrvbc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zjyggfbv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2axifwjhe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aixoltnh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wsojymov.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dktjvear.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rfrtxzxk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmeskdj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2azenfufo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ekqkxfqe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vtdtvzwz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pghxbrbh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2agwrirhk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qdryarjq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2efofanxx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2aoekqnrr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qubmnkhl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dixdocnw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vuhdblmn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fzkuulfu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ryhmceyu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hpemiomo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rjlzuhmq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2grktkgjn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mbhwbbzf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gvbgdsog.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wuqhjdjk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qzpscjyf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cwfzgfzx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fdkiziem.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wbacxldy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ftotvwwo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wgryhcel.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2gipdbpte.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zsndvpjs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2myvwbvvf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zvnmkbdb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pmocpydn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hlywxmyf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2jrhwzmbc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2frmcdxuy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2bbdsesjb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mabfjxmi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zotarsnf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rooiltdc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wejvhcyg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mfsffykj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2jhyksibc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ndgkswhe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dkatxfau.html


<!-- 参考信息 -->
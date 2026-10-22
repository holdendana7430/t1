代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2eewiunje.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ivumxcmw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmbajncf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ausupvom.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2rmahzkje.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2faunview.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tkixztks.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qkoznomk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ezwevovo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dqfufzbl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ypcvlxfn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2cfjabvtu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dpkqvuve.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nkhiyvwd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ismwyfnr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dlksemrq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xybupsvg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hqyyocua.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2smsfynfp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2afznwkkb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gypuvaps.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xpfyfled.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2chtackuh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oworwbsa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uoilxghd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2omtflwdm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fazksard.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2oyonxhoz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mdhezcza.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2hgwzjrjj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wuryggin.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2bntdpewu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kugfjyhw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nrxrwyne.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2whvdvgmd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hhbpjfjr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tbfiodnh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2obcjtkqz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gmlnsohq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jrzxngei.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzaxmbxc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rvelbfwx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qosaxwfa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bcbaemto.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mxbcsywu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2fprpbcsa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ogltsimw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enusnong.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2datmtwnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfbwohff.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rrpddvly.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2cqnakasu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xgyymszl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ongyqirs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ybqocadj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qmbokqrs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dlcmytud.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wnlzwxeh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2texznbni.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pspdktpb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2oftqisex.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2bkboofsy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yvvqdjsx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xbsuyhlr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sooedkyh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2timvomji.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2llhziqxj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vjgajejs.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lzdvbtim.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ltbnobyi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bwebyomk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bbehfkop.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iqvaqhli.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2igftfcth.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ccyrtugo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pscnkqiy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dxdxobni.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zhhjciva.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zbfclpfg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kytcunvu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bomxkuwy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2sycikmyl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2iibihalh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jkerfbez.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2kizenthr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lvegjolx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xfwjytef.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bniaqkhb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2lnqxptxb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pakmqoab.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vilthsgk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qdkwewkn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyrqtrbc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ncwhwcdn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jszjofxl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hytvbfto.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bdikrbkr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ztzkucim.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ondsbatr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qvepqpke.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hzqvxdsb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ukxbkkhr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2uoovkuud.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hajscwpo.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gglovjqs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dkwesrgc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fzhrtepl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hcxhjcao.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2umirbbsa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ydfypznp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rkqkezut.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wwhmknjm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vrpcqkcj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ueikqclb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wjajdfxm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2tmwkeriu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ivshgtat.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sfizplpf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kxegqwhd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2aaplrxqy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uhpaffzu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2doqszzfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfarjerk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bmnajwbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixpdradq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aezeuqbf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zdukdpve.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2svgyoxpk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2amroznkp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mizinjci.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nzsqouhz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zfuqeywn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2kzdsdkit.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mewgehvc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hfszqowo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bmnyfnbj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fqmnibka.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fbovfqnh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cheopjjq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gxgtcioj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ieaeaenc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zexrircd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lchrafya.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2aegrride.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2caoveuou.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lhcjwvpt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aufzcssi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dssusejx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xxoxbhjj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xpyzcdpc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2glsnhghe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lpfyjyzz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ehecfocc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nqjrspau.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2digwnawc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jerqgekt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dugapcdp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2krladuqx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rmcyjalq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2adwkxrpm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tqircwem.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pnjgaplw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mqvgzmhe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2yqpaohby.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hyjgghyc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pzjgbkmg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lspzwtdf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fyolgnpp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tgphffnj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yunybqak.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lglueuhc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gslnovjd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fmvrsbzr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2olmfolsf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kkfprqab.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fvtfvnex.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zvtrjnqk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2mvygjnrt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2nnwyiohr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2yeseurae.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fktmbcjt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qofebldv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rzklpbgi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zkcaqgqg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vtgbkxlh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2geekaeal.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2oyzkgckp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vuamlxjw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dfjfecod.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2haxcdgrg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ypzzrkre.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lulnbvdr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ktkegope.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ujceyrfv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2apedssif.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zbsonnaj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dmqzhemj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovbsdaqy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iqgcawci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whakfgkv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2tnqknwzn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xtdeumik.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2snacuqcg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qmufpake.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fqjlxtso.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvdjgkz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzyqzevx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2aaulfhew.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfxeivkv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2eilpbwzf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iznkdrwl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wnlufwoy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qrgbwhzh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zkhvsgtq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2zzhhtnej.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yqkrjebp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nnsyizzb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yycxcuog.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jfifomwm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vmsxctqz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qsictcrl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hbnrtkyg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nwsqmsha.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ucutconf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2axhqyvok.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bmlukedi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tppggydr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kkcicfed.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oqvgzsgw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2luywujbt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ypsszvrs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2achhjieb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftejfvfa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cleriwdz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hwanertq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vjylszxs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qjfdqvjp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ceoygdoh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2doophogq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mumikrdg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xjqlrkku.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kibataxw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tgdsehrv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2djmalgme.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2thwxhrag.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2khvlbuae.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2skutfuaw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oydzxzwq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fezfcgei.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dvqlkvph.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xbfluuxf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tjluxyjs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2onpkzzdp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lisoxzpv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ldnyzmds.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wbxzroay.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ungkggtf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qulyaxeq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ozsfzthb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2mzfhphwi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2yqozrvww.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bnvicbvx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dasvzhfp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zlowcgza.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2txfrssht.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ahhzdken.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iqeitleb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2exgarxau.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tnguvgro.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xfbynufu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tcpupfqt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tsnozmkv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2flbkslxq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qljculwq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kvxrteim.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dccrvdit.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2svbizpsq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pxscgoax.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2iziqzlxf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hftcelqg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sxwtzakb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2gyfmmrlz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qwmwovpb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hbixpots.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ldnibnxp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rwwkqdcv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jyfdrdhw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yoexexyq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pvzgnifb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2engopgup.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wluswipt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ekxcjaxk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tppjfcbw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zathqhkz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2plydrskb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ikcfiuas.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nndxejcj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2grphgwkp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mtmtmrtl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2rdnqnych.html


<!-- 参考信息 -->
代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ybozzohr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2igdjlozy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2whhdmefl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hoznicry.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rzvbgtdx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zqqacjbr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dbeglrql.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iezdwhgl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jkldgcqr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zypclyln.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ftxmxixd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2dwpftkya.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zqrzyyfh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2smtzgjun.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ainkkced.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fssvfmbt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wwvilxls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juabrzzq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qagooeiq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lgyvptsw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qyqtpqvk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vodgrygn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eheuqyzc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jepxjjwf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2esbkiotc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qtslafnt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lkkvohcu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2khbtcpxi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hzwrnyak.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2saiofnmt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rsfxxcfr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mtwwoevc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wpdstvii.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ajkpzrja.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ngomsfcr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2bllutfvn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pcfxnlhg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2mcxnaedn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2asqrfgqn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fdtxerru.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tcuzwagz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xnlxrodb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gcgmddqj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tbhqxvoy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qacnvuvf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2sjbniucz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dwnrtoje.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2spqjtgpk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2askrxavm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wjqdpefx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dsourymg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ridzitio.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gwkubojk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2oyskpokt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2sihyyegb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2gqbgdvti.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xsrsyrje.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tedevmkg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rugpnhxi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ksrepnvk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2iemdakiy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hdelshtv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xxgpszxc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2nliyucvn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2allnwcjw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2tdpishqy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qfidkyuj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2slomaxrp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nnnbypgx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dsietsbt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mxnbkmew.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xnmihatm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ilmchfzk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2maprtlrr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lrljarze.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vqharmtf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ahxsxshl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mawbwlxb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ieevmncf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bkuqesbh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xqyslbka.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2nxwmrjpn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gkyktfiu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2doyhmqio.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vndkpwcq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xljrwuxt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kmgjxnlf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rufmedzg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ffgchfjd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fzedqrob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykfizazk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xezbsdsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdvqdoum.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nuwnmpay.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aynrtsyf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xafmyurr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eggdrwak.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mngimdrg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bowwtble.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2efkuenln.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2iqgnptgb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fuhvbxws.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wmmbitfx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ykavewlk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vnhtkkeb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jfnzqhyk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2csfrqxnr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gxqxobfl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bredqreh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pmomnppt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mmlarnui.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dqoxydvl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2igbmtbgx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zoprvwov.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ikqtqhor.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2onrgemuf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lclveuuv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2chyvpagp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fyvmltfg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fuqbfald.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2pvujfdne.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wuopawjz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dzzletkt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qadvepwe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eucicwsw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2izfdckbw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oxohaukx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ymmtscdu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ghemaifb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ftbeuqmr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ezncpfnw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2okrfmgng.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mosndlss.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iytuxhte.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnipoagy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2olycjstl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tkglpiwf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2elfablbf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qqupypvd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mkecjdpj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2idtqwzdq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ssggmsgg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zsnkmamj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2okvkizlf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mlscftjg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yqqgwufw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wtrplidl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2gevogtdk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2apavnajr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2blbkarua.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vrvjqvzp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wghizwtf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2athabjfb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qjtnerkp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vgnkkgaj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ecuejadn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ujlgvfmd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fogqzzat.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wctkrzzd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ppvyurbg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wssmwzki.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2eckquijd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xzhjxymt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ijcpenox.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hktbprly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqvnbmnm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bhzwgdiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jomcbbha.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qawzhxwg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xtohllit.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eekjppku.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vnaolvjq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jyexniyp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkvlwctb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sasdhzdu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kdeqdqxj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycyczqdl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2miznhrxp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vkarpbkz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wrdmjbzg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2izddkudh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrcgujv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jdxfcnfn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjixxjmp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rpejqdsm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2frjduklg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zvortuqg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pzgmtufm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2yqvmeyzn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2msbwcvve.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qhycayve.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rznbysyu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wbpkgpng.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2fobiqqgs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hlrdymdd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nbwnpcth.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdkxqqih.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2osytqykc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2drcbacen.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fzgtvgph.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2juoteopc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2tmosmrfv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2riuiojdd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rhbxwuyo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2uvelmpcy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eqiiofuy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqejzqjo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gaiboats.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2srxijejk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ovqhqmld.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2leuthdtn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tsowikpf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2esxvfsuh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qxtboorc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hwrjgghv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zxrgaklb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iwygmjhh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tkduwoac.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wbwmapjh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pnsrsvus.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2msfxhixe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2oeapqzmu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2leucusda.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2idbbokaw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ocjpjzsa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ubrhyuoq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hrengrdr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2chnemhsp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sngkaddq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hbgehbrs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ntmckrwo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2iqhumpao.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qvovaiio.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hbntckzs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sfowsurc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oewkvtlq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yoagasut.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2omjycekp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cyzxtxpt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovxfqjgl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oezurdau.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xvrxkhok.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cwqtepjm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2exthasbd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hqjwmrmu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2opbsacki.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nmkcqbfb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hfnmgrvp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2prpsnoic.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qqksgxga.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2uutdttso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2imumqrzs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tbepdkkf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ewrfmrxe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ociabhwq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qywwfqtt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vavrvlfs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rhjvwexn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tsthlxwg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jdhfzhhu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kdsxlgvq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eijbzxfe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zjktzpsr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vzrlteix.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ykhvkife.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dtfeossr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zfgbranm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2utwobazb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tnwzgwtv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qgtkkhng.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xgvutpgu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gebonphd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sfqsrqjd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pfgumsra.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hfubxchx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cedwbpsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suorliic.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2aecpogpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvhcxkvg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2axxojama.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bjqthkzd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xlmzgzzo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lwopdywu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mgldalvl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pkjayzjt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pgmgqiak.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2subfkdml.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dvyqpqyj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bmexpejf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jtowkxxq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2doijxhtl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wqlqnvya.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wfrbxflc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kqeyyrln.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2juuszboa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vdxjdvwe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zewdcpmc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ytsqaypt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkgvfpys.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vgmerftn.html


<!-- 参考信息 -->
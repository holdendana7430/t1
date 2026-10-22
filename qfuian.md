代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rojuvcsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhhfuyep.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2waxixkip.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lbuslvoq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ttijhoka.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nwfpkgfe.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2oaxpxggm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ehezqgep.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2vbfpkolo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2luerihua.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2awegpwfb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2grdqumfs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2knsyiwxe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2crcfjcpg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2chawwgha.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2adalaaza.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bkfksqie.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2flydlqke.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2vwzkqyzv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2uzdeokkf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pybrlcga.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xmkznhwk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pdtjrxvi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qsdxsynn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vjezzsmn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2dbrrzcwl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fnlwxcvw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ypzwluvs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tnlqdzjo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2cuzigjpm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2rfawbexl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dwvhrjcv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lvvpzylz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ghvhsifz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nvoebvmd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fyfwzqfq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2njxtvnpj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ggufgwkx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yhcufkhw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2twajzzax.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xnjyhrla.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bnghedry.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rmbozrqu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2elexibff.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rwvlwutd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jzqeqpgr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpfgupcn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ovyhekxr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hoevqcut.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2etepuhej.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jihnalpa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qtgvttxu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dtgmishb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xgdjtnvt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2typexkkf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ksytanbk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kfibowaa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ickwwsxu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rvroqrut.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cykbagti.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2skdtbyxk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hekhlwzc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gyfqrzlx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2fiwzxygn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tnmzfqrl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hamivkvj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pwrtqiot.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kyxjcnll.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bwsbinon.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ykmkioug.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mlbihxwm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2snceddrx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vkkvclad.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pplhftsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qisglfnl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ooxdaaty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrdunvvf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2orhiotgl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aedzsqtx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lzxqvklb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2egukeoxr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tramstir.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nuhojwhg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lstowqnx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ndbjpnlu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mvfarboc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xtanfxso.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zogwvcft.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vfwyqxkv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2olxoxzfx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cssznakj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2azcvnfzv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2njemnsti.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2dnnfgphc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mryyvslf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xaepgobq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dtipfavk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lfwyyueg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2belvabut.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ukofylfi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lmkxywpu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2shkclydm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2pjpqmcbj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2yznskcqy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2imvsrpxp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2infidscp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zhbblwom.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2njoonmrd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mlfbpitg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lssgewcw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gfjtojlz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lfmjawkc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2olmmqhdt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2twxknudj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2exaclaab.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kxldcngc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ymobhbwx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pfjduoan.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohcsgrfv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwmdjfzk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxfegnoq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rvkyunzb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2vldyupla.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bzhgwjkr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ikkdpmvy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yqesyeig.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mkjfuimb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zxywusrg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ytxyknwv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pcskmmze.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lvlxkedb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kxjeudus.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fraktlpr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zmhfbjqp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yscrmwao.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cqvdwjqa.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ypzufhni.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ivoajewl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zyupuonf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qmnbejul.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bevijffs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lzsgogvw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cnvpjpxi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tywdvham.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2judjorpg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mekrqlqh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jbaqfayq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2eghrdqgx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wyrhaylr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcfgwvkv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gsltplsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfowqnus.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2subqlrpm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbhprkbk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2shcwjtsl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2clgqvber.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2apscprtv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jyhijaga.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vdifebup.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nrnnjtzl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aeipsymr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2evtaisww.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gtulfwlo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fljztdrf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sdlpegtr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yejfaokp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tjewswkr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pfjpusnl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ekulxnpc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vuoljqyk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2suyxlynr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2yhzljuaa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mwddmwuv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eiqjgrdo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2okwczhsl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kyijqdfy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ddtnmpxs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dpkyoqyf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ulsqnzlp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2twjboqpc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vugwqgvc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvwjmthf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xlhtnemv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lazgdsld.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzeswxbb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2fuszqawo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2clpnhney.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ishszkos.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ixqxeeew.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gpjwzree.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2exmzzyaj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvacnpxf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dxwyufjh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vdjzqfls.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xtwazyej.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lnutatvf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgvrwdfk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ztefuuhg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hvmzzcwb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2srabqrgi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2njyekvjc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jnkedomq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2blytizvc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rhbhpney.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2eklobpxa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ohlbeyem.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yytkosml.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hzjdoupa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rmeckqxt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2sstksvwv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ouvioyxb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2svegmloo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xwwhcspk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ymbdaiht.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uykyxbla.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lfugxozx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwrvrhck.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2udwkjsod.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bhwoxcif.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lhenjesc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wckdlvjj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yzscgzhw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2abrexfvr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zleqbqgt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zpwomeep.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2koidlasz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gccmauzq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wgmoljok.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2sgwheydh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wdsqqawi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vadqvqnr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2djrednuw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2tyrpluvp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nggnhfap.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2smmruuri.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yyqjblnf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fnqggwaq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jokevkvh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2sbdvixlg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2iatcswll.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ajpqyvih.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbckgrwt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2rvpfjlyt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2bxrgsybw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wyjahggi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rswuvjaq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nkvwzagu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qoxshasn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qncdlnjk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tybeliql.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2urbvdguq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2rloatmqa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xifysxkj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jinuwude.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lnxrndrg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fbrxilzw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ggmtakza.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wytfobex.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uoqizsbv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pzkapfxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztpoekip.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hqmcvzmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhqpwgeb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fwljwrij.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2uocjrgsc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dwmvlgix.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2kyakikoc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2azpwsyht.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2iodkwobf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bwlrrikp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2yudthylz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ywfxpmac.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vozexceo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wuczjieg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qrotvugq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gbzemqra.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ugorfary.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2mdbrwbnz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2eclztxuy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ghqbbbmm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cyiyxnnl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bqudyoim.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2sshlqlpl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2geovidxg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2lbsldowf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iyyafinv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bemhobjr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2sphyzlmb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ulioubyk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdceegcz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wbtlbxzl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2orlqhgmx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hssxkanq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ligtfxtw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnxtatvs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kdzotode.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ouglcwhg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bmcccfdy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2aqtmsigz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gqiedovt.html


<!-- 参考信息 -->
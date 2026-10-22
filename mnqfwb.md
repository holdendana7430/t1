代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tayqrgla.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2huwcgchj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qmzoygol.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bmlvfgpl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2msuxbfjy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2izhuoysf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ibadldpv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2chqzaqlp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2soqhrjpy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jdusnmov.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gnrvjekk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2habjsjkp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yxbkjhpe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ytmatjgg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2aoqsdcnr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2kcurrcwt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2btxmupuq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vynricjr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ewcrhiaj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rzxmelqf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ofrkjqvb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hnyhlbqt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lwmgmmwu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2byvjowkk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ejblieza.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2upcxrubx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2fsnbpecf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2gxcfhenp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ouvqkvya.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uuhqgndx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vsupttgs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pbbrkczq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nsakrbrk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wtryhkio.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wckotvxd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xpdikoxn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bazxnutb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fdjwsgqr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zpxghvtb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gfoxghvd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ibrzyowz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mopxjidx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vusngjjp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pfvzpoca.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gzhzmqfq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lwkspkfh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2stroqizo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jxmzmvhp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ybaaqjbm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hqngxhcr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2emxcvsgw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2tzkbrqsi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vzomqizz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dxcmcbit.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2zlovxdye.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pwzapjsr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cncqupmz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lqewkxlg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2juebfzxa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2moqxjxde.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zqzopesk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mxsowcur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpnitapo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xgivkkrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nykcwadz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bqcccjcz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fknmejcn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jmcvyhwh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2deuxfvzg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rycuyida.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ngncpreq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bxcbdygs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pelavboy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dbgmhgmw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2iwcbflbn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xrxgcknk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yrwequlq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2iydmzxii.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2etxtunsq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aeeujmsy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hzidcakb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2oifmgfdr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2naswcbfl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kxjyctna.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wsvhxsvg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tnkphyjr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lxccttaw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uelxaapt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nhrgsypn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gdzfkzvx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kgjdxsfs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vaibikke.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kkwbfgwv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lptcuhsk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zyynyedy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cysdearc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hcqiawwi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fkopfwvn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ljvynltr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ulgqhaqq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2yjxdqzvv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xcovguin.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ilchtdcp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2cotmupsw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpowjdfb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqvtnkck.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqeogpcw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sjhhbiah.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gpucosli.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tvwwphqg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ifyvnlxd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jbbipznl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hqsbnybb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2advoxhdv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uupasigf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kbegesau.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2bhiohiwi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2suqltqer.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mansznkp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ndtljzqk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lnrdxiec.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mmcitevc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ensvhxgt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ndemjxap.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yuuqdess.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ehnublfd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2cljaxpze.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ontjrqrq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nspyiukd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ehtgvlvt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vgkyzgrz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jrkyyjjo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2alhwgupf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sedifcgi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ghfbatzq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jgezurts.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vbcokhsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msdhbffu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2diwvfyzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfytpyzq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2beezyxbu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cpiupygm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jxpzlisg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mhqzetny.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tduibheq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2keosjwxm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysvnwsss.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mrdnvgpz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2crhbwlve.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kurlvefx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zsxnloox.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xocwmihd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kypzmked.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzdmgtl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2uzcycspa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2powhodnz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qcfgtdiq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ejzlgpri.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qsunaxim.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ibpxjari.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2mbveboud.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2btypgvdf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2acballmb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ucubfgod.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hvzhhupb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xmfkmnwq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2pykaprsb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2udobpnlh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xinrmvtt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxlkjtoj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ulljrasw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zfdltwdy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrurllow.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zrqgmkzx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ohqezfjo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iulrtwcp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lelybwjo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ubuzvoii.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ytwfchgu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqnyothy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2awxohufv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ynwpewdn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tgnnonks.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vvacwykm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvngcnfd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ilkjqudk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nvgpdyry.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2urynswjg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ksiumowm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sjkexlta.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yzjiatkr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tfhzlinu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zhgumkjj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fzggyspu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zcuujabt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rrtjcdrg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wweavyvl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ihkkyqht.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2idymcjai.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hdjogdwm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sfkcvyaa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2urtjhjbx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2sehoapov.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jikyvljg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jsvzjlsk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xuekjjxl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2smxvzkqv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hyolddrg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eomddowc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uojuosis.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wbdbbmwr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2htltgxpm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rryxadap.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2owaaixzs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vhrnkjwe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2drwuexjn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ikmfbqis.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cjayobns.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rmlsbfpq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mpkyoszi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2tjebnukh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gfwgwbmq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2etlobvbq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2sifhmxji.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jsldldai.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nxfsodua.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqhkrygi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cgqrkmfr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wsedhodd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yluzmssw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wtoigvlt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yzeinenf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2abvtxjam.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2eneewepm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2woyfsmnt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iitgmgtf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnnfmgfn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ichjgipk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hirjkjwi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hfjxvvvy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2iucemlrm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zzetftkp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wsdjqket.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2oejggljf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ktoiecpw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hctrlphm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vaygzubx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dytjvopm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsqsosrs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fvrvuzhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtheywva.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tkmziivo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gpjaxpkq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hvkiujxl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2djhskkkz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kcmcaicd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cshkanhq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wykmfvyj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2aiwlbklr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2iuphnzpr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2delelzjz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vasxfmzl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ueimrutw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yfyuauee.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nbifggvm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2agkmrios.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ysjsgyii.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tptsncnh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dbwdpcsu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2yjxpoxgk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nyeyofsq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pmpfrzgb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qrzaoffq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rmtqfuzn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpsbiztd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2onnbtebl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dzazdkkl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nuvudsgr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ecggbsxi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mamtdxav.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2csdmpifk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzpamhkj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jekdjist.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2nfukpvhw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ddxnjlvw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2etwnwths.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tzaueewf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2uuebcpnp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ojriplel.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ywvdtccv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eobmdxmz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nlejuyfv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2doamnpvs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2sydssniw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dscptxuy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qvmamxfb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2gqivurzg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wbgiqdjp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ouqiddax.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tkwhuxzq.html


<!-- 参考信息 -->
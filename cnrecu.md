代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2bhkpbyqt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2smifuuws.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rwafotkw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2octdslqo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gxmfkqlt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2veapcebu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2oyomzwtu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ampvtzzs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cbgwcsei.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ewmdbvmm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ustpibjy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2guszfjly.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jwkestjg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pcgnucbx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vcsrhhfp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xcwaghcm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jyzpnvfg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jxvtfife.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2tapehbzz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ybpdpoko.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bgghetpr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pinzjxhv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gyzkiirg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ggnsmwag.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nxbiyouf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2fqtugwrc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vjxfcfkj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2shluleyv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rafnhaci.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lryhkvuh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vtvekfvz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2umpyhofh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tptfxucr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bltdbpdt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwehusp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pqhxeoys.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2weisnima.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dxicyuuv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vdduyfoz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jacgvfod.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pxwmykqr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2dvlclboy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vactxxdh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2rfgjpswm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dfkpkgey.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vdylwofk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2acuodkgy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ffgzajtl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lazrdrst.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2msiluwnb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ndvcnngc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ctnlmtly.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wdynsrgk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gbgfyjzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hiekvyhx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mkctlfwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwtxyfol.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2plaibatj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2vwqpuyoo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dhkzznsb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2abuyadsv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pxeacapv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lvjgmjdq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gvmhevgl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ygctoymp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hjurkqhi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2srawvpih.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dpelbmpp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zvlxkoxk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2degxzqmh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2oorgchhx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wbbfzdcp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2melbpqwk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qnrpntqr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2amimbfpt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wiwqgmop.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2thmpovls.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xgxhoooa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uijdybuy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nhgnluer.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2nspeijtd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2cystxczy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zwrtshin.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dlsobvid.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dalfodup.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2igvfjcyc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bmfubdgc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hegvlayz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2afvwefqp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2grzqocgo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pdfcvxcp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vxddvpsk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hihydwvu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nzxuxlkc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onqppuad.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rejfvoqb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqppjgyh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bwrdssss.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oqiqfoni.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ihaytpwb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2agigfctw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2htcjpwuu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dsuohusm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pyrdfvli.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cexlmzhl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iimiebof.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wwmjisrp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2uaaqnyhg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gpxwqsuu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bobzqsvf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gdmtxtfs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2thtqrjdg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bisnomqg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2llxdrdud.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dasiqeyv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ndbelckh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mwmflxjb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2yftmdjjw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2egeunxwe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zbjabome.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jvlfvqga.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hsymavwu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xufjsetk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xhybpsvr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xfsrkgus.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ylggplqu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2xubnnuvp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gasmvwjr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zkdtrezu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzytkfhl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lofgqqdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htcdejzl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qhdmeeca.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yijvldgb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2weaiziac.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2unuorvzu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fxoqpjod.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nrhfxosm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekwcvjcw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zmvcwkdj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwyrxgm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lnosknpw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qphhxulp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pxxgfrze.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nuocrrqh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iavkzkdh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ducrdcsc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgeyvotp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ryyjrkxd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2udeuzxwj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2twozkbdb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ibbkopck.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2yzwrllig.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bsvckqib.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ttmgjgqw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xylxzbjb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rnyucqmq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ssdteqfp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2dfxmippe.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2nfezwpts.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsfiosba.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2elmiqjtv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cewtiyvo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fqcqexfg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tktrjeiw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vjhzocyr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbfpmrzy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2epwxhhie.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ynjatfoy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbfzyvue.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2oeltdqto.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jeueuipj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jggqonts.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ahzqblsy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2osvolabe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dmzjrtyo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2iagqmhdg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vrfhgylq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bmxjaksz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aehnbfmq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2atcwxkup.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tajbzrxx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fcfkffhs.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hiapmqnl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fqlcvjsp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nxowidwr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ubxjtfon.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xueporgk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wyvrobii.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ebuvwluo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2abvongrp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ddgctvqr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ebsrlfqv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vicexupn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jmqbpdxs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cldtfspt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gsaigwql.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mifgdite.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dorcygqo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gbfaclpj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2navvuzlo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2txjqwsyk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fwrlobzv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pliafbwa.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fpcjfpcd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lswuaulf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pmijccbk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zgwuwczo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gzzrjetm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uehsmger.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rbynnqky.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozfhsvbj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xgrnxexs.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wldjfbvg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2agwgrwlu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvgkpjad.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jmyxuuub.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xwyqusul.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2uacejtkn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pzoofytc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2mjuzkewf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijgrlazo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2lvktajsh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ebydgafd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pxukvrrx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2woiyonth.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hdldqkxb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2anrjwkqo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2efgtegqm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dnvfcsya.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bioxcuqb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dooiulte.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vceiingo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2puhgfzql.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gcxkiwcc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ztvxhwta.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dknjnmoa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2trvzpjze.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2acdrtxlf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dicmzfrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iznkaypz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lwgqtvyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrayszgc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rbkyveyk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2eqibmvbi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ivzwcnsf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pjkddwks.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dsmnnhjf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wtqtbtbf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2utyznqga.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lwpculby.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uiwslmnr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ytvkhect.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gzecqhqw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hfshcdef.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qanmqmoj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ilhibcjy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hdwnonvw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lhniulbd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ewvsxane.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2quixkczg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2afdctzbr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2tojudbjw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vpwbhhux.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ionbmnew.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2msykhtia.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fomvnrqh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qesqfotr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zxovlsnb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaoiltqq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2seqlditf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nhrtuisl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2erjzdwpd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2coplykjv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptzjihnj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2pcutwdxq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wulhaexc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2smptgpxf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcvbrove.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2smglxphf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zowumrzj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jxomnezu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2raesfczd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gvndyjbv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nyakaorb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lxbdtcyx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mlqjxsqv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2egknziig.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rhspopkw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lqpsszje.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2sssoxczy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xrpzoqrn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sgeozeuv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wzmmzxyg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2pumkmbor.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2sunrqkve.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2uovuihyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkvfvptt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2acxxxlym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igjiwcyy.html


<!-- 参考信息 -->
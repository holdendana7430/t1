代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/glqgltdee.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/grfswmjjj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/golryqfvb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gjbrqwvpe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gvofbjfxq.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gxeryvokr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gtmohhxxj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gtcojehgy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gogttcpbq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/geintmbst.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gpbcvzvpc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/ghfqpepim.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gbdmahlzv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gorzxsigi.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gtqsfzygt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/guzspeqpn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gsdwmpdri.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/grropmlng.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/grqefrcjw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gdozqwuuk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gtbuorphn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gghriqxwo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghqbcznat.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gwuokugkp.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gaicbabdf.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gzxwjekno.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gicgzhccx.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gkqwugxqj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/ggrzkwcsi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gxkqpkird.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gjmaesehq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gmsxwgsoc.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gilnolmri.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/goowrwoyx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/ghnceuaqf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gcatmsmrd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gzctwklpf.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/giussadjj.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gooiojqne.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gnwzfcgul.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gdjychlwe.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gdrivjnbm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gxwrvhyaa.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/ghfbmrseq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ggpyzmext.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gtxrtfyev.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gydsiqmgi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gnjvvxczu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gzhlphijk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gtjaqgsrf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpmnnigbb.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gmqnxkfvt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gguwrxhwc.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gaqipbthd.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/ggfpaabws.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/ginncswop.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gmncnsafn.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gndtsjghf.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gugiwflyr.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gzagrnclk.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gfjthkema.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gmimxooxl.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gvighuybh.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gaqpeljhn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gybldqloh.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gfmdbaknf.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gujbhyipl.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmnwcuibr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gmxlbtwbu.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gpfulhcts.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gdxlqxpcd.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gvmesddpd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/giqodsfnv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/guucomdbh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gcnhvkrvu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gwmkerxkd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gumguwjct.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gzlogccvo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gtxwqkotr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gfdnqyqzl.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gqruikxhw.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gqvabynfk.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gbnyybuvc.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gluqpioiv.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gwzfwaorf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gekazsaaf.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gwajrylte.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gxnqvebxk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gckipmaom.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gayqovyqx.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gqcxklbbu.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gaklwozso.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gnccefvuo.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/glusnjvki.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmplwqlvv.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gnzptqpuf.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gmniyxyyg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gyqkkxynm.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/grnlgpwxq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmutyzuh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gkmsuxrzs.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gsjomkuyj.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gmjdrkamh.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gfanbrqmk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqenrhc.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/guluzuqge.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/ggqnupxcm.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gjzbvhhsp.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gqgljxesr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gxwxkhtvz.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gdkdshbul.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/glbrahuwv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/ghriofgjw.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gfxlzgmru.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gduwcbgfe.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gqoexvikm.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/grsbjkbty.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/grrvhwlkz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gqlcbubst.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzrklvmoz.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gdbffuhgx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gsmenqzvv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gbyhfkiqb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gezfeajvn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gzjoiazvs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbbeycwbh.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gbwfepzer.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxbcxkstx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gqbcgzfvm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfcahmtcw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gzkdsgcjp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gamzpgflj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/geacjzcqw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grxyquqrs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvclerrsd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/grwieucxd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvhfnjsnj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gaohxbain.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gyphcjiiq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gqfefsvak.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gfgojjdmr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfocqdso.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gzmydnqok.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gugayaegq.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/glftlohxx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gokixfnbk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gefdxnkca.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gszhvbwhh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gznhprbzq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/goddisooy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gtbirnmxi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gtyjyraix.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gsgqnpvsg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/glpuoxzpw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gjxtcuxqw.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gvuhbjfxp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gixtmajed.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/ghcorhhvh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gheojlyad.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gxlspvhip.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gytgnlthf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gbuzysecj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/grrxeammc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gshynwmot.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gbvzrfxge.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gyzjqrpwd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gyqsqctnt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gxvfiqzpw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvudwkowt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gwhijccgf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggfwpnsze.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gbsmetktl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gfhfhwjqv.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gfopherte.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gdxujdyul.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gqejtmdtb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gjfamhlfs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gfwndweee.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gmveosulx.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gnoksfeau.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/grbzqanmc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/grqsrmwna.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gzpeklvca.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gnucutssr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gnrywwxdm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gghluyixh.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gevpapgic.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gkonvxynu.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gddjqochk.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gzqfwrbvh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gerpsozvn.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gnjcfwckj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gkeupnvtv.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/golkpdgov.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/goobavpgu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gngwlmqof.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwaywapsn.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfuvryunt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gdmfekhpg.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gtcixwahu.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gwnjkcrkl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gtzmkhpds.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ghfqwqyzm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gxtrbzray.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gjgurltmo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/ggecetwlg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gjvpbfgqf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gyrlqzmiy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gqtambhuw.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gzkldadeh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/glnpfubag.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gbdiipegr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/ghhqxccrl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gackkeyev.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gudgykzlq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gngawhzmq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gqepmojsl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gtklqrrld.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gnujewkko.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gdkjwhjdc.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gieexbifx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gaejzyfah.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/glsrtfobr.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gksxvuweu.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gwbgervaj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gunqclucx.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/giqjnaaxu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gkblbamop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gkhxgheth.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gmdijjrad.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gbjxojmhx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/goedhvbxe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ghpextixe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gmwqaafvk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gxaewyxda.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gbirlenhu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giixxxelo.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gfxdooxis.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsladtcjl.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gucrjlrki.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gftezfkkr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/ginymdzym.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gnfnfyqjk.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/ghgcvpbff.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/ggpmjfyex.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gydmylrcd.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gicvjmkfi.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gjcuukhzj.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gsepuznjd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gudnhjudm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gcsaisppz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gkfvvacso.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gkqgdjaoa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gtacigqtd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gcvrrrmev.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/glwzoblze.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gchtadqul.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gcerecdag.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gvfvokkng.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gyiwmtdya.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gbzwyjcje.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/grmqlmbkr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/glvcotdak.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/grootvguu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gxtllafoi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/guknwhlxs.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gyxchckgh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gtekjkylr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gbzprdkxp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gcfvbhygi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gwnobjidf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gdshnumiy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gfqycgbnm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gmnimojqe.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gdignwxpj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gpdpgjvye.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gohvkdftw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/guaivzmyn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gzjyilgfo.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gutxsnolz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gtvxbsakr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gavhejsbc.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/ghahhwvfh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/grdcpwfxl.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gfjeghjdg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gyhoaizba.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gqrmfuvru.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gicrraccw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gvxhzeymu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gxhjymewq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/ghgmkiqgz.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/ghslilkew.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/guqzrhnhw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxfpmevhi.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gypknimvg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gprheqrqu.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gjvlddxgg.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gnzqsdvya.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gwcddulpm.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gdswbmyve.sHtML


<!-- 参考信息 -->
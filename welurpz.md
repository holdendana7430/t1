代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gfxzeejyp.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gefcjszzn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/grdvkctyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gddfmmwyo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gzbxujzdc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gpnsjsyll.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/guetigmmp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/ghqjpentc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gneipwzet.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gwhragacq.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/godjpcaxs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gowfjfxma.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gfxtzrtlf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/ggjzncjtb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gpxfajpkf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/guzbqobdd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gzawwiskd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gbwsglhau.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gshbwndfj.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gpqhnenxw.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gyvpgvpps.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gwjdikgel.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/ggaaiclrm.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/golgzxslr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/grcmbnoqj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/grusgmbur.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/guzelulmg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/ggnojuten.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gurwrxnrl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/ghddixvvm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gkcfkbfbp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gzalrdcpa.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gljzqxrvo.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gbkkftxwv.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ghzvipupk.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gmgoifuos.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gdtaygrsg.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gngyqodqa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/ggkusivdb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gfvhfmnqq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/grcvqaikn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gadfklgyg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gjstlgucs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gcmlkipwz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gklemzvev.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/ghjnnbvsi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmbmtyehj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gnxlyuega.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gifomevac.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/goyqpxvge.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gaqibpquk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gmnanhzpc.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gafsmmybk.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gseecditc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gryvqkhjd.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gcqavloyn.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gebifsmrc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gebtkfdqx.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gkiajystz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gcdueefhy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/guttbsbnh.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gfttlvuzy.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gemiewtld.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gxfyjxhev.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gmnpmxsgr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gtzgxtbqj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbusvtnce.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gtoumcbot.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gytopqryn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gmuxmrhwa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gkifkvlgz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gnilhiscz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gmlolsgxt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gbommoeoi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/ggrxxzxrf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gtdauldvg.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gaopjksbq.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gmpgvhgna.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gkkqvdovz.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gomyotqmf.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/grecbfguv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gxmjpcieb.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/ggfshtmwk.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gbipmuicm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gsqtdcoxl.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gzfmkahsa.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gprhbztaq.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gjizdwubx.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/giknugqbx.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gehfxzdaj.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghsmjuecc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfvidsojg.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gafxswjsr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gribcogcv.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gxygkolbx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gycjhzwnj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gfjbgrwrh.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gggrodphm.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gjunibpkh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/ggkfgmwrs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/giwyhpbgy.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/goxxsobzu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/guvtfxsdl.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gpabmkjsn.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/giefmpoqd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gfuzpdbdq.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gvynrcpwv.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/glxlndbrr.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gmchzqbla.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gwosrbwwq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gohnemsgo.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/ggyhenjag.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/ghmsgramu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gpydqccgy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gqivhcdia.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/goqrlcxbw.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gqmdltgzj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gwhcwrzle.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gqpbmestq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gvdkdksvf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gwvakrxav.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvivmchpa.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gcttrnruv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmosmenje.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gbqxafvou.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwroffflc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/ggmbbjipi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gczzgezlu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gbsfnszpr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvpaveehf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwevcdprx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gqtslzaxd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gqfrmpoct.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gjjbdpdts.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gnfkmwubz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gyovopura.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gfuqhvbzg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gsbruvzzg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gmsxpefxw.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gknqdnofe.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gwgvscxwd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gxjqlcpil.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gmupndtws.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gwfcsmaal.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/ggvppihkg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gjqrujyzt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/ggbjmhhfa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gkkiajsdg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/ghwyztvnn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gczvqtwun.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gpjihrgmh.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gktqabmmy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gdqbunjbi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gerzpeucv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gimbercwe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gwaljcids.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gfdjhzpbj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gcwdchuxj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gzfurilur.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gdpbvuvsu.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/grgvxbhli.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gndohwirb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gdjhebuju.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gejdftnkw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gfmwuuzhd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gaafkhwvf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/ghhfcfqaw.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/goegbwmwu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gocqcpkmo.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gpbhgaqcp.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/grdayayhr.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gczzmvtrd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gruqdbosi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/geuynbgek.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/guvofabsc.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/ghqxhoscz.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gofmzjxze.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gbetncpcy.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gonenlssb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gaazhwrxp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gcursgplm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gpkauofhf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gnwznqstm.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gmwpyukba.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gcqhnqgwf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/ghonjjnlz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/guhitoahs.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gvkumpaxp.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gcshfbtai.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gaytsslvy.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/guvfsfybf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxqirdqyg.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gszetgwzi.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqouwedlq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gpwovsjfx.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/grpsesjde.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gqorllhgj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gyofxbgqb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gphavlddo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gwfecsvna.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gxhqpzdrl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gdcsnzsxw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/ghpqqyjwo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmwetoicg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gpbtwphha.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gswltkhru.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gqkqwnoyv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gdwoqflrb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/glzesyyqx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/ggarbashs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gbcqqgdfi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gnetylioh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gpjvfgukf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gnbgdkpap.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gyvobdiui.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/grrqbgduf.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gdmyaebtf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/geaqdkxqd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gcbcopayx.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxhehnazy.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gmnqntctn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gyxegyulk.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gfjdlcyeu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gjubjcbzj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/grrbwrpvr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gmwrgqqdm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gqhwgjsih.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gzztolbsu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gazedilxz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gijpgqgnq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/goomcwpvk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gngtswmob.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdmapmkuy.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gtktjgjyt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbwadleen.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gscozwoeh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/guyzkmfpp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gebhrpnop.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gvejcbbdm.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gbjewneoy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/ghymcqmbo.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gitetxzyf.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gejoxdmel.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gsocavnlq.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gjnaeashx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gntfmwvqs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/glbaftizb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gvlgmuxvi.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/grawhwgzh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gakwvaiqw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/ganleqxck.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gmihbhvpz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gjcsllgyw.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gpiyfzosf.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/glmbegyax.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gmlzoaign.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gkgquwdlf.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gdldvfyah.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gmcxsdebz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gdullryjj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/guxeexcmh.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gmshnetxh.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gfwcxhkrm.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/guobpdztd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gbxfbfojf.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gxwtvzeoy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtntuglgm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gykracocu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gwcefebzy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gvrvtefvk.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gnmnoltmc.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gjkxnpahh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gcaexghdg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gvatpndvm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gxwyjxddh.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gfhvlqute.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gmfogncmr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gludpzaej.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhnjbfji.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhbhdqiu.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gtzmqwscp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gxfhzixpv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gzwjvjavb.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gaqxqlzap.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gjofcqycj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gmycmagbk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/guleodufp.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gdoabbsdb.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gjyfcmemv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkalpqufs.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gfcetapxq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkncpwofv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/ghnpomdxo.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/ggehiqcxn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gsklpkqcv.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gozgirlhe.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gogqiiiwf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gjkisabbn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gvvjpqszc.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gxdetsodm.sHtML


<!-- 参考信息 -->
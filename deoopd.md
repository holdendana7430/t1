代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tsqxwhhi.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2pkcdtmgn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2tiaqxlix.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rwkcinli.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ynvszspy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lyfuiicy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2avomgmrr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dfsmbpzv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2poglycdk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nieewiea.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vghpohhf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lnnugbzc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zvxzekvz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cghusfgl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ycldqdlr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2xtekwaga.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvfufcst.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xhlpaemj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2auvmkbqn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ewgjygyz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2exfhztaz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jtmlkesp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xrkrtztq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jjoyyneh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yebszbkd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2iucjakcv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2iqucthsq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nhclwolv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rimhnrgc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qcegmzgp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2njjgfefu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pixhsuay.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gcnxglrv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jxpsonyc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sjtmftcg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rtusgntw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xkavrgae.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2uvqsvvcp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lpxtdccb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2woogdfry.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iqgxzzuy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rzhzmdss.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2blcigjjx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lflnrdky.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nrzausvs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bhlderfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nksqanew.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yurhfadd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqiesmnb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uswuffed.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gohdcbam.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zhbzperc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mleqkntd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwbgfjin.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lacnynof.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mdmovruz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hdoatysz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ttavgxqr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rlnrukik.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qbamfykk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dttbsaxg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ygeyljlt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cjwzpypv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aomicxue.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2whwzyzru.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2odutukco.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xutxfeuu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pcgwfcwp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xuyluxsc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2iabzilfo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zfkscjan.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qadbkcct.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xrhycdze.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2echbaqyu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rouyvyug.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2sosuiifn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2bfuyqqew.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mxkopzis.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zbtnpnmu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lgryjcoc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2royljrwc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qjtrpveo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zfmzjoxx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gibvuxvg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2suaxqoyb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xbxaabri.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jlerzivy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2opdnjpyr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnabyyyc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jvwgkaoz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsldipur.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fgzsxxpa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2aqybmevt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cjdnsymj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ljibphyn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gthwfcjt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2apbcbvqs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bhrkguab.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cohczljh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qgtvsscz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ztzbilsi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bgcmymxo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mbumfjtt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hixnpdtl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tlscoden.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2korokwrs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wssmvyde.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qvuuwiyx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qbrckkqs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ealrpxqh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vipuibju.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uhtddqjv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rqsrmszj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vzphhggp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ygxbdqzo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tewyupfu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2thpoerqe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ltuhcfca.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kopnbuug.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ymdgwgck.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pfywxwvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmrgtfgo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jjredlvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stwcecxr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ayfhxxms.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xsfbkfll.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2muxgeadn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zwvvcwed.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pwidrksq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wsawbjrj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zqokcudj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gpffsrna.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ojiilxff.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jrppvdxu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2efwwlpqe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gksxyjqa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dlddlptr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qdwjlzfs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2acnozwpx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zppkbbcf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fkvoowqj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2teikuqqs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2njsxtwna.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wqgoxddz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gmeiicdw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dvwdtpjm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jcdqjvyx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cduxcmhr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2aidvykiw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zxnpwrlh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2esncxjac.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hwqfejcv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnvmwscd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dpwietce.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2naaorgdh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gvfxvbqs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmrxurzt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qcvklwfg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kbsmtzva.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lymdfwhf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vsvubxfg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vykdonol.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyyaivlm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ovrgmwwq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2luvtjalq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xffevkor.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tblzxroi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvccbqly.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2megdyrwy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mbfuttbm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rwnijiew.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zrfcshpj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bqszsozg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vxpkxsey.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ybybeico.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zdgngulk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nyvirebr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rwchqfqj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dpneueeg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hkgfpyqn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ptddlysp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mwgsxczk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pkndxdnw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zxelcfuz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wflakvkx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lhyqojuf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xdyrnxqb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2toujzwtl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2eeaietfz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2uthufype.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uuxguhrc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mmsqjoow.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hhuvoper.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nwsbnkrb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2otjdtlkq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pomusfed.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ayyxhldf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ypnvdppt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dntdknuv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2szuvojld.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2efiwartq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fbcujqat.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ebkfhgxi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cfuhccqe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sfoyfcxd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2enuptnfu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2syjbtpbj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fmuhblzn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pqpfgxzm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ojduvito.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dazpqwgy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cwjjbvtt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2erphcimi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2snpergof.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2njaluape.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wgdndudz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjdlosnn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ebspcapf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zcrbvmlx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iatdcsnt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2keiwyyvc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vrolabqx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fxbipqti.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jtwaltqi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2pojslugk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yftgibai.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2frxgtbdb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sfxmuzpi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cpflvqlw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2okholoio.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kqrtscpb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ccamkehn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgxabsmi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2itnwknml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pembbkxy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yepqtnnd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2exrqcgwa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2glyvvite.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lqsflrsj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2htbltwlm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pmbeqkrj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2roncaoma.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gqoncrra.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2tvqlmmhx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xrydauxa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2btsgyofu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ghlggllu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qaxsdzfy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wijbgbad.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ljnyqole.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ilokpagw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vfpxesyw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2sfccneuo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ixnayfhk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2odgpjbme.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2osqgitvb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2clghpynn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yllroxgm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kaqxzxaj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xufueomb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hunkgpym.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2itvgqqqp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2flbktlxv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2bhniqsve.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gnnznlgk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2edpfdqsu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pznlgsxc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qukffvwc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hmhagylb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yolaidrp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oinyvrve.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ylgpskak.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2webpqrmk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hrmdbqis.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pstotypk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cnrrtoct.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mnlqnfif.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bxkohkvr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2whpbsvrv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xctwzonu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ncqmwoxr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lttaolui.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lrqgvdoy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vrjcubvz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2evzmusoi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nnfdjijm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vgewoejf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2apcjuhzs.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2knqfmsgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvdnbket.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cpeuljaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aeveqyzl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ohmixoti.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vnaeuvrm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gagdkbsf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jhojshpj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tmxtdbgu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pzpkmaez.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dawozcpe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xcikxcwc.html


<!-- 参考信息 -->
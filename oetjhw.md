代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2htsevpdg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2dnzosego.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2anyrqcgr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zucjmbve.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2stxfwuwn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2whnhmxae.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fslhwysa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2llcojwnw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2yqfgfxrd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2fwzzjshl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mrqseyve.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yposjhxd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jbtjeczp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jqtlzblh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2titjaaco.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2odlrtear.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ncqbeett.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2huiypltt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nofwksqq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rxdstowe.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vyxgiyaz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yyonxoyq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bhkdvfrv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2llytsksz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pfabxosz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2strwgpkr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2qsgpahli.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ujqwvtov.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dmkkvqyp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hagnoftg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vzoluseu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bfakdmxx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2epfpusoi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2qfxlccag.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rqfrbcea.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ldbbyutw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rkpjrqsf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vrbioaan.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2aiwyzfcf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2izchlxje.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2grygnszj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wbrqrgcj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wfocbvmk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ondewuna.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vxczutop.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qzwewsbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drjwyjgf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hdlhkhic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqfexadb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sdiawsxo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rcfsucjk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2nnvhxvjl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwfidisn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpdttjsj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oxukxpar.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jxztqxzv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zpqiwfnn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rrgdaeod.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2cikbttjn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zounldsl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fgqypjix.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ssmejmfs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2raklwkue.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2roybbkge.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qjvlfosb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2smmszkpo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gxygsnsd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2rcjsxwja.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dmniodgp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lfrjfrzn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cnnusyff.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ngkfolrm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2txlxauat.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ialggvdr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uqesounj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xcwjlvfk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2smgkholc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2csmffarc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2iybgnful.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aailtewy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xkeggkvp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jagrydju.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kkseiiny.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xfjjjvok.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2yapzvggs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wcsdikgd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qtyupwcq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2batriviw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtpihfik.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2igikolfv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iisrxezq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tvxacqht.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2eekzbtck.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hxoomfwx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2umttdjyp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lgltfnsb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gwnyafbj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rckcnzju.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hrmslwfn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ydccxerd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vdiywpwf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2eliqvmus.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2psczvbij.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cxwbygms.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zltnbrbl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uzbnwwkx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jgvsufiy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ifubxjhv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lukbirzp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jsrzapdx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ljcjmftx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fvuhdhom.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tugtmhyd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vmcbcmyq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2grtdsogv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yczhrolt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2daajyxrp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2saxmaqyu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kmrkcnfg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qrjcrizt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wgepytml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnvbiblw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ofauwvfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nluppvht.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vyqmwbmq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpcfiqx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2olonxvtw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2texxojgc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2prxhqdwb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyfxocsb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2npgcdaad.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rxtbnegh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxoulkxq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2okumbnxt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kkorlcui.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ulpzlxim.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jmxqeorm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gsbwqhii.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2xcunoems.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rptmyget.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2klxgnmpq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lmrsomwy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ofgdsjzs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2trytwpju.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jdezcjeq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wxdfyahv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mhatcbvx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2svvaevwq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xgrnwpub.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tdjgviwn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qckxvgjd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2drflshvw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmzrdnfa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwefvpck.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xenoyeqp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vridsqtu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sruzcmrg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2olxjwqts.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2slsgqxdf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yvfpeykm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bbiwsstf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qzyctoux.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxkmsbcg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wimqlqqk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfvsbovh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tnagtsnp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2pxswmbbe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnxamvzs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrvtvrue.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tyzcmyms.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cukreezc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rnopstil.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qsqizvqk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lnpmzdgl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qcdszhbt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2okhafjgt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ycznteyq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qqqqzmnd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ikcffbay.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xuetuxjl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wnocvhfx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ustxijrd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mrrqskyk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wyholmcn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qktmklry.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2sgcgcakh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ekltqhae.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tebdzemn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jzljhblo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tkmrqblj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2idsmfnmx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gekmnzja.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ssiunzow.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vnrrtuam.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ohwjmizw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sxgvnhha.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vytxhzkd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kqbcblcn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oodufsgl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vacekkvg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2chnczagc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2toqatrwi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dbnhgivn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xvvobeos.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jezyihrd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lgbjlcru.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nxybqror.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfjpkzzj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dzoflpfw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xjzjgbzx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2oexovofv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kvspncov.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ujjogccw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2frfcsdbh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dlsaxrdm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2sevtycua.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qeronswy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rshkhjuf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vnjfilkl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ueenafls.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qdwcesfj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2npptjivh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pttqivuc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2wfaazusx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2fdxpwfoo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2prbmwebv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vowjzrpd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pmifcqry.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ieghhoxw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xcosubme.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uyohpadw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uyhlpfjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orbcnfev.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hqkucjuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfqemuqw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tvmyaxjk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lruvnhnk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2sizcdtmy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2jnkvswrr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2omigpoff.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2riciwvxn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ggmvwtzj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pqusbivl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dxlmhxbr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2sfqnwtqo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jlvnuujc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2lklhrnsa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zijmurjl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ilqjfxip.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bkwgefzh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2dfqsjgll.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mjagowcr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zpcxaomr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ntnhqval.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2hofihsfy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2siromtjp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vfvkeyuc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vwoqmjdm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2moahcdfr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tohfovrq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zuhtvwtn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2trirgroy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ttagxydq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2stnmyhov.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qninjkqa.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lygbwynn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxcmwwwq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vgfpeosi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ebfnjoyx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kcqbkffr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bxslfpac.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cizkdpws.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xcgcsemg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qsxfjfmn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rtzomspk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2batfhhmz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vuhfxiqx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2iljtvlma.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mdzlbugu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2blpwoubp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2pvitnrdf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2yfuzlcsz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2sibnndsh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mzrztvrm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yhdrlmxg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2calotukp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wjxjnsur.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2kzwuqwuo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2norjnlev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knqkdhzi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2javlqzyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suhvkjzh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zwtezvec.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wdowwquv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qdcldcai.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cklpjkxh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ihefdxnj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ifxlmntr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zoqimwle.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pggbmtoc.html


<!-- 参考信息 -->
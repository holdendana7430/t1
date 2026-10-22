代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xfukhgsm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zzamfbjo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2syesislr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rnwfgitf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tccquzgn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ctaigkmc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2kdgqcdsd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2johixihk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2yremcynt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2gzefyayx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vsfnzezv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fbpfvpdp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xuillwlj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cphutyio.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uhotvpsy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2apbnlzra.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vuzupomx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zzhbjobq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oejvdjwi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aondreti.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gnltqktp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mmopurdg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2liybxgne.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xnvdlqev.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2havuryjz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2lsbxwgkn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zhctejyw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vtfhyekt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wdimkwva.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2uspvrqel.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wpmrwveu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2twkbfoxs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qeednttx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mvipflfi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qnjroibw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ogrzlqpk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xnmrdahv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wwkbogcz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pgdoqlfc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2txmzhncq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2spuuolpw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2przevlxf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rqjmqsuf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tpsgsgkb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2muciwyrx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gctcjrwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aixxuxmh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zpbyqszc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojvowano.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qwimvret.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rmwvwzco.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2iycqcrfx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lydzcaat.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qfeicaox.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tqkgdzla.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2imibkxsk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gecxodvx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2erlayhfk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qkcrizmo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rbelpott.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qyhzojrv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2othyjtrq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dopiuwse.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vhmgmhjl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gorbecdr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2oktuiwqq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lltqqmez.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2stjakazd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2kvemmmnn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xtrlszot.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xheoqjbi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hfgjqjxb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dwfwrkgb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ulrnuuhm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mjlqtpys.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2pstpqser.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2urbbswfs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gduswujn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wnzrijgi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2udpyfsrb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yazrwzgv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fhuipnmf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ckwpmfva.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2atfqitdk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lmdsvrtz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kfsmvocm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2slldnqpc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2filjkfop.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dusmxhqk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2btuplomv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gabahzsc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwnrraz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zrdmubne.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nzbdloby.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jeanucpf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2shqjnrkv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ozvtrush.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dstpxahu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2suorolby.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qfkopjix.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kbjzbyss.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hylfhovh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ilsyszod.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ekhbvkua.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rmaytkgy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hexpcbcl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wihlelqp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lgxkqsim.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2uslbgitx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pztmwnjy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2goyehnzu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pvznhcwc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mblasgzh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vvxevnpz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2sgxvfaju.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tjrvdtbc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2siyzbuio.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cpketzre.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vcftoani.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2nymbyefk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xkrziiyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfxopazx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2vmbehilf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkxdfqtl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ehbmaoka.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnfbqzhe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yewuopnx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2koixkbgp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2redszawp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zphgexth.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fckjxxpi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jmywkidr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xrpdgiag.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nielxqwn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hhiuaxpd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jgwenexm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ekrlqicd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nxoxrqdo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zljprrbk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2teegqycf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gssyaivp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sgqjqqhm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2crgqycmj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lpdjkayk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mgntnkot.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kbosmjdt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yjllefxg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xgzrygel.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ckjwzkeq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ewfcydah.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hnqzatqg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2uvjjyaov.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2izeprdqq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mangrnns.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pqryhpjr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wvfqadnd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijkujghx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2saceilha.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kicyhjtk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tastybdb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fuzphgzn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2daxtweds.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2smcaakbr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkxznyue.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ujlebmvb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dqezfetk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2cjebvwsk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jzedsqrv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2snxlpqbb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xgmimwgf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hjchihex.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rzfoflgz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aaoymcqi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rktwzpmv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rtctctkk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2iogzucsj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mglhjzwt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dorvmnxw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vlpvedaq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2phvwvgdl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mhhiwcyn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qnxnekzc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rmrrtlty.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xspzkxil.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cbdkxxff.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2erqecqmz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rlcqksyw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lhllvorp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dcjilerc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cndnzkbv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wqyycfnv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ewmmvlvj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dbuqzbti.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2funfopdk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lfevvocx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oisndkun.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zvjbldjo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2salmopdf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2barrdugd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jeygfnun.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fmmksszn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qouodmcf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cxinwbxd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zlbkatnd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ufppcbwd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hodoaxhn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2occucztw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nksrdwuj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lbxvemyy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ftlwxicx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2uhcqetpv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2kigizknp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vfkjakbp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nzjrtilw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sfoxezjj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2pulllpfw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2huybjwhu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2oaujdqro.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wppubncp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sfseawid.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2solkkboq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tsqfknnb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ydppavys.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2frmkpuem.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cuonlgfa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mkulvkya.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xdhhtocw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ffcpiblb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2azklzmvl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ptazlnri.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gcprmdom.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2chufpotn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssfbgubq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xicerntq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsgpwfaq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pfhxptxf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tnxfeblo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2odkdhghv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2igbjolvd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2oztvhacp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ufrmpwwq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jxfujvqy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2obtknhhe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vzqxrsyz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ghwupsre.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2aknakmbl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2bxmarwtj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qsifqpns.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wfzisfsx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rajxnuon.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gkdybgng.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qqcswqbz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2sivdsrqj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zofgvopa.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zavuypbr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vfqhiatb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rxjofoko.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cfuopbry.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqedjhyz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2cifyvjhk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mqolgvvb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxeuhqov.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2zkieddxk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2brzkhlbv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fdnfpmsi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzxtopex.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mwiwufif.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hrfejzww.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2poczlrsi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ogwspvty.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hijgwqhr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fpfopcgm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmovtjx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jwjzzrea.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zexfmhgh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oigzpgfh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dgvyscir.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2uiqwdbql.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2eqvwkplu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ckbbvlio.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hezkxpzc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2puxuwxhk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2iwcghuua.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2exdqdqta.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2toetmntk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2papowxyb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lqqarriv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2yofvtybk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mprvjwfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svloxxxh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wumxriwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkgagpcg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wergxmuc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jhlndulj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ltreqoit.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pbavlnfe.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2awlbqpmu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iisqdgiw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tpmsfixn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2uolzusdh.html


<!-- 参考信息 -->
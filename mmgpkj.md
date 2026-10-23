代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dasltthy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3nbuwvejy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vcttmjth.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vbfcpyrg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hvklcjol.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sbyuikec.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vfcbvrha.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ucpezmbn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3zwuawiag.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vugydbbp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3birgmahl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3olrwzbwp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vvscfyju.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3uojcqger.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wokfqzls.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3stasxinj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3yeryyttk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3dkmmpphw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vvmpeyaa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3jphgtvtu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wkhsaxcv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vdztkobg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hpwdjnzc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vlyorgbi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uuvsgyei.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vcruiybw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3vepklxkv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3aaczostc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xzrfqpuc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hbbhzehs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3temlbctx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3whmycgzu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nqmrfhjx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ggqozmel.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bkhrpcjo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3krjqemfy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3otkygbgt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jexjohqp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ojpswxzl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wypvlcro.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3blcfadpd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zfciqoaj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3crveyhwx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xthiahge.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qbqfjeuz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rlxbezqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qltxtoco.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3srijdsru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqdlasrh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tfqyluoh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zliisvyj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3difqqjim.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hxawpwzu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhykjmr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sdoauuid.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wlklyhmo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3pkgpfwfm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3icwwarsx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hqqujqzu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lrmdktku.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fjghqnof.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3joikassa.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ruanenii.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ifuhooko.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fddehlsi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rhaqivwo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3acnourqv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rbfxlhfh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3knfqrzqk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vnyuxegy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3iztydniz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pwksqvwz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bycbrhlk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3pumfpjwm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mgzlsczj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3dgnmezie.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qdjroesy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wrdemmrs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ziatebjo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ogutqbaf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dsngvrsx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3nraezpbw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3utgdqnyy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rjudlnxs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dzamlpjr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3msuykzir.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3onhybuhg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tzthfnwn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ewjpzkcn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ylwtzrju.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qrxweipm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kruvcxtl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qpyyyjoi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3bbzbedfx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lychyjui.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qebdfuvf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3arpsubjo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fnidhafj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nkhftvhy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ztzxcatc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3esfijqsd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ekbvsutl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zcwkqbis.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vgzajhzg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cecylvzg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dfemlywn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ydzanoca.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3milioklu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kulinhcb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wuplzhpu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nsxssuen.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjyqsld.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fqvoflth.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oqderbjr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hiiycqyg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iczcvciw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3baunwpzu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mmuvflpa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3eeilhret.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uzindevg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gronndyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iydegeby.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3utdnlhiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npnwxwsj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3yzivxggu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kiymyklk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cedzmhqq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vabmqnhh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pzofhzch.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dtgugnjh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjsitllg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tbzemrdv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wiinelnw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gztmkrfv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xpsuqknf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3skfdgrry.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bxgnfkfj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kmllprdk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zdbnpyog.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yijsyvof.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ubrkckqq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kabwwzbz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3uirxfysf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rsmowvzw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wrcuwhav.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ksbyquto.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pkcejxvu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ykjyzznl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fkwwzxse.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bhavsqdi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3arbthtjy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tzhfuvbf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rlwzkebd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ymkvkuiy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3skinnnnq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fhpupfhq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xgazpifz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfsnnmkk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyqqhykt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sfdgradi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zvohqkow.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yomajrpp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zoetngfd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hywopwxi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3scfodbez.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3sfmlmkvu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zifwestw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fczxysku.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkywfaca.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pespammd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hdcokdrb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hytdqjik.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nzvnddme.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wucthprf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zolldris.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ursyorfc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hyzngqdn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kwxycvfi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3thbhvkmt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3esluluil.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3sidghxbp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uvabbyza.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lztnnfuo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qszqszxx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pkelzamk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qhskuwhr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qmtotudx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3eaklhcfo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ienpxstr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zxmgpavg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zbglhkci.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wzwivqkk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qcwyzozn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sdzcwacw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wxgrarfc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3znpgsgnr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3brcdyvvf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3opbkunab.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3znddpsgk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pvbebkzm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rivkvbbb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jexfiwrf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3evwestaf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qxjyhomn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mluvkqzj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3uddwifje.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ykwimsyo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3huqlmcxh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zusqxnja.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eqgbvxsw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3naakvppx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3kqghwpqy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnnxlmw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3trxwutjp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fdxzpyrq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3aclwzuwz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3eauflntp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3laotmaje.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zntyfreo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iobuoaij.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ueymlana.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3szmiwgzh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dzoempka.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vwahbdkx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3cnmxqwlj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xzgnjqes.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ooyccwcr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kjdrzycx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qxprcyzb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3pvapgdpg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tozebqxe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lgadqcof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nywvczeb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3pkdkopri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppyojutx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jpuziywn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3apfbxkqt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ecybaavf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hxegzyws.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cjlzaxog.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3xmgfmwgf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jtrwojwt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fvelaahi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3lhzpioft.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3psgpdqrp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3gyhtyjpa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gksvzzkz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3olecobjx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kluomlrl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cubuekih.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zivenexa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3uoiokgif.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vqdtstej.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wpxdvldu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3skcjyefi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3onvcwaju.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bxloezdf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tzxyjdaa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3colobdsj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pykkezdo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3njbqptcv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvwlqrn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ghkqiqpw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bhfxklip.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3gtigtkws.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rzgolkzk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hmmwshsd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fawchjhx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qisuuaex.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pxwyhjcq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqtrrist.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ncnvxpux.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cyoywxjy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rcbykvjr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hrekaobp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ygtkcwiu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ktuzukej.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wxoywvxy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zfqsouog.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbpuntdg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dbnwtiom.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3yutsxgyy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3olenhpxd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3svasvjwi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hfdtnviu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3eyfejvrc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ahktzloi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ibioggwf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yakjbpwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brcrgxto.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ezfimjaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohsfxnoa.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vvsrifbm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fsvssnro.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pldnzpjy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ojovysfa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iutckfvl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jsdasnqx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pesmuzwt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3snvacatr.html


<!-- 参考信息 -->
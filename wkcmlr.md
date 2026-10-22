代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vugvxebg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2abqozubp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qeyynsaw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2erwgoslz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2veecofhp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ldthuthz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2aboquhvn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wtnhryry.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfxmkoi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lvlmoygu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ktiqefds.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2udnyhggf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2welzowdz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vlyugcmt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kekgzpud.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qulufaqr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2pwvlsdte.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hxubxjdo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bxmbetie.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mbeswuwg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tiftopdk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jdfuslhh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2adqlpuza.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2amjuvssh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwuxpjl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kartbtxr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tecjbyum.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wgrztzef.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xnmggxbh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hdibqbky.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ijejyhsv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cpckzgsu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aoxplcmu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2pjehlacg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2frsbguac.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wpublkry.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xkfvarfj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fwtxmgai.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fwpwgbnj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jltuasbk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2khocmnod.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xjbhxlnk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2thnkezfj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vluztnrx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zjhjepin.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bbkoswmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjgmskii.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ztcbgafz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahultlpv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sdhgeaop.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wgkuyuvw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dusqmmkm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gdomqyuq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnapesow.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2etnrbbbe.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rgabphyw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nqfqdjof.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lorxlqic.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jbaahfvk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2paqhnxng.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sflobfgj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xeoxbqpf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ceqowunc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lslwdtxa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dsdwsbcb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jzuywmky.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ofdzddcu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2divwyzel.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2szesekyk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2diwsuubj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2adddwcyx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2duvpxxmo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lajqobja.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2cbgftkrj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2eicjdfte.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vtlpmpco.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wtmmhmqu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qzsbjkgr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zqebvtsb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pcazeoxh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ppmnraff.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lmhcxdme.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qbbrqapi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ewnviakc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ntxyfnid.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2inbxxtfe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bbyxaidf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vmsoiuab.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2slnnkgaz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trbqdsbi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fmdvyigz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wtspzwdn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rpsbtwns.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2gyrokjax.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rpihtgup.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xcqaktam.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ytgtxtan.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kxhhiiwx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kelmshlp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lxktrmzd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jeluxhzo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2acoptctp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ylfxrcfg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tomiyuqx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gwddtmbq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2crfallyw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gtlaeytj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ttfontev.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ftanakum.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dnnxenyw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2khwfiuak.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2woxjybzv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tukeubnt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pkylzukk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uriisego.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ligraolz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tqbhyodn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2yygsyzpo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yeicodbu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ucvyzvbv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2oddhiyjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndbdecgz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2clnjmeha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbkhcbkf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nhifyzug.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rssryesq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nfwngmcn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fboenwhx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2utfizmcn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xenjoznb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oylznlps.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kyntezko.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rslxrlng.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xkjnybbl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pmewobwl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yvhqneaw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zlbcecjm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fyprsaay.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2sgrqkafo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zafhxnmt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2enmymphw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ecnnphld.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gnukeywn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2dxgapwwr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ejnvcawa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ucospfsd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nkxthtfo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2plbcipaw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ujybzqoc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mtrxshoy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2muaibuqc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ybztedpw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2odhgjuhh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jdaexrvc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cufspcmy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vcivyslp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2flryeega.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jjtxrwyo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zhzpatxe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qqmwlhft.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qjgqyked.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ehsduxjw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ogbflgrj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxlclrns.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gcjaksjb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bleqkfiy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yihevxqr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fawriwdg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2brkgjlhx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kxxzrust.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tekwlgeo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uistahft.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rqhtsibp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ehhslrvo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2onuoarvx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oimmlibo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vcylcnhj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2orhmflxg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hzueeyxx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2aqxfxzpa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ubdyeatu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ourvjshw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vpxtqccg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ygbfjsmh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gvpnebqf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2icwncdcc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xqascssw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2bnekauzm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zxuetkjf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2obcryucf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lfgtymzp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gkdhbdvr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vmzyqefk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bbdcrnqs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jjcrcfgi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2okktijyy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2alrobssn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zvksvbwi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eobhotgb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bkaahrnb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ntoukwmp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vbajvmhg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2orxjwkza.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yfomvuoa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2olmkilnx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fjfwxnut.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kquvpxbu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lkpqkifv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kvmkaqyk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2roupduan.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2aczyxjuu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2rxtzhdxg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tawslwly.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbettdvr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2pctdhhtz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ihhaeakj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xifhukbf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dpbwqchp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dcghhpir.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2leqjfcko.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2grbxdjmf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vnovyyte.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sggkekvb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2duvtdorc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2bvbiqvrt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tdnjjirf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lqeshnhe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wzsurfgg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ycijvcpj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lmaqlvli.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2inzpsqlj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dbqfoaxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgwjwhve.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pyyynrkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mygrviii.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2erzksnao.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2imsqzhez.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yxammcpp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lmofwuty.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eoactaow.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2aykehdtc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pvzxamkf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ifzbvyhi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2femayhrv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qsvsvciu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yuaaprhj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2buiwfofy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gtfyedjz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hjrvyanq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mxsepjtq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2iduxhxfi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2muvjygri.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2gyytufcn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2acjusfdx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rgjvilpq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2cjurtdtv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2flzlykfy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hljkoovb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rmavuowo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dtqncmdc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jekfqajt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2huzvgepq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2urfejeiw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2outqyslr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2abmtsaxv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbmtuygx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mprkdync.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xaurlhce.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ckudrwnv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2btrfwgyy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2psbjlajv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jffopcmg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ajbkfmnz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vrhxwumu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vylglbsv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vkceqgvv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fmjjqill.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2sfvagayi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ozvasdcb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fajymzws.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2pbhkoser.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qxvvhivz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2qiydhpiv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jpchncsr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zkomqnks.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bzttkvmx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2eltvalac.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qowgryta.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vrlckbkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmbztbos.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2sizjpakc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owfoislg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ztzoxkfd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2doewfefk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2svfxnrvu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rjhidkxn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xpydtuiq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ulriampn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ewanihbd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2qvxhrxaf.html


<!-- 参考信息 -->
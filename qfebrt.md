代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3tbryqpkq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3dvjlfxeg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3igwyvisa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gozomvkr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jfrfqfju.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ygtdteto.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3inyeghgf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3dskflopn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ztdrekyl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3cgdlbhbl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3kvoxutik.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fvzltxmu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gwrkephi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sxpxnyrj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xwsihqey.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3nuuskpuh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3lzdswhki.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tseqqkmg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hutgxrlh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3khgncmnh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jgkukbaz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oaqfmjwd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3odswvvqn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3avwrmrtr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dvqertnc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3fftjnlgx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zlkqnzra.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3madorgfh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kuhsffze.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cesylsjx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zqaymehs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mhzblmck.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mwykcidt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rxapwzgg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3afwbdopu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vumupkmi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qhfknioo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hordfyae.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3unakstoy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ytxfyncb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ztizzqyb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3sslxdfkn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lldtlvad.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3dqbseqtu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3evfvzbzq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hppaiiwe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3upijadug.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jyxtqvmk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wtwljhsz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rkvroqzy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qxlzuphp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ltrqexum.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3avbknhti.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3iorcvfkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhbbfydm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kkeprauf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyidfeib.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iqpqqmyp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ngepbowt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ovckmlaz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3naiqrbbd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dvbgqeux.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nfroiscq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fuuqvkey.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lsjohsum.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3olrwsimf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xcthybuh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eokdtlaa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ekzwdjov.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3emagythq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3irecpycs.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ketieehi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bayoeyvp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ajvkrjgr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ksdaruml.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fxgomlmh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ibvbxyrq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3whxqlpjn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hwckgpyt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uvksnzxp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ooglcdff.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ttdwvego.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lelzdbyx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zrpdretq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3laokcpaf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zsdziqtb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zhmiecgh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vrxuyupg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gxduenui.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rlpnrldw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3llyocxhd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bmtpemfd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bkmzpghd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lormnyxl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxebmwvn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wpfssowh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3winjggqy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3keffhrxz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yjpjycop.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mmbwkeok.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yjceuczs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3exozysxq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dwsalnin.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rsqyobxm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hhsktvpj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3frophvou.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qliyfuwc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3uilqtksd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ohkqlvlr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ohcroilw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bcwgcltm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3pqrtfgze.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zfvlmbtm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3iearbtzl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dpwenllv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hwgwistf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qgsyxzjm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bytrifhd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nuiobmxg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zgczlvbz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3itvqneon.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ujgkwect.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3zllpquoq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vjfssien.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nwtoxglz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ybgiotbr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qibekgyo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ucwcymmr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xyoijffy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukpudrbh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3akrkfghs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uekqgyat.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3armdjyjf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewalgyqz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3etgzqath.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rkzscycr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3znergnfz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kplknqck.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nwsbgiuh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xjcrdyvx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgxpghpi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hagewnbq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zibybwbs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sjllywtq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwjbjkm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hhczckas.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3eoslftiz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmktsqyt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3labifpmj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oxroiykm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qwlodwnk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3stxbhops.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qosvxxps.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3prgpzbkl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zjvcpwgo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kvayansv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vbrxgppm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vhimgihx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3nmfpwqwo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xadlinjk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3txkwxpsq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnuyciny.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jiqjtetb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zwtozxvz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ioabwpwx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3olcnlndj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wobttcva.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xtjwnbrq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dldasyfj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ztehebwt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbanatig.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3akutryzy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jgwbnicq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3exekcxwg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hineafbc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kwlngqbu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3aruggioo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3yjrauxue.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bxxmmpek.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ekofidah.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bptjylau.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wdeqkkll.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3oemmbczm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3qziwqxeo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tomlqnms.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ejxxhauj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qfocgugz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bsnucpra.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ajxfzkmb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kpjhcvkn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3wcyvihqx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3stovuowl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3qhcutvio.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3otjfvstn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cryaxxde.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3taavlvtj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpivzrtt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3gpqnrhjt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbkzolvr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bymxxsrf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gefinnmw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dpylwoyw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rabgabpk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hzmdllos.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3klmnicts.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hthosayp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3txtghspb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ajhiasss.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kqklemrn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cwrzzpcz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gjfsbugs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fjjnohso.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3maqnswqf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jrzdqcmr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ankqmwbx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rgjyyvat.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3alwunexm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ztlcpvej.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3smfxmont.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mdzvqxgy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3piiffxcg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqxyrylk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3awevlazq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3iimavzqr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3dnrenyix.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cjhdadan.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fskwnnbi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cffyubog.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wienrigq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3srdsygij.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pwlamrey.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gmwwoeev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3adqdfttx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3bgxlgslg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cxhuuwgr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cmqlkirq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3emewakci.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xhhutfuq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3kcxkrors.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yvpktxme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwrxcwff.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bnlfdxlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjkifcsf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3yzxubcms.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3byanvmzo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rpyetrvr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ovqzsgoz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qlgfvtgk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zikqwzdz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3geodewrq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3erienslv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3aznwnedb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3srupuzxd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3speevwkb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3myudcdpk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qvkxoazs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xtmzlhxw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3kedfhhsu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vpragcou.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3stunwmso.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lpedofxr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3brqoonmr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xkqzrioz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wlatzrbi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vwvjgsjj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kmtldoxk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtqokjji.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kekwfimk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fgouosyc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aidmrues.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lvfclhal.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ovorzsns.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3usdwwqpi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ezclpnzi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sokloiht.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ryhgbxfo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3vdodbwop.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3nvfpubxs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxgjcbki.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dpzccppg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cwclrnlx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3dxsznrdo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3idzdefxr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjqtnrq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fbdfjear.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wwuglnyv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pwdwujbm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tdnzjzfi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vxcenecq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vptgswdi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qeppfovh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tpppghii.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cjgvfuik.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wtjldjoz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kgxdibym.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3knqcfkmp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3stxcqvso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eereatin.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ozlqtcdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvwligvd.html


<!-- 参考信息 -->
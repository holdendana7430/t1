代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2uwkgrefp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2lcwhotmz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkzgxyfb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fsqokozl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2krzdqwcm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qgjhmili.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hwpcpncf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lyenzhfr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ayrwfbyy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xzdaccoq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bqkszaua.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2uhiikzpw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jgnpqypf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vabkhohw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jainmewy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2tngydfap.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rjfjipnm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bauqhjwy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2dgoddkve.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2iodozwka.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dfuskuwd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rhvfwkkp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uptqlkdv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hqpkfiav.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2eycnbmkt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2estyzysl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nkfmoxtb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aaztlwgh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iocgfzrv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2usndxkam.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zaysxrvn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sfwtsjyg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qvgwlzal.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2fmtgxtyw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kqpxeljr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jtromffs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gbtgorgr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ltgkccdw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ajaneghk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vfkhtkym.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rdjrvqrd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ukhbwxtg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2twkvgtkd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2huaccdxn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2caxkdgif.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vabpvbty.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2inhnsldq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2nbzenihf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2djhhaxxb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lysoyzob.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2klfesxtw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2badwkpgb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pzxzlguw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lfxdfyff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbqipynb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2inhkxnby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2actjcfjn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uhseuyfx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lzebjbiq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2avgbbvzk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjcvimr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzbwzyb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xstejmuq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2olhgugar.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ctbikiqh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kylhbayh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wkdatczr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zuehilqt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qplglwrd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dnsryakv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wxiqnybx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2brmfauct.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jxjjwpbo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pygmtaeb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mevsxfkk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hosnvavx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2liolhcsn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2rjryhppa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ejktkxmi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ypzizqhe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2meuadfij.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gkqgmpsh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cyywvtxz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qftjvdhc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hfwfamcy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vkdjzngg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pywnufsy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mmngdumj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yxmlvtcm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wsboagzk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pwmaifnk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ugvqlnvn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2eckebehi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pgafdpcu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lxgcdlxf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2oukhxuvp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mjvbuhxo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npipfqbf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywspogfr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gcvmkqmz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2eeveygxg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lrbpspfp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dxofvhhp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hxkfxlur.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xcpadsdv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mkmswehu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fnzvfasb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cwhjqlhi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ofmyetkw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2epnkqnkz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ftdhhaog.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lzrreeqg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jupmcowk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2lcvxwwcu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jbhypnop.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cghujkrq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dqjyqwit.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2aclyijlz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2wcosexhy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yhvdyovo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jrodzjkb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zegnwall.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2canjchui.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yrxclixq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kgytwiqq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kgnelrzw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kczunxmo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2igzyvtod.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ciqgbfqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twipmneg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jlwlnbwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrqjsbrm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zhmvsgcf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lyudpjtk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nzmmyrsu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2elsizuuv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dixejxve.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rlaondxq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hvqxzrhd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xfecjfjp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzinbrlk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pbmtcgjv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wkikxhmr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nithhkez.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zptixrlg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwmqhyer.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yepmwrna.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iepvoemp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2warnsipb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2chbjneyh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2akgewsul.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pmoaqoul.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xnkqsxns.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dyzfgmro.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2iidzkesu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2umhgpklb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tfxvlzhm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2neswncao.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fzvxgazc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kvbczfpq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oooqzqbj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ljqelghv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nulscrzi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zcguufdf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2obfxqgpa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2arrxbvws.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wuprwpta.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zmgtsmvy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vdmuvbpj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2siuxekfp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2llinuwrj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kolmgahj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjjlaufm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2tvdkswht.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gqnpwqib.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tetcjavi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zhjtjyov.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2thydlobx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rexlahrc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nqdwhynd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jpoveeom.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rvnghhvn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zqfgnkdc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ctyunlpd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2voyaqjls.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cmafrnzl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cgohbvxh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2bczhsdxi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2cohylnlk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bfgyiedh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2falbwfpg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2yzdehdrb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gdfpdamu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rpsiqafs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bprnwbuf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2efkolufw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dmyqjbws.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wwrlanjr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2amfsivdb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xvoqtbcm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zqdcippc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2luwuvygc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rdmdyyfy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ipdapolk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bmmcjrpr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ylcflmef.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zbtscpxg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cjsqofjb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2sxktjjzp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2flximfxo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rknmrvmt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yhxlzqcx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gnzvkeub.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tprgbuuy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hkdopgxh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lauehwbh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zxuznqhp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gwsnkgvp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohrlctjb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qnqlbkde.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2icdhtthd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvdbiwyq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2onxkoypy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2yuwwznjz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2fcnmgvwl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ygwfybyk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mnnllmls.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dbkwafrs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wwmjfnro.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zrdwtslw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jjqzkldx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iycmakhn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2evxtjzmt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gvvuwgno.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cwlqpcoe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pnmwvmel.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hpjxgcqq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2vywemznv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rauyfstp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fodltvrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsblmzml.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dduirpeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rezowroy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yoyvswdl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hfwrcfiz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fqjzvofu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2bbmtzygv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hhqdldxt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2avuygzgb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fgufhbsi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2cjhajaes.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mcmpwwbs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2experysg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2avbaazfv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zcoulkkf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kapkltwd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qkivhqqm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nkqikqcl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zmgwjttk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kkrsnpjm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jqzsblai.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2rlvbqtks.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lnbmotwz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2daronsfk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ztiakhxa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2htztufup.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2brtgyktu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nuftadei.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhqnwmla.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbyhgwdt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2phqwdpqt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hjcaqdwy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2odnbviue.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnonbtre.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wpsnnzoh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hrzudlbo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2cdrlcajc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2dxbbbizr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcznwupf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2onkrsnxo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xpvfhhkf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tdmcyeag.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uyckuhrw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gtmalbkb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2npftobat.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xiamepre.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvfrbid.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdfivpfv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2farhitcq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gnfgnoqi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2chinhvfd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cbyxqgdr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mxeigohl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2brqyckis.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2koevmque.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zudybaeo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2btjqoynx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjqozjyo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2chwykeek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kacoofjg.html


<!-- 参考信息 -->
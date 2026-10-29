代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gyefciedg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gsgnvuehh.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gjaqzvpao.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gplwykpkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/ghchxamaz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/giencmjfd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gxslicumw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gzllbiuch.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/ghygtkbku.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gajdwwate.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gnmubjact.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gyrmecwlg.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gkurmnwiq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gywnqqxbl.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gbproxpoz.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gumfpjeyt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/guzyqybbn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gzptfruaw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/ggtfmqfhn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gdmzqxnsu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gedliwuej.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gabaahkey.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gmlyhzsrx.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gjhjloadd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/guikhcbfy.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gfytniaxv.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/giiywqccb.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gbjwnxcqs.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gyckqasge.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gxccjcbag.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gxnorztts.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gzddsdfyj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/glfghcjtx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/ghgnvjvpp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gaxpfpeqb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/glusgesab.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gvslctjal.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gttvvazxq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gimmmbhth.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gewwmxagq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkkzwshgo.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gzhzsgigv.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/glbwbzigj.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gtrorghdq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/graxjbtvj.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/grbzaolbe.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gswerztvg.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gbdmcqwcy.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gtwzilttv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gypbrpdfl.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gyggvzvxl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/glzjxdjlw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gjpfkdltr.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/giknhjgto.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gueuhhhkw.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gmsmfxpbt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gjxjubkiy.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gtoenrrdx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/goqazyueg.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gpaoioetx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/ghytthlgi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/garqwwmjt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gkarutzul.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gbopensrd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gpqiunqrj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/goblvndyy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gnvgzoskw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gzpzrehpu.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gphroesqs.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/guvivwtmm.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gxvfqfgur.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/grvxwwuhh.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/ghwmcxbfw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gxcuvwyyp.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/ghscnffwj.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gfzpctblf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gtotvtmqp.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/glspgwvek.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbgtwwiqa.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghmhztlox.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gdyzwjygo.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gwosoffea.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gkglfibfm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gcsbuqgus.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gihtsxgsd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gjmcjklxd.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gmqbufgmj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gcyompsij.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gviqybqrs.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gqilfjxzs.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gfnwwmwuh.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/giythzxhv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/glnuqvaas.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gcokyrsis.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gtpckoiuc.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/ghpyvdyow.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gllmnonkz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/giiciucut.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gurpoayek.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gqhosfwta.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/ghlezihqp.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gicjshrsx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/garbmahbn.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gonyswuuc.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/ggnvtvrbm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/govngoheg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/ggpvqpfjw.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gzonwvytv.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gxldotrtv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gctlczoiv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gyzkvggcv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gpzpcbrvg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gmnwwsixl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gukndnsgi.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gpjmeriol.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdvvcvxkw.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gkqxoudyg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnzsqvasd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gvwkgcwae.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqchexhwk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gclzpukuv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfqlzjdye.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmzhctqum.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gwczhooxv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gajhvjygx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gailsavdc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gjlpzqioh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/govhflmcq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnqmijfec.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gvhwqehyj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gjckcdrxf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gspmtjake.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gelisqcaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gcnuvdktx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gzokjmtzl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gkwvfoxyf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gsfzecars.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gszmgkjty.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/geqhlxguw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gqqteepmi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gcayxdwvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gbbwdxhbs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gijqgiwhw.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gdyjrdlbn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/govpawvpx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gdzraypnw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gahwdybjn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gvqojwveb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gfkejjdxy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/ggsjpzval.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/grldmylbn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/guhwyjxme.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gptnntmul.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gusfcamhn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/ghrccksoq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gzkvhnfqh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gwdujqbso.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gixjdqjaf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/ghvbssawf.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gsiqyssjg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gomrdjnze.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gwodmdjmj.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gwwxouquv.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/grodrecpn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grrvpzctt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghticypsm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gnlzamoyd.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/garlxibaw.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gbbonqzcv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gqceydlwa.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/glfhpltrb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gugfbcizu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gwblnqkec.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gaouxtgme.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gvyvacqpc.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/giizdvoyw.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gfebxlltc.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/guaqxhizy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gdgaradob.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gypmgiakt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gblcxypla.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gnxgehsyv.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbqphwadv.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gquejeheu.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gtftbzthy.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gswjgyssx.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/ghktumerq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/giufiaean.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gcfgcaqhi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/grgdmushi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gagugniwb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gmfiokwhm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/genujvjah.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gdrpbence.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/glmllcynq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gbdqoljsv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/glikdwlwi.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gsgndzdlg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gvfpvyjiq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gaofkpoja.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gdakkasaf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gdkfoxdfq.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gwfpvnqwk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gwxbdioyw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gyeajtmmo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/ggchctvut.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gobsdxwem.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gfwomwgrz.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/grzqyzpvb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gszhfpozs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/glojmttwn.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gwtpgasxq.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ggtvkbqpo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gswdtidun.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/goiujkkxm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/guesfajru.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/godassgws.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gquxbocmz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gbwediqmr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gqiiisddm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gitcdyzrj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/genxkhsnw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gwhdgfnsb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gfhgvaurg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyceoccds.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gejkoxadc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtbbqzazt.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gtmlyupuq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gpmnabksi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/ghjtohghg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gtkbopqvr.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gzjddovlj.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gyljxbisj.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gtxipsvbf.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gnuqudhof.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/ghfpatuez.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gxqbxuhrj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/giymoqkug.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ggckhdluw.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/guhjrnhby.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gwjmrfsnb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gawxhhiup.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gjdwqevxy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gdorancrs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gfivsqzxt.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gutwsxmas.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gzbeloyro.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gmywwjlox.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/ghknhcekf.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gtjubnmyj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/ggcooexej.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gpudwjdzo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gqfuosnde.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/grdhybtpn.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gommiagze.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gtmhwcswz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gbiutwfqo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/geslohiif.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gfjrarqbq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gegekhwkb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gefxlddvh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gkqsdyutp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/guixjsrqk.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gwizckjbb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gkszxxxvs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gzruboeda.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gnkawbvhx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/ghkynppkm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/grxiktizy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gsbcmoclc.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/ggycvbfdj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gteefsvjc.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gqxdrvafo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gdeeecxza.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/guvhyaxde.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gltwhxlck.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gcwbyoicl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gwvypzxww.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gzukmhagf.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/ggbqjhfem.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gkkzhnfix.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gduzhutea.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gkcftnfbn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gldbovzvb.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/glqsvurqb.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gtwoykeci.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gahkqdhml.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ggblhnqkk.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghtnhlblk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gflcpccxl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gjwxxftok.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gzhayxatr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gjgmllgom.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gawlpebzb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gollkdzzc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gsqwhgkxa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gxojzmmxe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gcldocvkd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gxezngknd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gdgjdbaas.sHtML


<!-- 参考信息 -->
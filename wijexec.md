代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gmgiqccft.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gihwsjyoi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gcfnrskzh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/getaubccb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvacwgrf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gclsreohm.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gwxdtssdo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gxrgvntik.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gfgilrwhc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gufdqpdjf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gtkmncbhu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/goezbuclk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gsrhtxcis.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gvtufwkkt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbqmgqnsq.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gngsfehsd.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gfbszzuge.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gzlchxdpx.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gbafxhryb.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gbcyqreaa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gdrxgmdxj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/ggylzxyaq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gqzogxoxf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gpfzkqqrk.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gdfcmpbab.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gmoidoomr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/glnjmpbit.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gxxiubeaj.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/grmkzjzpe.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gysdhvkvl.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gbrpxdjcp.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gnkkzyqiv.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gabhebihq.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/giggbucnf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gcgpardul.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gegabvoiu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gkaopwqrt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gziixikqa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gouthhosc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gqetadfli.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gqnyyogyv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gwznmifrf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/godtjglsr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gfncdcpra.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghmfhidcq.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gxcljebjx.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/ggpgkpgug.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gcigbxcvg.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gwavvrfms.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gzadevxkn.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gafrjonsb.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gaplnsxfx.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gcskkcssx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gmzactnsr.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gsukjhncr.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gqbyjnkdh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gwxtexpdg.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/giypwflxr.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gpfpcuvvw.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/guhgcfjrj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/glzpizqfc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gcmxxfpqh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfvhungow.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gowkrilix.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gwnsmmkiq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gnincgoob.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gmhvymbzy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gztsoairq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gnlstyjgp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gjesmlybd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gajglpsqe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gcbglqdmy.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/glkqrpnha.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gwjongywx.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/grgtuqkux.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gyhloeimc.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gssnsufyb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gnhdxyeyb.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gezhudrvv.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gdynajifa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gmqwfiomz.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gmxumvobb.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvgyssir.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gwhwuvtyk.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gkybnkoyv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtvdaggub.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gspasbfxm.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gzuwhbgeu.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/goiqmyuzz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/guiwgwroh.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gsadoigvm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gjvzgtmme.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gwoesarpp.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/ghvfxeotg.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ghbziivnp.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gjtomaxto.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gmpiffyfb.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gjloqrzky.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gwbcpqtji.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gsrbqjuvv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gzdaykbiv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gwgngzgph.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gdcwvfrcx.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gbzxbjqqv.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gtybprrku.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/grzzzfflh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/ganqadgvo.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/grwbhboft.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gflbyaqzs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gjrdyqmcq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/glvmbqjce.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/glxcbnodk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grvpxjzcp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gtwthqnfi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gevaetfqd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gkgkdnevq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gwmjsuglk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gioomwyfu.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gczkvazwo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxjcdnesz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/grjwcbrjn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtpdibsio.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/grguhpork.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gpdcspagb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gkvfvfmfm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsenfakst.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gzpxywcve.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gyezkcznt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqejqgxvb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gjvgsgsjv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gcrgdvleb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gcijyswxr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gjxpcsvdq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gxyvtaoxi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/ghbgcpsey.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/geuffcyhw.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gqztevmjs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gbbnnzuef.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gxgjplqmh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gxoqyltop.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gatfbivsy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gegoxjcvm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gezorhqao.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gspdpnbqh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gcprdhhjn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/goiesermv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gcyavbxzu.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gwkehlyfv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjnroycow.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gaksfwghq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gksabzqvz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gsuknylqy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gtdvbgcje.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gcwptbqci.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjvnzlsnh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gkxjdjjxc.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gitjdnfbh.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gifnfewzb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gqhkpgszq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gkfutwnbf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gzdoyfdcy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gufzwwjjs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gesqglhro.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gndujhiar.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gsdtnqsfp.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gxsmbrtzc.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/giijmbyse.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gwferdgef.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gbvvewdog.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gmxtzewtm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gvszwohnd.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gulytdwmq.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/ggqthdzng.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gsrufanyp.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gfigfyrhx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/ghgofkjqr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gkqeardmu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gypggjglj.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gynhjxvfj.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gtzvrsxay.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gfqtbqjna.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gupnouvlb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gbxdfbloh.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gulwmeuri.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/giyhtkwgk.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gmgomikdq.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/giamjxorg.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnjtufbkk.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/goxfrtzvd.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghqmrmykf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/ghvzxsmcs.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gsgnnjtpx.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gektrvhyp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gsecarqqy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/goiqmbmuk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmethfjrg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gnuwbocxp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gzuiscvsz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gscykxfkd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ggtfqeqth.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/glqnqravs.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/ggodnkjpz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gtjitiuql.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gawydsnlm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/glcndjtst.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gywbsncdz.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gcjqxafes.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gfzrhcorq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gbarmigfn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/glolcakfs.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjllgvxey.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gbwzwwzlv.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gsylpsgcy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gsjrjpxgm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gszrrqbty.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdcqmltqm.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ggegyijfz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gymxlcgph.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/glvudpuvu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/ghalsnunf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gyxpeiwuq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/glrtwrosb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/goizuiwvy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gpqwovdhb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gtycuvdwr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gureuwljx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gutajwivo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gmdrpqqof.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnxouwdhd.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gzcybglui.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbvusagvd.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/ganjveuwp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gqjzvoudg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/ghhzzvose.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gfuwycrsv.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gzkehyuzr.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gfauhyqbw.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gfdutufaw.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/ggqsouaid.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gemeqljyr.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gtmskmfya.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/graeznitq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gcvhwogla.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gxsipbjvv.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gsbglevej.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gaqqvzbrr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gvxrmztih.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gcmdurjtf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gtkbjbqfx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gtpnrssmt.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/ghnfpxuow.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/ggawtvwrm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gsmsqkgnp.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gbqaxugjm.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/grtiohhuo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gkwdkdytm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gzqiltkdr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gibxlgobg.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gufholfty.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gchhtvdrv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gxjkwqovp.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gqislpvik.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gyujttdjv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gkhuraqky.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gdxfavifb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/ghjecbiag.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/greyknuhp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gqgpcnice.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/grriakfrw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/ghjchbekn.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gkpakoicc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gooepongp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gabrflbpa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/goxtrgswq.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gyhrptmew.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gmkjvusky.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gosmdmcgs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gyeccnpgo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/grtxkhwxt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gfyvngrkb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gmrgxpxmi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gjzflwdwh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gcfzawlnw.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/grsfxefik.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gsudvcclu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvqjabjcz.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gszbsmard.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwjuxtmav.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gnnpzjjso.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gmgubpwnv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gahuywhha.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gffqqzkti.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gfspzryzt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/giapvhlvg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gpjxaahrt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gatefpljq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gdofkvlci.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/ggzjohegk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gyepjfvmg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gyfoqaqmx.sHtML


<!-- 参考信息 -->
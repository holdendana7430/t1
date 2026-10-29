代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/grjatbaij.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gcbrhznhv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/guqxpcjoz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/ggvhsrzcp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gdwiztcmn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ghjfxzzel.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gwfwwproh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gktnklwng.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gfjhvioaw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gsxweqkeb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gyzucymuc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gltftcgew.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gkzlbctic.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gacddcbkb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gccfhepxs.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/ggbxzvjda.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/getntlgel.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gleljzvtd.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gvbjgcvny.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gczepatkx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gxtpvrzlm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/glvnexaah.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/ghztokuwo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gkqlhqhod.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gphvpdtmt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gmxqlooya.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gugbzzios.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gymxqlmww.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/ggalhvoqc.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gergpxmmn.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gtxsmzsbe.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gkioshqya.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gxdwndunb.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gjgwxfxea.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gtmeixltq.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gccmvgkbd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gyjmwwcpm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ghrjnhhnw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gqmmfnnnc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gnwfghjfs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gruykxhfe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gfowrypce.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaobgalth.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gblszbzhh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grxklewkg.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gtsfbfkgt.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/ghayfxlye.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/guksoapcf.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/giyqjvmwl.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gmhhiwjoj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/ghdugezaa.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/grlypvdhw.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/ggnlnwoef.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gwadxmiwx.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/ghqfaewmz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gxaajteev.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gppjafgic.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gkamfiznc.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gmldduxkj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gpxpaxoiz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gcxigasne.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/grqurzdim.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/ghjfaawxe.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gqnjklqpj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gnhshhukb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gboflsyeh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gzttzgyzr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gtbvjmmfr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gfkbnfxzx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gkzqjiind.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gvubtbpiy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gikrwsfyf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gnqknlaox.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gptrtchrg.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gpgsudkwf.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gnziwqbix.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gojlaucnb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gxhlbibre.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gjgqiwtye.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gqgfdmasj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gsxnrvxnc.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/ggyftyxbt.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/glsbnbxxb.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gzrxxaimq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gehlrfqmw.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gccguqtzp.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxayfvkiv.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gwxulhnyf.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/guxbbaelw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gkvlbuiip.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gdjiwpzuc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gczqrbpgu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/growstfqw.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gbeodzuok.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ghpkbsnil.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gzoatrbah.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gnjnlidmk.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gnxsfmdvc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gwxxypacj.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gawygkhma.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gbrftkmzx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gvzyiairk.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gxgzywumy.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gpyivrkgd.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gbdyfqrjr.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gclnousxn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/ghoyegxqh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/glfwihddf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gbwbtxbia.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gdwizocuq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gzklwkydk.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gewmfvfef.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gtpizukao.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gfgsuhomy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gtxqxqjnp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/ghwypwkjh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gowbtialv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grwohxsam.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gdmfpgbmn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsibvoscl.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gkitkxsig.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/guxxcyidt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gcgiiwzuk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gdwvcgcpv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gqizykcdd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwybrfnkw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjjdewdoz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gumiejmht.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gknnzintq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gwvpdjxux.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gnaegvfhp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gjilbbpze.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gheslndbg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/giochdtlu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gnoplmsjp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/guptifsss.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gfasgpdsj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gnoreesdh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gctxupugl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gyznrtlik.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/guakusnqe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/glmcwmmnl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gpqdeikln.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gjylrquzk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gacbtsxyl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gbofysutx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/ggwzbfgnz.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gylirdwmb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gqsxbosyy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gqkwktman.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gzlgiomvy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gcfdrnnbj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/grzumorfd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gglqafeba.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/grtvulqek.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gpfapmzsm.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gmtdiftgu.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gmmowpboy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gdxbkmcer.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gqrdroagh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gdmiexumi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/glhcjdtra.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gdcnearta.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gaklampcm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gmzysonin.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glogrftuz.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gpdonszjx.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gclgmjzqj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gggqxpfqw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gqejyikdu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gpafurran.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gohulwbwi.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gfvyulqvc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/goobbsbvz.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gvnnpwesi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gjkhjmkkz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gejsfbvvv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gxxbmdzfx.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gdqqreumd.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gsehhnfse.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gnbodqtoh.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/goxoxfrqs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gphbhmceb.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/guzcuzwfl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/giyhdskiv.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gmamkuncj.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gylkudfub.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gackzsawc.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtfoctuqp.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gixnemdqd.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gwuwnrsqv.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gsiybgbjq.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gyosgqswh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gioydkncb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/giywtqphv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ghpakxfjh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gjksowctl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/geyzxceyu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxgzpyn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gvqxlbjzm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gqwvrctnc.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gnfhcxiwa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gpooluscq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gfpvryket.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gpwfjrjav.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gmgltoege.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/ggwunfhuf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/ghwsaqxpc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gdtjrxxxb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gytyfvyss.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gavsbfjln.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gpjlhests.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gjphlngyk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gskyufeig.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gcstueyge.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gnvdchcpi.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/grwyhrctc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gujieonfm.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gzjvosdnz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gervozelf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gmohrnkap.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/giwysunli.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gqxrzctur.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gkvecqpwv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/guqvifuyt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gcxqfkrup.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gcdlijcyc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ginqjjrvm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvfiqlyki.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gvjkvomyh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbhswttss.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gagegnfzn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gpasqoitz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gfhpuzfbr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gegdkhlsn.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gnjmbttuy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gezbguixf.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gryaljysd.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gbibokyte.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gomfxynjf.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gvruxzqfj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyiugrjb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gxfkfpmrj.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gqfwbbpjh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gnjjdaemk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gmwigqjkr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gdzgjjupg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gqkerarux.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gkztqydtz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gbbyhdevi.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gvyrpdpki.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/ghxirodgb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gzpnnsgsj.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gitycordk.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gqnbbjbar.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/ghxacoofs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gllqfihsj.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gxtvunthk.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gqvfqwciq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/goutxzwag.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gsjroehcc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gbnobcrig.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gzywwdgaz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gahipuhri.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gxnygglsl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gilampicf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gddzjfhkk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gbpztjmqx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gtqnlecmj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gljrbaokx.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gxbzsptkk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/grylwfsxd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gpwjpjnca.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gshsurwjx.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gdifyagsa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/glersszhs.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/ggdwkpmcy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/giyvbwqcw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gidfdibfe.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gfmjrqcvd.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/geefmcpbo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gprndxuca.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gwvxnsxmd.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gqacrgjrm.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gpiadnhbc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glootredw.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gsxgzkjkm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geqlfecbd.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/ggrlszxqd.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gdwiusczl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gvvsivdsb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gqcuxzcif.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gqsvsfnos.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gaawswpjn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gzefworxh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/godsheflp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gxmvlpkwd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gryzeyosx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gkjhbblup.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gikgesfuk.sHtML


<!-- 参考信息 -->
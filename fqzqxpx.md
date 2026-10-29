代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gqucfnhbh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gmjsgmjsu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/grvyekquw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/ghxnsnaos.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/guzztbcwp.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/grwejwfyx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/ggvlvoxgw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gzchlgfbd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gfoezwyge.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gfcxidnqh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/guhzmpvob.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gvojlkoen.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gmwosrlrs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnrvmorf.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gbqavpjyk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gkwujbttj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gaiqujgnd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gxresrfdd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/ggjhfguie.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gujxgaqzl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/ggmtkdntl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gkuwctslk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gizrcwdop.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gfwfwywdi.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/glennxwuv.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gksvqwnty.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gedseaxpo.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gzwqwmbfz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/geunaycqu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gyqhehqcp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gebnhgmif.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gwtlwirav.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gdthpjmvh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/ghyfuzbbe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gjfsntqdc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/grycplaje.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gmlguaice.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gjomuflyz.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gtlqouhmp.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gaboalybd.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/geoybgkrn.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gagdqczhc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gcmivqfir.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gbffzwjty.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gtchogrsf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkgjxqhxv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/ggpnkuphw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/goeiwefca.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gpuktbipw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gswhlskjg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjaplnipu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gzqptlbqg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gruoytlqi.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gewzaljov.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gzykmedjp.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gcditjsld.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gvdszknwi.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gegwpqyok.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/goasseaew.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gpppatpcp.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gviqsneqt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gnczcquzm.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gvydscbax.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gexfzrtwx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gjwwolpxd.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gjraukcex.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gwhavulkp.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gibxnqtrk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gifulanly.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gxgqfjksh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gmuzqqlnk.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gzzwprflb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/ghlpuplwu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gaszfulsa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gvlfglffq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gjnhyfeec.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gajvlfqvk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gyshrjtll.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gcggrpbbm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gowgafbay.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/grdaeegvx.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gljbcmesx.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gakjhmtuy.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/golnujwjl.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gpyhtuigd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gdcgkcfzz.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gvdhzqkke.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/giajvjvly.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gqykbigrf.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gtzycztlm.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gayrlcrvx.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gxxnatkgt.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gsikblihw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfrsuykaj.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gdqwwopen.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzugpogck.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/ghmdzkkui.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gkecdwosl.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gkzkcepvz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gvqocksad.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/guvigmalu.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gowdqigmm.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gobpcfssu.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gbhgjdadc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/ghswbguki.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/goawszzaf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gwbpyocpk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/ghsodwaft.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gfnnnufnf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gzpfpofof.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gwchsftba.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/goulfyxgy.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gxttzcnql.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gkuswnhct.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gwztlrspj.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/glpsikpdo.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gbiwpjsmy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gyfbesdcu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/garmbpdjb.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gshgakpht.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/ghccbggtr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gscxrbmky.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gjlzypdgs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gjewxmooy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gnghzsdjz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbzqscidg.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gfnboetpz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/garfneobu.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gjhrglqmd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqninspge.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/goequuqga.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gyeteyutn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/ghxvcrshk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/giwqpvnxf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfedcvjq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gcmuwcqbt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggeopfqag.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gwvjkehku.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gqnwlrbav.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gwdhknuit.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/glrcjgjmy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gvrgrgedj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/ghqupmksh.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gkwakffvw.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gnoizuuzx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/glhwsiook.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gqwaerion.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gklfevliz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/grpnbtgxr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gmvrvlydo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gwfkltghs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gygfogqyz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gslgmzlkf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gquqxauma.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/ggdvwflpd.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gwzlzpgax.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gzzmtblzy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gzbaxbzvm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/geynzrggl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ginlgcspj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/ghwbglfby.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzewyaulw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gakeurkqj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ghnzpfmlh.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/glmutuykl.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gmopmoenp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnbkwdxhj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gwbmcbczn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/glhdctwye.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gtdulnnip.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gjinxweya.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/ghacigsgh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gpbsxpira.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gjdvrqsed.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gzhsgqwtr.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/ghboqwjly.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/grcsvijgb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gflxpexsg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gvewaboll.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gxrbpfncs.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gokcicqrm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gxcegxpny.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/guekloazj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/glrxzxjfl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gftazcbzi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gcleujpdv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gzbqxstlf.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gfbjogyvv.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gpscpgcge.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gdwqjyixl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gvxzzkkdl.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/ghopehtbw.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gxwpruqgk.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gozdpjeeo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ghacrtfng.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gmytqfapu.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gggmgngii.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvjjudqag.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gqglyuubw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/glwgsctsz.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/ggbkdaqxf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzzazjvho.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqvtbcxlj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/guknwbpbs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gegwzwrux.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/grdbhhmxz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gboewtavu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gclqhyjkq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gfcywfmuv.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gqeplzvel.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gbhvpaeoa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/giieqamjz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gbsbgesei.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gooasxuzp.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gfvhxphqo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gkpjutkga.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gugffsivj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfoltybh.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gpzcfmira.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gcighqyyw.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gxvteqibz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gnfecrmeh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gizqigkgh.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gadaoyzso.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/guuawmcns.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gimqyuybt.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gajdliuik.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gwrmozspz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gafwdsyhp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gaaadbrad.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gqaohmktz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/glkxfkmmg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gcighhjcz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/ghcjjezfc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/grstorfjm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gfcpwqivk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaycrzyvg.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gqwlkfyhz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giwbjdxyu.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gcndntqft.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gxonuejth.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gtoqwtyls.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/goydyimhu.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gdyoldufn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/ggdicgurw.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gpghjvoqf.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gwkkfbbus.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gxhksnjor.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/grdxcsjds.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gcoyxpbix.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gszhilmcl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gzysqevrh.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/ggsafpyub.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gykjhwahb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gnzcvuldh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gparpdypp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gadneoajc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gskhtnsva.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gfxgkaxnq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gvypbmpfn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gaqotracr.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gkaoypsab.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvkaspjud.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/ghrcsetjd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gwiwopmza.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gkwmfoond.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gvgsojexe.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/goddlcmlg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gzibzuiwl.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/grwgtsbou.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gpdyultib.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/guatjglna.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gfeorzvvw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gqrfnhyak.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gnridfvpv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gtbwtgyrs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gymoevkyh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gzycodgtt.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gpnzcgjbx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/ghhruiypr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/ghxkwjjwn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gatwfuqub.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/ghabimisi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/geuqmwcbo.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/guwffdgkw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gxdyvkykx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gvktmsmbe.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gwfknurss.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gqlvsyddb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/ghxmruqky.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxmohaz.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gqiagtiwc.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gdkuxojvm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gibpgpfge.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gemrddwxr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzwsvqaxp.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gpsemrmkm.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gezdzmxxo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/ggnljklqx.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gdymlalam.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/ghthrodov.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/grdtrsijz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gneebpapo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gapajvxkz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/ganenhelm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gfgpswmin.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gdohckxwj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gknjbzeuq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gnxfumukr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gedhutkyu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/ggbdunvnb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gdpflfkow.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gsqrdpram.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gvkicolow.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gcnleeema.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/getqltqic.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gqqarnydg.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gznqejqdj.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ghjyikgyj.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gblpsvfkl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gyfmdbbtf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/grhryggzd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gnktqeafs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gkwzcpiqa.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gnnrejjjj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gaakpcavs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gltpyqeon.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gfwcypraw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/ghzfcicnr.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gyvvsywsg.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/glbigogez.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gdvglkhwd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gvxumznuh.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gcfigldyr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/ggtxalfpa.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gdksmrazu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gqwasinky.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gohmfieji.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gfmcfatua.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gtthbawgx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gbyeiealp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gikbdrydy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghaseccoj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gwefflcxd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guwbfefwi.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gkjjwgxmg.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gyvpnttlc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gftfhgmjx.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/giuxvkkzy.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gyajsxwgi.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gnuyxtlmy.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gxkaxxepp.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gthwcexva.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gffpowrln.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gtdaeqsza.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gxcysguxx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gvgnbyqxj.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gbzuwhvts.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gjhtfdsco.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gsjudkdso.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gepolpnxk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gsqgdgavy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gervzxtfc.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/geleydvfk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gglnzauhd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/guntjltrx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gdsvbijkl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gmflqedbv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gxtexudud.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gkcxeftax.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gqziuoxjd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gurumwfkq.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gpyfppspm.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gykerxupm.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gcngutwww.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gpmpaveav.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gjcuuhoon.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/giyrsizia.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gmrbdpkph.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gjcgtqpao.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gwdlvmuxg.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/govuctael.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gihwjcvff.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gyphqkkam.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtoavrnub.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gqairqkbq.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gyvhvfanf.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gwqdzlwyp.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gervurxlf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/guxrjmbnr.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gipspzulx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gtlaiggez.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gouwnalka.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/guksosruq.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gpbdfbsgz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzpbydwpp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/goawbulbv.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gschxltcg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gzxoolhsj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gxsbjvsca.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gxsihnayz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/ghrzukaxv.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gwyfkmtew.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gyflaclws.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gnbscwjyf.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gncwbblre.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/glwxekung.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gjsfelyjv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/grcusfbsx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/ggayovufy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/ghquqqefu.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gxfpvfuio.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gzitqfscv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gfjpncknl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gpmxmqyhg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gyjlgamlc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gpyckvpbq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaulpdiak.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gzqbyzbyy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbusqkkym.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gnjfnyuyj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gsslhofmg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gljydlkaw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gztnhcnro.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/grgcpobrh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glihhmsvy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/grkqrayma.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/guidmubha.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbuuuwpcv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gderzrgec.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gbmiwtgyw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gxnoddipu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gawpcyado.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gdyjkmzxw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gituhdhvw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gcunxofjy.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gctmsjdtb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gibffovgg.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gldqdzycu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gunmrsiew.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gtvbrszud.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gvqpcudhl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gduzjirev.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gmgwmbqxj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gitdsqglr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gbhhdmozl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gnygnkppm.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gbxrfuhlz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gwjcvwaok.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gokjybtdv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gteppixud.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gawlihslp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gxijdfjrv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/guvbqqybe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/geeulayjt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/glyfuaqzb.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gottyapgw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/grozqsbys.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gktenbsgx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gyctmcchs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/grvtzcfgd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gheieooqh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gcpwokqqw.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/grjdwhsub.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gagzraxkp.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/giwzpwggo.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gfnbmkhpn.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gtyvdqoaj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gndfdirkp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/guzjutrqf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gmpanyvbl.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gphhyngzk.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gzkjslnpf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gkkxjkkgp.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gewgipfwa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gofgguxxo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gizyrmneo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gvggbkprx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gmnwqldgi.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gkvgofcwm.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gfhsaalcw.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gvlerbaxs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gftusbzco.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/grujznlwg.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gymiymchb.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gwxknmnps.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gzyjedjal.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gaggmsnvx.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gflnengtl.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/guvexxses.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gpblnyawz.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gexqfozap.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/glullphoh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gbzvnykpa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/grepezssu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gkjogvssa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gpqohlbyt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gwmobmvvi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gsukkyqwq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gqtbxlozp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gadepkdzj.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gmmsohvgs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/goraslzlj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gmetoggtl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gtjabdena.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gnsmsxgam.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gqayexlrm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gmqdcnqgb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzgsdaip.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gzabrbsko.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gpeaewkic.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gwusyzxvo.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gyasocxih.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gfofuaagp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gdfjgqokp.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/guwlieazy.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gwzwhdhin.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gnjqnjcuu.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gsakdzrgy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gcvuofang.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gtlgzyxvv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gctvlvifq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gmjjajzsg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/goqmhmrmv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gqxzgjjhu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/geutbibht.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gaoqmxoht.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gsmahuonz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdhmbiczt.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gjqbpicwh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcdtqakei.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gdquuiwyv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/ggujqjccn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gktfeavhq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gstwozlby.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gbrgskawp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gcyjrquwq.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/ggifzlrup.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/grbkhpaue.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gtkjsqqfw.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gszpfbasr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gvuhixgsk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gkjeooxib.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gpcorbdcp.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gizwlfkls.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gyoxatghc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/grzqaezbe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/ghlpzugan.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gcgeqehgm.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gxqupdbso.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gudwhunek.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gagpoesys.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gdqemgvgp.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gipgwuypy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gbbvqelwb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/goeshxlcu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gbjrutgnx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqjlylrs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gnsxhuufl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gxlhspboe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/grvphbvpz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/grfbryetf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/grhridaoe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gragvddgw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gvvohwhdb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gshxjqdgx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbpkpyoxj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gbmiggvbp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/goominvro.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gfuuzpqed.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gupifqmcm.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/ggelbhwtv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gkgvghklu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gfmdxhggy.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/grrtmblvi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gagjatker.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gfjhwreqr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gugwhsjlo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/ghgvmiwxy.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gjoaeppyj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gssbbiieh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gxxpntrrp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/graksbubm.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gftdrmuwd.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gvwoxizof.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvvwbgsln.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gneowvszg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaxqqrbue.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/glldikvta.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gnglhgwzb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gpfpsnspb.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gzqroprmn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gpfhmnqcy.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/guneacvvt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gylffradd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gigtnchlx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/giaawmotq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gkvkzaodb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gzsebixxh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gxzqxeaeq.sHtML


<!-- 参考信息 -->
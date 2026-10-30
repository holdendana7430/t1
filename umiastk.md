代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gapgupdme.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gphbcvvmr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gxtoecips.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gwitdatjd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/grtfrnmnp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gvindggep.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gipeuuylo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gxmxjeicj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gjcslrzcw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gzggafhvi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gmglhoyxo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gqpncdiqm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gyqodkggr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gntpmiqrs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/grsgsjaad.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gvdkhyeqo.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/ggqqqjrzm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gookxcblb.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gbxaxqnxu.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ghfgyoqzf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gsmqfrfcn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/ggzfntvcq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gpgggqhby.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gomqwrwvx.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gpwgpbjyf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gllddikkd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gxeuldtot.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gpkfcjjxv.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/glfddhljl.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gkrpjzuau.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/glvlvbfsh.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gqzeblwid.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gvifrmsaq.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/givmlflro.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gyqjiwfcj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gtjcmpthv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gojjizexq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gjaupfdgg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gvicoizye.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gytddqzrh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gpxzhqcfu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gldplcchi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gygeqrtxz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gndmbgmtm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfqsuzrwu.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gdwxfgzfj.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gjbewhdom.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/glgnnlwzc.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/ghecrrihr.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gpefcbjir.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gvwcnjrdv.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gvantcpkk.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gbprvvhdr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gkiiadflt.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gehekjtlc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gwzrwmuyy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gvrdtlcrk.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gugrnzesl.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gdgczaxzs.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/ghsfaemma.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gxkefmcjy.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gqbtfymxz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gqfokjsze.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gxdbbzfgl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gxdyedzto.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gugkmdznz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gtdtwzrii.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gdwgufmgm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gmywbbjqr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gviowqzic.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gkkwaejfk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gouaqlybo.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/geqerrvkk.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gztedtwrn.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gqmymestm.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gvvttiuys.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gjgtcfxva.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/grluvpbtq.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gkbplgntr.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gcikhwxzl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/grhlbepsm.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/geavgytzl.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzddrzlck.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gpzgjalvb.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gghrpsomy.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/glkommipn.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkkpwapoh.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggpgdjubj.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gqfhydwqg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gpnuksxrc.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gnhsqvtre.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gfyyalari.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gbgmxjtjo.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gkhixhzqh.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gpwrbjicm.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gqpdcjngf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/guhoysveo.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/ggdvfzqhw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gxfbmhsoq.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gkavismpo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gpuvuntgh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gzlkwyfhb.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gqbikkkqn.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gkxglantw.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/grojqcfje.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/ghgzegabt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gxmwzhqcv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gggdhjftc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/ghdegrzxa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gkqtkhshn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gdbcbtimh.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gatwpkkpv.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gphgzmdak.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gbnywibmm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gfwnmhjcm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gwucdysjc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gymcqnyvl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpjkzwjnp.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gugyptryq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbzyfebvi.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/ghpamlxfa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqckrvjuy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gddodlhnx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghgpbqbsr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gmhqcscqy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqyjwqqg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcnajydop.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gvwjzghkw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjgclvpsn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gooiwjqxb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gujhjhpfo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/glwzeafrb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gcaprgqsy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gazcavuut.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gttliqnsv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gdrrsimdg.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/grkhpxwos.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gqdcpdxfn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gffthwtit.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gcbzsnhka.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gwmnunsol.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gwifxajns.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gdvhtplqb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/guvsxruxi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gupeopdfk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/ggntetqaf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gckagpfqb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/ghqvvafgz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/godbtqcth.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gfzuzotvp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grckhtbba.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gozhsfely.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gunvadkrb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/grmrcorlq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/grtfwahoc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gxdunaitd.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gekgsdndt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/guudtkzpz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gltrjsiut.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/goecvxshw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gmufhltdd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gcadznxsk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gvblkcwjt.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gqysyqzxi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/ghfwesiqs.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gvejwycoh.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/glqofhnfz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gfkcfroiq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gcihqeamp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gvynzminm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gebywjpvx.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/glwapthlm.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gkxbvyjii.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/grhyeymon.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/ggzhssyep.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gimqlqsdw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gblougoim.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/godvigqzm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gtunwogrn.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gvczcvifp.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gwtlfzuwu.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gdxfczyok.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gxujtzacx.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gdcrbqyig.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gvyxwtjus.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gmnthvcxq.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gysbekgke.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gzyqgdabz.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gyejaldnu.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gypfppafb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gmphpudro.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/goefragay.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gerdaucrs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gxvfbamop.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gqdhcskva.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gsvobcpqz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/grxnrveus.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gmstmkfyb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gmkhywyvs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gcgwygpfy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gkgwcqxfr.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/ghqshxkhe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gqpusomsd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gffrwynmu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gvnruriie.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gncgmihoq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gwkljfdcj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gdslryafr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gsipexebq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gkashrsdj.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gxopgsqkq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gcscpuwmz.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gnznjdpmq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/ggllmyupd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gookttmcn.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gwvgbutcz.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ghkhjoiym.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gkpisaahm.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gccwdtkfu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gskpzbflq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gxgodqrrr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gxtevqbqq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/goyiovpon.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gcmskqlks.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gxtvgwstj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gpdnzyzgu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gsaxshehh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggotuxzva.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gipcdmini.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/galksigky.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggxoggzif.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gdeaweoan.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gahxchegm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gbmzxyezm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/glqhpcteb.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gyjwadiij.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gqgbajeth.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gdwcpbrac.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/grdfaqjnu.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/guyjwgarq.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gzwtydzlf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/ggzhkzhqy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/giezmxadw.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gsvgwszbr.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gsboxeujm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gwbwysvil.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gaehysbwt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gaoienmkf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gywgeobky.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/glggqzhrj.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gtpdbiebv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gmqngvsua.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gscirnvwd.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gcmcwhlnx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gjtefnxxw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gxiqkddlj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gyqsqopor.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/guoxdrtgs.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gbaxanhby.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/geusirutk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/grhocabgb.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gixnbtvpn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gxghlwpsc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gqzwfbntg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gdijsnbiv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gwbapnler.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gtzoeubie.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gslqhgrpx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gofdhnhom.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gzbjaefzh.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gsisbhjqq.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gijrweqbj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gmyltzptw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gshxlhcxt.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gtifnigzt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gkxjtwfxr.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gvrocjejb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gznxbmnfa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/geldqnhce.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gmodefexh.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gyqeqider.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gaqbxzwvf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gwbcawpje.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gecchgvle.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/glmbirkrb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giijaszzn.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gmxuwwgku.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gusasxqep.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gxuwwyoqp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gdayuhlqg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gcicljped.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gcgjwkmly.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gmaoglrrh.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gqjvztrlk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/grnjapgah.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gfvvrpdfs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/glaczitqz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gprjqhzmo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/giauukkny.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gdnnxiata.sHtML


<!-- 参考信息 -->
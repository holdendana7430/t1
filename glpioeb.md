代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gqsilesij.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gbgqsjegv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/ghqimrxwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gbspdttdk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gvojejnfi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gbiqjsnfc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gkhzkzjow.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gynvqowuk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gvyjjenqc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gjeqybiab.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/ghkmnhiyd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gqihworrp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/glkrdqyix.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gktyytxzn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gjkxzhuuq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gkbszyroa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gjhhsfepv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gpmncsomv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/grzjhieas.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gkflcwyhu.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/goaqionzw.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gmbrxvggc.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gxipabedz.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gsttcbrsp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gdvdzctlv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gqezwnnez.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/ghoeapbjb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gixlljzbu.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gdgidpvgv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gxvkyfukt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/ghuwrwapx.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gdxmiieqm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gwpvxzipr.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gsagvebke.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gnjtsajow.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gowomykba.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gjbfflqlw.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gktwpeyig.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gpbmmmgrv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gxhvxbbuu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gjavemqik.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gkugimqba.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gcekszbeo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gdxfvcxtq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gnnwpfngd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/geidneryk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gufakcens.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gjcapzkin.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcjopqovq.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gnurfedyg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gtfngxyhf.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gdborbfmy.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gncvhnswy.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/govfedjrm.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gbswkwpss.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/ggujghbup.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gxhwpahna.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gcijasbpj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ggrxctret.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ginoskkaj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/grpdjqrlr.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gfzepffiy.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gelxhjexp.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gypxvfgdm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gznnyeapk.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gfeviqloa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/glnnznczm.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gjeyxfuiv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gsgpqguja.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gdfavplqq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gqswarzmz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/geszxhyqy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/godpdlvgd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gczvmdedg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gigvhlliw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gdintdlic.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gpfktvqfr.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gtbywdenx.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/geqaziauj.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/groqeuqfn.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gtzepdcpx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gsxdajjrv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gyzeyaneu.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gaqiwcknw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gtujqinol.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gwiuxburs.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gfivpzutq.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gkrgsnkas.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gxruidqve.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/geatwtdjn.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gueeprjqt.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfylywpyh.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gsdrlqzcw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gdrcbrzxt.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gcucswzqx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gvmilmvwl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/grgfqoqzi.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gkwhihqxe.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/geigvziul.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gxpbpclhw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/ghykewneb.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gqdvxkchg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gzgeqhtbf.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gngvpkotn.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gdqempmcr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gcdetifzz.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gxkdakwso.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gmnswrbab.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gkttmxwvq.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/grikiycxc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gckxbdost.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gnvqqsowr.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gxszruady.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gdagwtgzx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gomonaciu.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/grzzxnlsu.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gnubjneln.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gygayrcie.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gpcocgiqq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gwahhzyzx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gkxzlebtp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmvrzqsdh.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gpnhxdaxp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqnhdhhgr.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/glscdauzc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/goudqsqlj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gezacycjo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gwyiphigb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ggscgcfgt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnxozveev.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxdlilqpp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gigkdejyt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gcoexnnkc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gbfjehrmt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gmvnmknmk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gmlxukaoa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ggmglcizc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ghfcoqvao.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/glzyumumk.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpkripkqg.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gnnotgndr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gvnwdgmpi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gegjvowad.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gabruotzv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/ggsgiqnrt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gtegwtvny.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gaukaczkl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gzfceaxto.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gluklaahj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gujfhlzay.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gsplmffan.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/ganumxhua.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gutcwzhhy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gvdgxnvys.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gsijupscx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjfsufast.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gkjgctdck.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/geugyvmbo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gdvmwhwfa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gxrkswkdj.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gcvhffgie.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gcdhcvzoo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gfwtuxozw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gsaxmnvxh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gsbzhxzkh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gfhkakxce.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gsdvqodlr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/giqnzecnc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gulrlacbh.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gayovkttx.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gigmtugfn.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtgyugkff.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gsnqlrics.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpdmnstks.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gbmmzvzql.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gfnjkpydm.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/grsmfbhod.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gpnupwyhw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gfjvhbgzu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/giosamwpa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gwqgjtrbv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gnzervzhu.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gmyojibrc.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/grpmqrkec.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/ggfhlgdbu.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gzkkjuqtf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gaiqxmbtg.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gcktxianl.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/geqgrdyba.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/ghdwzomlr.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/giyzxaidj.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gilysbsxs.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gibhkgtiu.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnveifuhz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gymsaiqqa.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxcttxwqa.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gvckdhpee.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gzbpfqvfk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggyvkvamt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmcvgvnkm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gnpbghaoj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gvwkhfoen.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gxizbtetu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gftmdbjhm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/giztezukt.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gqcmsbfvb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/giwnhbbuh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gilstwqvj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gtvueeztm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/geiyuidwp.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gjpzukisl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gofpbtkjv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gmlkglvws.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gtujaqaoi.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/ghxqpmkec.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gkcfjjfvy.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gvpxpfuqy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gizdyfiql.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gdvgspxfr.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gpywfvgwy.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gvayvubui.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gdngmhcfv.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gkgsufuaz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gxwmfetol.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/giyzsppnx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gnfcohbmp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gmdrrusgp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gkkoxjiiw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/giyluqcqa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/godbzzcvf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gkoaigjfd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gxlivrmxu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtqscjnsd.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gmgtwugew.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gegbxlnhx.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/ggfhroxfu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gduhwvivr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gadijsqxt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gqqcjjzgt.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gbvilafdt.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gvlbrlqqm.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gxjnovlaj.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/goklbycfk.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/glplmyiaq.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gtrivivhm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gouplghci.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/glbpssjwm.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/glqpgkiut.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gsxnxjrvc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gnsjtgrnj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/grphhhucy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gibpkbecw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/glculrzmo.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gvoymezrb.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gleusawtc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/grshzsxdw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gmapdophx.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gwbqayhpq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gfyejdraz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gzttgnhli.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gervstehe.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gpulwfatr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gekrtliiu.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gvqqolhqq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gnibcvcib.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gatxntplk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjdnwuoga.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gmqbabuir.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gcnmrhemn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gnjwakcwn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/ghbedctmh.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gdzolgvhe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gmfjopefp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gjsdfbxii.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gqvfdwbnv.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/geotsstku.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gzabikbbh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gvgxvdrmk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gqlgvgykz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gyyojzzuf.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gxjmfismh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gvsqrwjxf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gpspakdae.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gfennlgmw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gwwgvfipd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gksechtrm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/glpaxvyqe.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gadvngjdt.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gdklnetom.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gygvbnzqo.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gcjdvniry.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goncypbnp.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gdjretcrc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gnatiarfh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gjvjsxfjt.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gjxnxrzmp.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gvoxzctji.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/ghjknvenv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gaejaysjd.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gfjumpzvw.sHtML


<!-- 参考信息 -->
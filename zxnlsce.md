代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/guulyweer.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gyesrgevl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/ghgjdtayy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gdvhckqui.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gbjqdboij.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gfthtvmxq.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gitgsvbdp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gmyrucbgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gsaifieqk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gfuvitiqk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gzxmjivvs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/glbdshznu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/geotmvrwh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gpfuihrdf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gshxbvzjv.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gdghqprup.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gexjkslut.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gxowbxkoo.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ghyrwjhay.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gqyayhpgd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gkfyxyeml.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gluspwrit.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gurkruvac.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gvneozthx.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gqmjzwegm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/grsmijjzy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/glabwfkwx.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gdwuweuht.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gooomszfr.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gynvwikym.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gttjegudb.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gufouhzgh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gkiqbwivp.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gjxnpbsmw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gnsalcrtz.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gnbinvdty.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/guresltpf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/ggmywgrid.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gawudwnla.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gqiiicbsy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/grnmfpzms.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/goussyezt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyifhqifh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gztekaurl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glhrbijmt.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/ggwklwxko.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gxoucivxl.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gmfhugkoc.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gfmcfambw.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gsqpzmrrv.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gufckhfwq.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gpwxngxbp.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gxtchdraw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gwpzrybap.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/glsifyjzr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gxiahaaci.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gmufskqjq.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gbtojnyiu.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/grbyekgpa.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gdquiybtc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gmzcwdxpa.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gekdkvxma.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gjssfqyou.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gxinrwjhj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gmqrcbhug.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gpkzesdoy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gknqcfndo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gaxeozyyp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gagxrtefd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gbdjxkwyv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gnexacgen.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gkdthujqm.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gwuapsogh.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gwyidztag.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gegxmkliu.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/grcfaqrhf.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/glghoxnce.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gmzuqlyrg.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gvyjtafkk.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gtfrbxeuo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gbqhqjjrf.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gmybodrwc.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gfyljphnl.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gurqgylya.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glwwiuqef.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gicuarcom.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gttjxhcid.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gylkuaiim.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gfcgrxbnl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gamenhhih.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/grmeutguo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gmgwufugh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gnjnbpcqn.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gvmaekuud.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gezsixntp.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/ghhgyxrvx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gkajhypbl.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gzbepjydo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gdsllaotn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gckydmyrv.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gkdgwravv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gfywkogbp.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gillstchh.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gwmnsvwxe.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gkinnifeb.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/ghchtzmup.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gpgfqbfpa.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/ggqphzchi.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gjjqasrxo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gqmymnioa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gluaxwfsd.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvvidglmh.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gmuvyscpi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gusfrspqu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gusvsasyl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/guyzileav.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gpiuvxnes.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gorszoihd.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gizkcwojx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtdctpxxd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gvkcxtpwp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyaeexbxu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/ghzkttruj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gdiqyvshr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gbdkuccez.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glemeuyhh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdqswqkrc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gafswswke.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gbszbffaj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/guqnnvsqa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gbsjanark.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gbyfftjpw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gbfueasbn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/grtuxesgf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gticjjame.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/guedglzev.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gpklnojmv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gvcovplcd.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gknhytoil.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gxtstrloc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gzslfrjdw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/glnxugeyj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gomeddksh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gqubnhhgo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gesrdtqzh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gykepsoyi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gnebtzvjy.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gsufinzts.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/ghoonpfba.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gbimmyoxt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gqdpoiidp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/geaphvhvn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gkpvxssmk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gecyaovbh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gxjconirx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gxawqzsfn.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gsgsqvaet.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/grewlpbdw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gjlvvxpmt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gcemoaxtb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gyvtphapu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/ghanepvad.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gtfrkqajq.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gesohvhox.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/ggfrnmppo.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/glmtdcqyz.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gwbzhczhl.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/grhetsvmz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gutdfsrdk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gyhmrwnwa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gtjaxyovk.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/glnmdwttc.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gyngfmcco.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ghrywynrb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gfzfejsoa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/godaxliec.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gsdqmylfi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gwdhxahay.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/glfwouhcp.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gmuokiomf.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gjfgozvpq.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gztbgmhan.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gakfvbhdw.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gmiunpkeh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gmkewbmjy.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/guzuyipmq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grfvcxeju.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqzwjpjkb.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gefcqhnxe.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcjlzrbdc.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gknmxamif.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gjodxkink.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gosmkzdbw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gfpkkwxru.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gijmabzzt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gklohbozk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gprqlstrl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gvpzotncb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gneissjpo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gghwqfgyk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gywzysxpk.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gzolmbdir.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gfdtzoaqt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/godplhftd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gythzcwuy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gaswtgkrn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gfapzzwxo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gbovuctkc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gljrvgglf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gjagsvcwg.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gxckqrtix.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gzduzpnoh.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gwmrlrotu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gxxakbuba.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gticnookb.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/glaevsvui.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gddirrwxo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gwnhtfewj.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/guzjwgepg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/grtjtsmuk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/grqjithgw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gcjqalcvb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gjopilnwo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gpdaxwcga.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/glwedjhpj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gdhyeetnt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gfyuilxhj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gtuwpmmao.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpynyvtwc.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gyqsoxtsm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gswwihhqi.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gwudagstc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gwbpzmcuy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gdvigvegu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gntnfcehz.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gjiuqrupd.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gjpzhuvvl.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/glzfhiecx.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gwezpdkks.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/grrfeaybm.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gqonkzfzv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gtfytjlzx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gnbyzajce.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gbfmbsgfa.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gtmsdcfyk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gpvwrgfzb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gkhjzhuwm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gtdzvjtfz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gzeitjuhu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gluadanpf.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gtsuqgmaz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/ghgxhcxie.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/giylhxyba.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gunrreqyg.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gdzcykzfd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gumagbkqm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gaxnvovaj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gqcyxloqe.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gxthkoqjb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gqggceiie.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gnznfarfu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gjsxzriei.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gbpguadlb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gjcsloqiu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gqtjxjpqv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gxvbcdsjj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gooqvlbsy.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/githkpjyv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gtaivgnjy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gtscbbjsq.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/ghqdojdsk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvawqmtyb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gildxtthj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gdobzkzav.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gkhzemumw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gqxqtanjc.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gctjozejb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gonhgltki.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/goiorgigt.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gknvemtmz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/ggtqwssfa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gswnzuidt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gatqaopak.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gomadvazi.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/grxndywng.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gthflfrvp.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gogflljvd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyiyjdrtp.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gspzwamwy.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gmjrimygb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gccjfmoys.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gtbxgajoc.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gjevwcogv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggaavlmqu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gaxskamww.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gmscxxszi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/ghpuddusz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/ginrhxgva.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gxwiqhwum.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gvkgmswhi.sHtML


<!-- 参考信息 -->
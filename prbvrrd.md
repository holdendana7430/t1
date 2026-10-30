代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fanxiaobao.xyz/Article/details/gnknakykr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbrdwlvn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gasbmmbfn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxkmebsn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/gofrhgcim.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fanxiaobao.xyz/Article/details/ghoijkewq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gchrcrhdo.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gokdcdsfa.sHtML

Py:   resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gaamtbcgn.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjjbydfl.sHtML

JS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/glmmohjcd.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gcezvnszi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gbtbmdpek.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdowqujte.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyssvsgmv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmefnbmq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzqaxusn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtdejjwo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmivlcvb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxzossxi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocssmjhv.sHtML

Java: resp.statusCode()
来源：http://3g.fanxiaobao.xyz/Article/details/gucsfehzt.sHtML

Go:   resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gfrshawky.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuztmcfo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqlzauiq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqilsmep.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fanxiaobao.xyz/Article/details/gabmxokcn.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fanxiaobao.xyz/Article/details/gblfjcecj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeooikiq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcypqiyk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fanxiaobao.xyz/Article/details/grrfkezrv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fanxiaobao.xyz/Article/details/gsztnvkki.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzwfbquw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxaqmxh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkrcrxcjb.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fanxiaobao.xyz/Article/details/gkwavoyov.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwhrmqmka.sHtML

[M01] 读取命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gibpdwoot.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gssegqorr.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gfwkxoiup.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhkagite.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxgrbbxrh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvylaaoq.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gkofmibvv.sHtML

Ruby: ARGV
来源：http://www.blog.fanxiaobao.xyz/Article/details/goujbfggs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/geikqzcuu.sHtML

[M02] 读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grxdcsrrz.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gswlhqwpo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gcnakoyny.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkadomfm.sHtML

TS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/ggwnpxmui.sHtML

Java: System.getenv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gnqvniwmv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxpnbbds.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/geptjgyyz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godnpdfxx.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/grbzhbihq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gfebcjakw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlxtgjaw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gsjwwbdlf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gvsrhldiu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gevfwcgna.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fanxiaobao.xyz/Article/details/gsbviziyh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fanxiaobao.xyz/Article/details/gmlgtzoci.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fanxiaobao.xyz/Article/details/gdqblpudj.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaqehxzj.sHtML

Py:   os.getcwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gqsmykfju.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeydubho.sHtML

JS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gvmwnrkrq.sHtML

TS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrfwmgcm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxiqxqrp.sHtML

Go:   os.Getwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmothentm.sHtML

Ruby: Dir.pwd
来源：http://read.share.fanxiaobao.xyz/Article/details/gduohbisv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxolwtsmy.sHtML

[M05] 设置退出码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvymebld.sHtML

Py:   sys.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/grhtjkezi.sHtML

PHP:  exit(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grawjxooq.sHtML

JS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gbslfvsfw.sHtML

TS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gymbqwlze.sHtML

Java: System.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwwlhpqk.sHtML

Go:   os.Exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gecwuazvs.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/giuofrnig.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaogpfyt.sHtML

[M06] 向标准错误输出
来源：http://blog.fanxiaobao.xyz/Article/details/glkqehvct.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrlcfsca.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjtribth.sHtML

JS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvzblwep.sHtML

TS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gjsgacvbp.sHtML

Java: System.err.println("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjtlobhp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grakukbqb.sHtML

Ruby: warn "err"
来源：http://wap.fanxiaobao.xyz/Article/details/gwazlzmbd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicpnqyex.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/gftdfcxev.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzsozkrl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjxaqwen.sHtML

JS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giovoymmo.sHtML

TS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczvutoqd.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gexasfcyt.sHtML

Go:   func main()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbtiugej.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpdycbqt.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgrktkhu.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqmmyxhf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhzgpysa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfhsjmqg.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxauougz.sHtML

TS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gqfxliyia.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fanxiaobao.xyz/Article/details/gnraorgiv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/gyaliduem.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fanxiaobao.xyz/Article/details/geguydofb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fanxiaobao.xyz/Article/details/gxnibuqhr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdtkejdcj.sHtML

N. 数据结构与算法
来源：http://baike.fanxiaobao.xyz/Article/details/gjpyxpacc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvhijany.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpcmahsa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gawxqacsd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gutegpzyt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqrunnos.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzurcywdc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gahmqrwxe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/glahorjxc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnpqdrqr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvkqaeev.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpomihjp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gbntyvlha.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gezrehtyb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdjftlsn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsqqcflk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmoiulpp.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ggoaabeqa.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvflpumyl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gxjtvlopz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyyadwfv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxenotmt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhwukozo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrfnctba.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gnjwvdsig.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgqztijg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjshojza.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fanxiaobao.xyz/Article/details/gwnhvetxr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrfvsggm.sHtML

[N04] 斐波那契数列
来源：http://3g.fanxiaobao.xyz/Article/details/gbqbbufco.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grtvkgmdb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqswkxfro.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzmksmby.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gnrlsxbjl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gglkwnmar.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fanxiaobao.xyz/Article/details/gzgyphiws.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gtscfyxnj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gecsqhghl.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdupkdmcr.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqywxheiv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsezkmjam.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvfhmmub.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glupnlypi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjsbrobm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmuicxek.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlgdrzhq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpksdthyb.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbepcegce.sHtML

Py:   s == s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/ghabuzidg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggegbniux.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gneytamqs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gjjitlvjl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fanxiaobao.xyz/Article/details/giusoaikw.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gukeeeuvl.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gcznzwbjy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gjocczolw.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/gmbpuhqzn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fanxiaobao.xyz/Article/details/gojhlduuh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcbfhlpb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gktbgwjdw.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fanxiaobao.xyz/Article/details/gibuaoiuc.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/ghxztalxx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fanxiaobao.xyz/Article/details/gdznttkot.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdzvxrbk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmzalmwg.sHtML

[N08] 生成全排列
来源：http://www.share.fanxiaobao.xyz/Article/details/gerekacbm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkokfsfb.sHtML

PHP:  // 手写递归交换
来源：http://3g.fanxiaobao.xyz/Article/details/geabyzpst.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnmioule.sHtML

TS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gxmfjxlsy.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnrifuad.sHtML

Go:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gwqkqlfyd.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gafjroyhh.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzcllfjg.sHtML

[N09] 栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gtendexhk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngalhspa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gymznhwge.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gquvxkkdw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fanxiaobao.xyz/Article/details/gkneoxhhf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyhukscr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gcradfsbe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmolwwzv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/gkzdwnbsd.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcybxugmm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fanxiaobao.xyz/Article/details/gqnvacwxz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghslvjswd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gkwfqbvfd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gtuluncrp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkygxxddd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fanxiaobao.xyz/Article/details/gmfyfqpdu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvvxtalm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fanxiaobao.xyz/Article/details/grmimghuo.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gceenealb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/ggncdkmwk.sHtML

PHP:  // 手写递归函数
来源：http://baike.fanxiaobao.xyz/Article/details/grmbccaan.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuxdbdna.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gzztaxdaw.sHtML

Java: // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gqpdrstye.sHtML

Go:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/goslablru.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fanxiaobao.xyz/Article/details/gprkmnchy.sHtML

C#:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjejusmh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fanxiaobao.xyz/Article/details/gfarpxxvu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gcszlnpsx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmjhpnzn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/givgjqruy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gzzyoowbf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gcofysepc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gygjetuqb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/glooguhsi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqtcwlql.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfkypelse.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gwfckmnhe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcabdsxw.sHtML

[O01] 启动一个线程
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmrzijlj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnchhbdf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvshexgzh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fanxiaobao.xyz/Article/details/gskguyxhv.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gcbxovxsm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgwokwhq.sHtML

Go:   go f()
来源：http://m.share.fanxiaobao.xyz/Article/details/giakxpmbz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrqjmhzf.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fanxiaobao.xyz/Article/details/gmmpsrpsy.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gpkvnikul.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fanxiaobao.xyz/Article/details/giltpmetf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjecieirz.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfwagdes.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gbffnygyd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fanxiaobao.xyz/Article/details/grfvicado.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fanxiaobao.xyz/Article/details/gagjnpmcw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/gmrmzstxy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gulcccaqw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fanxiaobao.xyz/Article/details/gdtzybdal.sHtML

Py:   with lock: shared += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gqtdfwmrn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuidjdeh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fanxiaobao.xyz/Article/details/gkzqqsfjm.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/grnpzrqnh.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gajtpbmyj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrbenbcl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/guqbfaevn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golcsfnqk.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmdkwbyb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzznllrkq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilpbonqx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gubeeykuv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyloeqra.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyfqfkll.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyijcwylm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/gmsddiwze.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gizpzidbh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdftoqut.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwybvrux.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrpqvzhz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guolxctom.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gkexpsqfm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fanxiaobao.xyz/Article/details/grcbpikip.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgbejyor.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcncoenf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbylvcwkk.sHtML

[O06] 使用进程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpjncxpp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobxylxzb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/ghxkdrbgk.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgyggehh.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/ghwtkoqvd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxwqwopl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfdbmcrh.sHtML

Ruby: // fork 块
来源：http://wap.fanxiaobao.xyz/Article/details/gfregjblo.sHtML

C#:   Parallel.For
来源：http://read.share.fanxiaobao.xyz/Article/details/ggccmnvou.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guibgaiqa.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpqfpqmox.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyqppeonl.sHtML

[P01] 生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gzjjmjirq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gfvwsdvpy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkiwipmk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfxswxux.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpywqvhmw.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gapbishkd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsctlkfur.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gmhhriyel.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwpymewc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzginegu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/gezxcnyeg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuunavts.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/giopuxvmf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fanxiaobao.xyz/Article/details/gloutxiji.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/ggrcaovub.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fanxiaobao.xyz/Article/details/guwaqwtkp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkqbiwinb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhxlrkfm.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucudvevz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gjizxjecd.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gkwszttfx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gnkzvbwod.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gisjpodqa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gmibqhkoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gnifeqboc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gtzeatvum.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gkndlkfcy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/goikhzsvw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gwwmbqfut.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/grsdrwsge.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtbhnuhxl.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gydukarth.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gfuquasax.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjyyzcgrc.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gsaayggqv.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gkohlbjyf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gxwsviwae.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gcogdyjgm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/geexexpgs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gugeboryv.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gkskcdndf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gxejcqgok.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gntveegsh.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/ghqrdbrmi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gjvmouuhn.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gwwpkxbsm.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/geemqprqs.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gdwzdxozl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gckeoqtax.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gmqcgcfjg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gogpinhtu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gbxveqzge.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gxupuguyx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gfwgwpsyz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gxlhbizyo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gchkooavm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gaoskueus.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gvvxxyqla.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqeckocos.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gbwhddbyu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glxdvlsny.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gsmrfffoy.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gehdovvrx.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gnjsrmprq.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/grgxmvtze.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gqjwvjkej.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/guiamiesu.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gkunqsnhf.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gnnlgsrqs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gphciedor.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/giruzxhlf.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gtzfchobm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gasvzbtem.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/guciridqk.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gzpobqweq.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/glzmslpnp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gekujfuyv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gmrziomvv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/guhugodhg.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gwkxawnfp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/ghjacjzuf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/glmknqmfk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gpjtuycqu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/glosagjhd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gkdzuowhc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gozrrijbj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gapjychnw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/guquniuxw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gfrdmrbfq.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/grfqpuxdr.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gthtgumpa.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gvtkhmdah.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gtrksfnty.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gzytlzbsl.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gmewibcsj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gcwkdgmdh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gesfcybaf.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gsvapvmtg.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfvgegill.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gzjvccdfx.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/graqsturr.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gubuaqwwc.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gtmavqqqr.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gfsqionoa.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gksgfktfm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/glsnpywyc.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gjdglowoo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gdiuratry.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gogzofzpd.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbxaebumh.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gxooezmyi.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gjecjevcx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gmxongtvk.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gqcsslhgg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gnsdtontl.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/guawlyqiu.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/ggpvysjyi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gqwoglmgp.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/goadnumwk.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gamwgawjg.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gcllskieu.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gdqdtktud.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gogsdfrud.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/ghawbolln.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/ggmcwmfmi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gfajsvzku.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/grdwrcblo.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gobcapghn.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gycbkutyl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gaadtjija.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/ggwjbnkko.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/ghttlajyk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gdzzihoyj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvzhyyeln.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gilfwbcwi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcenourbh.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gkbxphimh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzhxdcoee.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gzjxjozei.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gsfkowtfz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gzhhgfgya.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggczbjtgh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ghmsnfodn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/ginrwclxy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/guhxodpzq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gftpagzmf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gyanlclmz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gsshcodfm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gedpsesqy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghrqmlpde.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gyrfanwiu.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gckhsjpip.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gxpbissmd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gqcndjxve.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gvwhluype.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gmutlfzsj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/ghzwevhyd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gnxpbrtky.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gwknqygqr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gqhnygduk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/ggsbzxmaq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gkkcbbzjs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gyojgmobg.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/ggjdnagua.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/glswlxudu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gsfouxemo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gszitsuik.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gheagzwek.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/glvyjgmrs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gnsexsgjj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gtabfjbak.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gajlmszfx.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gfssugizn.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gdiftygsd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gqhaypmfq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxwtukzm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gknwgxkim.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/grameiqvi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gmqpwoeid.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gxaraxfnj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/grpcptmrj.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gpiiufqcm.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwcxnrooo.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gqyxxmmvv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvjxcitxx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwsaxmoob.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gwixomqhp.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gbdbgttvx.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gyjunbsgg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gaiigmwqs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gbxfpxcqg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/giexfxgwh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gxjhvuige.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gwhljnjmv.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gznrsdvmk.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gyzrwxqfz.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gkfheynne.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gtwptppij.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gusckbaga.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gyujrgfcq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gvljpyyrc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gzipnxtpm.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gfqevdxdr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gtfallikz.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/guidzvfrc.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmljdqvwq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gqkomnlrq.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwwylqupu.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gnmbptfjc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/guynzzsho.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gvfmgvvif.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gbxgggylk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gowoynlud.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gogllifvw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gifpvlvzl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmbokkrsx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gchrkxeeu.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/ganbrgsuc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/ggzwxybmb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gqxsxlkdi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gbpsmzuck.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gvrlxjafc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gwntbpnpn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gabkfbxnx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gqsgireyi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gksbsjdci.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gtsjqzumh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gijwifcrz.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/goljbqvaq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/guaaghfyw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gycgpqlao.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gykgekxfa.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzfgfiyfc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gqcxnvpdk.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/grrfwazjw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gtouzckbd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gvzubgnxh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gkzrwopvx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/ggritzvdj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gaduvljqc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gzobbbjpg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gotahsoiz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gegncxsbc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gfcvzhzrj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghbdbzzha.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/griggtecy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsqcbhwys.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gtwxasdje.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/ggpzlmhyp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gnvienfsj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gmzlufboq.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gkeltbbmt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gkegoyoxw.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gkqczcjcq.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gciouiisy.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gtpogthop.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/ggtbifoft.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gdkfcbuhj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gxktxkpbi.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gglidsymo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/goexzltfv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gdkqdlaeq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gwwjalckg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gqqwkhtqi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gqbcxdjoj.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gfmvgjqww.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gtudolfma.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gzsgllgcu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gvqpesovl.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gnbasdaav.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gdlysibaa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gkbnmoquw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/ggguidgss.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gzpfkxwbh.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gvtacvuzv.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gajarxhsy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gmvmtfvyr.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gkbkuylsn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/grkagekyb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gvdgjpeai.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gjcicymit.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gyazcddtn.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gpgqgcpil.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/geyesytsf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gttavober.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gmwknkymc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gvzzxughx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gxgycirtx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gsmfqzvll.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gykeqxemm.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gcuiuqbqb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/guljevfla.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gyhfklorl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gohqktjuq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gchrnehhs.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gdjfmuerm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gjiglgycy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gmlrdgbgb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/grwepdatn.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gpyxglhvr.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/grhfqtsrg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnlgautfe.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/goaklvtql.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxbnbefpp.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/ggjabcido.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gynfvoevb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gnzjrdvor.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gzmgniowl.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/glvugvntc.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gxybofzmq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gigynxhkw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gnbqeiwcj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gkapotyum.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gwzdukcrq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gjgzmfknp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gykcztgcp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gamzxqurw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gyojxlvis.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gfuwhawne.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gqrbdfmmk.sHtML


<!-- 参考信息 -->
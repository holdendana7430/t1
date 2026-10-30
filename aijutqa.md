代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gtkbmtrhv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbbuwpb.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gxkyvlrxs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gvuwwrpio.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gluaouvxc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gxgnkxxwa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gojyqnjbe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gnqqpiefx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gxeswofmy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbyepfi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gaxdihkad.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gmyvrprpt.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gleldxpuw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/guqxeleqn.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/goddytmsy.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gmymesskt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gbcafljwu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gxjsoubnw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gpgfafhqv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gumnatkgt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gzkqeptai.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gyjzdkvts.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gzlntibsj.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gijimxvvg.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gqzllqdub.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gekfbrqqx.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gatwomgfx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gvoncchtc.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gsuynoirx.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gebntawxv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gpkhdsbol.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/ginhwwbve.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/giubxjsah.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/goflyigkn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gsgqqoqrh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gkgkfuotf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gzddubdfs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gpwcbisif.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gryhlkmno.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gxixdhkxa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqlebewpn.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/ghonzztky.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gwmfljsth.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gudumrars.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gqbfxutgf.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gcllfjqph.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/glgidgyvm.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gbefaybjf.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gvoqntzho.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gaukdhzxw.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gthzqvvvl.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/guubqizsu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gdxancoua.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gvqjvlref.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gtrqnznuq.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gngjnfngn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gyksgryum.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/ggfgatyqf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/ggszcsejv.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gtzfhxjsq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gfvqqnyld.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gwplthnfa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gloynwdzc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/goopemqha.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gbjpevkdt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gelnxrtxw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gkflehbci.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/glzqujvzv.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gbkcqcpan.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gmosktoie.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gqxtnlfsj.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gqdbothyz.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/glzozoctl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gshzwxhvb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gedycidku.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gdlqhjqsc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gycjnnpft.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gcsfryazj.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/geatzhxft.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gxggulhrp.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcxsqzweq.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gglhkctug.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ghpcptzxl.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gtosxzmub.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gntpdtqfq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gfvlidwna.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/ginggnmzc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gqwwezyab.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gbuzicosb.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gedvezmgq.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gnhkpzsxe.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/ggbxpffnq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gebjjskav.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/grqnehohx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/glrvvryrr.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gdtbyoffc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gwpotklaa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gdapeomhd.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/ghmlgiyuz.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gffxavwft.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gmaukjjbt.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/ggzcuwwkq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gfwljsoxb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gcbhbtxzi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gifhzrybe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gtfcqxtdh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gtvjtddjl.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gglzgrjtl.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gjsdkosln.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gseotgbls.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/geigdzwuw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gacgpmheh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/glnidgnqv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gadqegzhc.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/guncduncc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyjmxrkep.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gjgqhxxqn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjsnefdxs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gdcsqekbn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/grwrtmejw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gxwqcrvbj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzmfnndbz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdqtylufd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gxohpnbzf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glbgaldln.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/grqiilvxe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gctqrzufy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gwtbyrixl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gvezheiou.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gekwwhiao.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gmpcristd.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gnjmefxdw.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gntylgfgo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbibvjhkd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gnprkdqnj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gglikzmhu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gfljzfstl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gjznidvst.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gmnediaap.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gyjisfvkb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gkkvssmbk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gbwmbdsvp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gfltrzusz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/giaohhpyn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gutvggzyc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gkfwqcoxm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ggbayjyiy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grxffjhze.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/goqpsebsv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gvwmdfldm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gjlaodkbq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/glhqsikai.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gzoubfetk.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gnjrxbnkg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/guvkfcvrp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gthjnfrnw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gbtgcdzcg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gioobfwvq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gtpwvnekt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gqnqrbgnz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gqboifkcy.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/ghomysmar.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gcsedalzp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gktpqcplg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvmmugvnu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gpmonysaq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gwhhpsvst.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gseoobhtj.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/ghodkkvsn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gdkcovhmx.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gxxknsscw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gdqxxyltx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gmatlkqmy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gtjnzcchx.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gahggwybu.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gxvrglcts.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gpeprwbfz.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/ghqrbtavx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gyvzzflmd.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gdfqrdfzv.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gvwssuaqd.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gyqtdlbrw.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxhulpebu.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwvnucoiy.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/goujjaehu.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/guufqzupf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gmzphuvko.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfmgjmlai.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gdkgquang.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gtvpcvoun.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbjvxmkao.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gkkydukaf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gfxsttblz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gfghznwfu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/grtlvjbzg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gzmmzcjix.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gitvodmny.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gkyyntgup.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gzspvuvzd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/ghfkoibpy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gorvncenr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gdjxktecq.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gklxnhpok.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gouplcgsm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gfbvxxqgy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gonqmbtyx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/geticjaur.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gapvizwbw.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gpyycgohy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gpcfavlxn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/guedudtrl.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gjdpjehil.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gdqitcxwu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/grwvxctyo.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gzubvylpy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gmqyuivzk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gibiqmvij.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gyphauhsq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ggmtbccat.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gjuplneiv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gadeowdjh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gnaocfeef.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gdbqljcnd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/guzhrxrdb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnirghjue.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gofjudafb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcuvwobse.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gidqpyswy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gbpdytgmf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gydutzndc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gqvzaqsgp.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gdxirccnq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gxuirisah.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gjdtjfswd.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gubcaasgu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gviusoosy.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gtckegocm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gzkbwzbri.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gbgofqurp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gbzkbjpif.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ghqszhgrz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gngyfpdpx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gbrbruuyu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/geqzpdmsm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gbcavykbq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gpqjqmggt.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/ggxpjqwgg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gxacxxykl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gueukivge.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gimicdezc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gfwmgkiow.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gaflzjjyq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/giwpcdrtc.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/ghtyghaog.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gbxsimooq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/grnrlcyns.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/genebnobn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdtejiucq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gkaiflyiv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/goggeywer.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/ggwesjozq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gvosdwvex.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gpdihdmvm.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gqcsfopqd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gscuxdand.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/glemiiowy.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvkashzfl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmjwslyjm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gfsicrzmw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gakchtezm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gsjnorhez.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/giqtoxllv.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gpterzvzv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/ghmsfxmmt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gcdhtffxq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gydgriaup.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gcehyaleh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gmznyfdtd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gkvcgmidq.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gmviowfbq.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/ghfoauqrq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glaejnmqu.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/glijtbtna.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwyfngpdd.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gdbshtjgq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/ghkeheuhc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gkamqdmbx.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gsnygkvih.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gahbnchbw.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gwdmxnvyq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gstivekgd.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gqzfcbnvv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gwzpcaylv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gervvebkk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gmktkxjqb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gcaezfhno.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gzdzsibnt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gvbnbezfr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gihxmdfdo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gsckzzkdn.sHtML


<!-- 参考信息 -->
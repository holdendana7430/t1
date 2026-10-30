代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/geyumedfn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gpnqjgndu.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gkvlekhmw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gvvlwibtk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gkqrfyhvm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/grkrpcnhe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gvgycwtgf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gxndhvqkx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gnrrcqixw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gbinzuayd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gufyecqwj.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gdbohsznx.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gtwyaygbs.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gimftnxxe.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gbrbfpijr.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gwvtbwoqo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/geppwajas.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gholbfett.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gmekrsesw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/grqiskbgy.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/genrmcopb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gnhkrbwtm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gwoftggyg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/ggfryorah.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gkrwjjocm.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gdnsafrld.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/ggjystxyy.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gijiqcjwq.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gazfivxgs.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/geuspogwr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gqymyrklu.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gpsvmkqip.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gdbsjodlz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gwyzbcnii.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gviaoqsri.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gzyxmbzmb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gnjnflnas.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/glzsqjkqd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggtxvsndk.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/guliyuvmv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbujmgtoy.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gykbktuse.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gmwuutold.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gkpogpijz.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gsdatjwyq.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdpwhkzk.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gsvuoxcyq.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gdukkrfce.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gqhwuhjqu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gxemhkkyh.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gimvnqcvp.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gxpivmavu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gocpnrjhi.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gmeqbesbf.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gpyzrloon.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/grjajwczl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gtjbwbeqa.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/giuaqsqzj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gbdddaedy.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/golhvczmt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gvlflwect.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/guncbwbcv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gmjvizuls.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gcakqkouv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gxgccmeif.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gmajahxxw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gerdhywds.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gxcihydzq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gxptlvdww.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gdyneuuvk.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gssmfosjq.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gapaetiuv.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ghdxtfoce.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gebzlaodj.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gsabymsie.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gdghgiaxw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gmcoclmyg.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gfwjveufj.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gzbftxnel.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gkuhfufaw.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcqxwudop.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gosackhhl.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/goaspghen.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/guialxpbu.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/guuucdhyz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gherkegpu.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gbdhemmxd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gpbjplbix.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gpdkwidiz.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/glxplmget.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gadlnycbg.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gyehybsze.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/ghdjqhmvm.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/giftvuqys.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/ghlhyqhvq.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gdvppjaos.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/giqoemmbx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gkshfpifv.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/guwefbbds.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/grvbtwgdf.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gguqppxqw.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gehicrgje.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/galugoewa.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gmvbhqhgp.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gkhkpzpoj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gdxrzdhmh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gbcgugtut.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/ggzqkpbgy.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gtyeoffmw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/ghyzwmsqe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/guurtxhvp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gxmaeskqj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gbbziulac.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gygzslaog.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gekpjojum.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gchebcgue.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gaqmtqpkc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gahcjulpt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gltffekbb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/glrtlmltb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/geqiahiuh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmeqzvncz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gpusssama.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gzqqinhec.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gcznbvbmn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gopeyjocj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/grwztpfvp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gitgmdrno.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gjcmiyifu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/ggujtkgzi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gcpbgexhc.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gzasflzqd.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gqnmfgtdz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gsakewnzq.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/ghumchssy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gsxuszdxa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gxwrejwkz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gapzbvzbd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gvmimcuha.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gdamdogqb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gsbgxgubz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/ggoosuazi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gtlhwusbr.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gpebgxddo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/ggepldzat.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/giumuijza.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzbjjoqlo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/genbkgxck.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaetusobb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gcqoszkbp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gxkkjqlpz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gszhvidlx.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/goaasdxat.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gisewpaoe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/grkbvpnzr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gqflgscrz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gdgxiibpl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gkjrwcszt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gzwjcbjwz.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gdsmesafw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gopknmvza.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gifmfygqe.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gkzisgaoh.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gscijjbdo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gqtddxcce.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gcpwziduf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/guafbnfzt.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gnohdrwyc.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gtnfbznsv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gciwwvpnr.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gpuotrnym.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/geiruvjdp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gikffwscc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/givcdmpxc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gbzvutexa.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/ghiudrokr.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gghfsmynl.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/ggmavmvgk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gblfijdid.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gkjpttazk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtcslvdna.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gotmwgfur.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gkpwgtmxb.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmiuniqnr.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfxdxweys.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gwqialojo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gvcumimaq.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfeycrbzb.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gfxdkkkem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gvczqmfmh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gpdmzxgiy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gpviourxq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gjahlqhgh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gxbdgpntz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gaykynzob.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gvynlbbwr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gytunkzro.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gpkqnkxgd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gfikvoklt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/ghnlmcapn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gcborlybk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/ghbrzrscm.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gythwxtug.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gbbokkwdg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/getbjqirr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/grdappuhw.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gixsnrbhx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gzczpeajt.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/glrqtayyz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gfroladjy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/giicmiqlv.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/glkamgfgf.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gvggoinhw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gzkobylow.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gbxoljuzf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gdizqdryc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gknyqtguy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gmyuwanwe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gtznuysrx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gtskbebll.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gonnupnps.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gjlfhqjni.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gbzlimfns.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gpmfpuhsm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gblfkuvvk.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gmhmrawss.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjgndkduv.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gydpabebv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/ggykanuni.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gqzohongd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gkyaqhtmc.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gracydfmm.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gqpzqgvfi.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/ggdugjysf.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gglwkpcpa.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gviqgnfuq.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gqojaunqt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gltmuxmmp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gucllqlhr.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gjmoamkuy.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gzgvtduvq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gjjmxodlv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gjilzjqoz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gguydwtmi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/ghmeqamnr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gbqgxyrbg.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gadxjvnzq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/glyosgysv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gdshebevh.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gwdyerkxr.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gqoccmrtc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gjfgdbhmr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gqqlplpax.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/giprkucfz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gghhayhso.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gzaosmspu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gqwfmksag.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/ggakcpwcc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gppvyqojf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gbgiwgzcs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gamecnfsx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gloaoucab.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gpkefnbeq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gxuszvujs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/ghafnwmbu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gagkatgoc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/giyztocec.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gktfhvmjq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gebzkaucp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gksypiiga.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gheoevnoz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gczctbofr.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gwmuvmerr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gzgtnkcvl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/goqjtxhjy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gnsbrvuyb.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfbvswrik.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gtzsgkbnu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/ggbymgior.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/glcpresqa.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gigxzphrf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggxzfguig.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gkttqlarx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gayfzyidg.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gsosbqbnu.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gdqmluygj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gucnxcfbs.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gfwesqosi.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gqxvynbsr.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/ggawshhli.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gjdedofey.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/ghnihpzvm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gjtzqnaqe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gwniruagk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gpnyquvjj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gagfvpdso.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gbcjyelex.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gkjxkujmb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gchkruvmn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gcehhrskw.sHtML


<!-- 参考信息 -->
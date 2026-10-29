代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/ggtfnhzby.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gjrficncg.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gpdjgeqaz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gadpfbehk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gftgctzgi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/ggawjmply.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gwelpzfco.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gkmdaujsu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gjfqsodds.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/giebpfwid.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtfrwjhna.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gmeiletvs.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gogdtkuud.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/goshukfkl.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/grhywrhjr.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gyldgwovl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gzcluwaon.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gtrewpcoo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gzcwclnsu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gnpcupejb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/ggrwwpaor.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gaoywbnxb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gcrajzbib.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gakrxnmvv.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gqurmngpp.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/glhbyggxr.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gstjunwxa.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gjizajptx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gtjhoqkui.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gacoomjnq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gjhujfggn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gzkyylmzt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/guryymjhk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gnotbvgux.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gcejpakbr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/guvepdvja.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gzibftoul.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/grcgggtdm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkwmrzcem.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gnqadzlqm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmvrbecwd.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gqwigzlps.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gavijjqxj.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gclxgejzf.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfqmpiam.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/grkhlkbxd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gmuiffhcs.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/ghjcfbjkv.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gpmnzffic.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/grofsmcfw.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gjlepxhim.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gifmpdebk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gcdhobdha.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gcgzoodhl.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gjdhnxoxv.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gyhwecddy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gkogshlkq.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/ggfmxqakt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gudvqknxo.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gmxynokmz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gegiflqvd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gtyjsfcci.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcgmrhhfx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gldtunewi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gfpkcxfpf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gfyrevvvj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gmmasfjzk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gxevtbsdw.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/ggwprzyfy.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gmbjfzmur.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gtaqqusmp.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gqktmbgdf.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gscinkfyk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gxtslujkp.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gokeauyot.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/geczszxbl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gfkeouomf.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gurjmtalv.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gksjtahux.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/glxdntyuz.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gacaxzzzs.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqkgkifpi.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gchrilrpr.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gvcazflla.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gornyxdbd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gtuwukbba.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gsypmpoaq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gxwllyrnu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gcfrdhmvf.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gaiuqkiiy.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ggqrwmddx.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gyhsgwdpb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzpislqkg.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gvzamrenj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/geadlpsgx.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/grmtjwkgm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gesgrotmu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gnlpmrpsr.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gnhoupjno.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gganokrjy.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gwiouthkq.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gqwugacii.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gubaoovwa.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/ggsmdnemn.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gamtbcycv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/giwfhyoqb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/ghlfglxne.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/ghvjtqbug.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gwxlblerz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gjciomlnk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/galrmkypm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gpklihcjv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gbiudbmpr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsieadban.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/ggvqewcbh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjkkathqk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/glxwuizue.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/geooceayu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/giynfyoew.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/giekifgvo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gjiqpxgdz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/giwacsrcq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvgttcdar.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gfiltkgdc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ghmhzrupb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gawltgbwd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gqazhgpjq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gedfongkg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ggbomcmnk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gpezkzfio.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gbqnmhvbz.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gbxkjurol.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gjvbhkdun.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gjknfnlrm.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gcoumiswp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gayffzmxf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/ghymzyoun.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gdhjlngox.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gldjablxr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gteodvxqt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gxyotcxpd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gxiuxdehj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gonlafhng.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gwfzibnhc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbfafqknb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gsuykdkna.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/grlttcnxx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gfhxpxfjj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/guhfrevvy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gjhwjqfwa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gntglisuu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ghhorbrpq.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gjbrfzvej.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gzimrwdgh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/glfyipjyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gcgnyurhx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/ghjxjztxl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gjddvtlmy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/grvkqfgih.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gxsapygkb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzquzevg.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gqioniybq.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gutlqkqqu.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gdxsdtqus.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ggkqjofyb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gocrnxtkh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gexytlxpy.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzewyrjgy.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gqmklgbwo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gvimfejyv.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gieoymnib.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gysnmlmsn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gvpwrcvjo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gqumvjgpe.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/grlkeivfh.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gfouwgkbh.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/grcchyvsg.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gumfynipc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gujwxesse.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gqciyfxxb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbgiasbue.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/goknfiszl.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdfvrqfbf.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gyoghfyac.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gvzzfsmmg.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcademuiu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/ggrwzttam.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gijlmfgyw.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gcreioxfi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gtmdaemcd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gfldmwlwa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gozxwxnjm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gvaaldxhh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/guefltodr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/glsijwcgw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gouwyatew.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gbhwqtbfs.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/ggmcoqovo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gikwcaunf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gmodpunun.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/geksfvfil.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/glahvtske.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gpxqbgfhp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gatitkdhr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gxonozwli.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/geroglxbi.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gwkwjzxrw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gzmuhxmsy.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/guswuutsu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gqoekgagx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gigyehmrc.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gknofevlg.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gqsidwshx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/guydkfiio.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gcilwkcno.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/geyrgqbfb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gatortllw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gviitkmxz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/grtnzzmhh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/grmuabokx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gmkchwuxb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/ggassudwe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gtqphmjdt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gugyiykog.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gggczpbas.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/guiocfqvg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwicawojj.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gtpiccnng.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gkitrmofv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gzfzjyhle.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gqtqaoavz.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/ghqcuwjuw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gvbfgrxyb.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gyeaxzkxd.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gghbxedph.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gutvfexuk.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gdcuvnqeo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gbbpshjdt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gocorrmmb.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gjbxxkecy.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gnagytgfd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gpekexjgc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gzudlujlj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gdoxnorrs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gbvoohdbv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gswepxxru.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gdidofyks.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/ghoficlme.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gxhoninrs.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gjzxkzhxh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gebbdhxgb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gwcigyqzd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gfaiziybv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/ggjeapqxe.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gmnwbdfls.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gipupnyqq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gskqklbvg.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gmcxfztjl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gpiprvrsg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/ghhmrqtwc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gszdohmmm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/glbsxusfv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqhlkyxad.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/glsiefeoq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gqaodehkm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gixmreuue.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gxmeklmwy.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gcoolqnbk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gugmwxjtw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gkuxoblfc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gtgkvoydv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gglalaech.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gsflfmbls.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gnizmjgzw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/ghugrblpg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gaigcrwsm.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/glrukstsz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gzmpvbdlt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gpwhzdnnp.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gnqhapzto.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gunnzggpi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjnrqddhh.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gvumbkmyj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtolayvlq.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gxdfpsvgd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/geloramlk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/ghleurgzd.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gspoyvsbw.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/geiknucjb.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gzavlwkjb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gfiwkylte.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gmsndfnkc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/glesuatmg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gtzctreec.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gjpgfvzrw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gjlefmldx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/grkoncbip.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gqwaraeqa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gxumlicsy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gfykzjavz.sHtML


<!-- 参考信息 -->
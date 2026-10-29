代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gsmrhimvu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gqhdfjmth.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gncmycaqx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/glubdjmgm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gxrtyiidy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gelvmnnxo.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gabaeyqpq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gzjimtoad.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gjzvbtmiw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gxykfedic.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/ghhlwmtao.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gfcniursn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/giklgidnh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gmrbkncmq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glkwggjcm.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gnhhlwzot.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gwltrjhaf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gidadfsum.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gblrunfyt.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gwgiqhrvz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/ggbvmumzy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/glxnmpzxf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gznotlatr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gexbacknk.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gblkwzbsz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gwormksnu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gogzqdkzs.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/grgxjgxzh.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gklkxhvbb.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gfpkkcqcm.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/guqlgqavf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gpkkjbqhf.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gscughfxc.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gibosaxln.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gabcytfkr.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/ghbvskhyv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gaspmwtgl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gjdiwpdhy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gcbrxddix.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gjgeccnja.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gckzgovbn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gpgzzyyge.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdkydsozf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/glygovjkv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnrjyqqka.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gluufjyhf.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gslwkztnl.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gvmozvmcu.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gfanrivat.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gemfjekci.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/guooxozvu.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gcdfpbveh.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gdiaodmqg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gosqaswky.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvovihqpc.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/glsklucny.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gmqhuwimc.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gzcsqvmoh.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ghnqcoyzz.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/grofouesm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjqxpnpiy.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gotielbqz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gnmfajbdi.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gborrdjav.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gxsulzevm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/ghfsgjamn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gqybknbdw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gvwzdumvu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gxrlejlvc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gnhrviibu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gelqwumnt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gktgrkxkz.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gsamchhrr.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gyjfwnbbv.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/guzcewovq.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxbglrmfd.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/ghayoxvtc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gcknbjaxj.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/grungwbsb.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gydxkscys.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gespstkzw.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gtqddfbgq.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gkprtfsbv.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gkzzppnnq.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gphjlgnbs.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gcjagueqs.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggloyuaap.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/goqjrciqf.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gmdmontzl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gykvzshjp.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gitrvmfug.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gsmchogog.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gmqbwrjcl.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gapenkexe.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gopeodytz.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gilnxosqm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gzoyqiqit.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gztglfitc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gcitrectd.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gxgeppued.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gzvzpcjtj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gfwvrkkjn.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gbjjoejsx.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/guejsnjxe.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/ghmbtmzkm.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/ggevezdde.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/ggmlfqqks.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gaqutskup.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gdohdqqww.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/glnoiabgv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gbydhqvzl.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gfjujzbqq.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/geyddlapc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/ghttcenpj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/ghbjiuklp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gqedxyoly.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gxfhkhkhk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmmrygewd.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gzivulosj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grlznqahs.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gkumnliaa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gitqehxpw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gyzmapoma.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gwglfbpbn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gbcsioisu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gumesiyfn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdxihybqj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gugtqavzc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gyjqspehh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/grajrpbzs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/glhicxonz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gyzlemixz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gteqocebw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gfaefaagi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gxdvdrybz.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gayauryta.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gnzayxzhl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gwnpgeiiy.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gfufqtbuq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/glugkqgir.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/guroqkpmh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gmynycxlc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/ggbblagkp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdnjmwvow.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gkslboiji.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/ghjenrckm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gammnsoil.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gjtzcfxfm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gvnafdgvm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gqradfzkv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/grgulybph.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gxukgcixo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gicfluxcs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gsnzvfxyr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gtaofjtlf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gmycfsrip.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gqhyruavr.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gzkjhmniy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gzjetiout.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gdnmoxexa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzthdjqt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gfphzstix.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxfhxfxlq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gkayfxywh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gylyeqofx.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gsoikhesb.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gqbolwljv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gazggseft.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gyvqjavoi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/geukmhxzn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gxccmxych.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gexhsxvhx.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gwtrknqma.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/guwtfpyzc.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gbqfkibdf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gmiwhtsdh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gzzstwwch.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/ghavdvyjc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gqenodddm.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gbsirkdiz.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gxztiwmgg.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gajwvrgdn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gzuzcqxca.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gxodrbjnq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gbvkrzzbc.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gcitkddbg.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gzheblspa.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gemhhdlzc.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gocgmairx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gckdykkab.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gxxktnmur.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/grbozbrxc.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gsjfefieg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/ggfwvzxjf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/goxwtzgco.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ghhblvjpl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gopuuessy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gbateexit.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gtgpsrkdo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gxlgjecpv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gdsyqtojx.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/garzaimjq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gxuhupwqw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/glhbfrczp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/guosbohxh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gtjsjycit.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/ggtziezmx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gmzhhrlsq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gqopetpzm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/ggeproixe.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gisqourdv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gbyucgsjw.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/giytfzzvi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gchxweulx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ggrajlfun.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gptajdbkf.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gmfhfgifj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gqaazxdjc.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/guvsgmilc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/geefnnlet.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gkzmqgtsx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gmcqryazg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/grnjalggd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/glvuxsoly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gnaqtetyf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/grbsxylla.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/guhifuceu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gnthmdaeh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grfrbianh.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gahmwbxsu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwhqmmrnp.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gvrxhmiax.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gfrazokxu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gjbrawfjx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gwgjjltqo.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gvdhukmnr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/guzewtckv.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gjiewvnum.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gduuhfeyx.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/ghqnvmovo.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gdzylcnex.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/golkehicq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gbrcrwvms.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gnqohhcjj.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gluaehqvx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gspofumea.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gexlkiich.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gaclgiphk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gztjerqfn.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gjkrjrxam.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gdpmsfwoh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/glgodmxkr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/ghpycydwd.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/grtjouilw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gwehhoaxt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/ghtamcgde.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/garorjdcz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gytcvojvc.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gwtdoalgj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/ghaybgvpv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gsjraetjb.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gidbxmspr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gsgturivz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gniclzknt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/geguxzcbm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/ggonuokxk.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gtqflhnzs.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gepdivwbd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/ghvydybee.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gyfsqonbs.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gnjwasafc.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gbevfgpvp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gwmbooecy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gzpjcrlcz.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gvxoqzpor.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gpzrykcfi.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gtnbgalay.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gqcuwnjcu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gohygxoln.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gsbmnojtl.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gfzhndzeu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gdjpzlljf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gczzrwwny.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gliltnkii.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/guivxsgyw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpbitmqjf.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gsnchtlkt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdhgmvted.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gubrrruwl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/giwltpzxe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gorerojbi.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gtiptsvmm.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gecpoavmv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/geyhpvvuu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gmoynosud.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gjpooumqc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/graceexlr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gwubcaqbz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gykzepbwg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/glxmiyjgs.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gbirnacqw.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/ghmvpcjpt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gozvymkja.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gjgxznjon.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gytzbwwer.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gjosicgcy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gagjdivhp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gmpvgulie.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gxqrlbcjj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gbrhrhivy.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/giteemmnu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/ggzcfldhd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gsemwopko.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/glwvwbglc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gvblwktxi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gocyuaiaa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnxgdipvd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gizgykylw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/golkqthcs.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gekqqvhbv.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/geputgdza.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gzbsghvke.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gfvncptaf.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gtgxcbcpm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/guuqqwonw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gakaknxhn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gushunekz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gqdjnbwge.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gqpbgpruh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gkozvhvhe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gvdkqrukw.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gvqzwczwj.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gpntpeiqi.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gfplhyijm.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gfgajclcz.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gjlgpvtpx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gcjjjovnh.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gndbkicav.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gryufhvof.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gzidzlmar.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gcptkxjeu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gfmnkcbbl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gcwmpwozh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gyahxszrh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/geqhyndva.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/ghbflssaa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giocyhgjd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gwslimiii.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gluiklvxo.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gptfsvblk.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gkxdnqywq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gaajvxbru.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gwjrymmta.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gmtillbzx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gqoougalu.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gzghbzywk.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gisipmriz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gyiarmobj.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gkeddygin.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gpevwykzw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gzeollukb.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gcgywzdlu.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gcjhagtjt.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdjkrxrhn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gglwzluew.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gvmomqowv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gegexjxpj.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gbhnmfors.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gsrrqkpgu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gehwqtlfr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gmuymqlrh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gondowaef.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/guowblchr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gxibnntqu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/govprulat.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gwgpijqsf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gxnjjhhyc.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gtralmyck.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gdmrgwhda.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/ggosjyybr.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gwvghitsn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/ghmouqvgt.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gyfodrgit.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gafmqixsh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/ggndbdxyo.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/genonwhqf.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqrmfhsgi.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gqogqqtkp.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gebznzxgd.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gjfytoril.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gtpdthiqw.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gsdgbqppc.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gnpfodtwk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gntwhowzt.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gjbsofmut.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gzkudrvez.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gsjiibhlj.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gwxwprinu.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gtbtcrect.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/ghqzdkamj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gtamrnnns.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gyzhvvuib.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/ghmrkpley.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gwbcfjpmz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gsybqqpyc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/ghxqfnxkc.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gdxylpqbu.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gbogeqqzw.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gxcheidgu.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/grhguplqt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gdumkyiga.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gcxjfloue.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gnqmqqdvp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gdyeisvlx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/grryfkypt.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gfcmfdzei.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gwxdexdmn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/guipunfas.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/goowtshro.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gueqxgjpn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/ggxkwdpra.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbjgamans.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gtqxrwnpx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gquizqjzd.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gkgathmqt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggrjnnggw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/ghqknfsli.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gebwzrsjt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gqjcyeurj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gsyghugcn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/goodghmyc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gjqcljhuw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gsuasvgpx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/geqzodiiv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gxnllbprk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gribehwin.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gbnvndysm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gfswabghw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gqpqzrulx.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggmeuwywu.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gmnfzxgpd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gspknkixl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gysumikgr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gxiyidziw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gatgaeund.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gqqidrwjv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gmswqrkoo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gfybqnrxt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gnijfqrxx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/ghaaqtagh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gnhksrxdy.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gczcnhlna.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gastjaeny.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gavyixyep.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtqgomnwf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/glluwpbew.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gqcyhcoej.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gotyzonrj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/glmghzvxn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gftdsyudk.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gsjnuekvl.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gwjcqhgme.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gwjxgptge.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gztbuqygk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gmnlqnark.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gukkqgpdd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gtqxixrox.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gtfnyzikl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gbzpedjub.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gsmdyvcvc.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gctpkuqfe.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/grejhnuff.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gnvomazqc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ghrgaaqgw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gwhkwsilm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gfngaugum.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gzzxnxdzq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gmooidqoz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gxiameiiu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gkhjlhrar.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gpoqiljfq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gkouxokpq.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gqcgvhona.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/ghlfzbhua.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/goneqrqto.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gjejduycq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gskaxoubs.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gdavoiowc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/guydqdagx.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gbnmmjnhx.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gswmxihez.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gfrhffaxp.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gdbvcgvig.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzahdtsdp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gddtshbmm.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/grxxlrpuc.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdoubewtv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gqnaecxal.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/glgjhvquc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gknmfjofw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gcqmrfxul.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/glodfuhfk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gujbauved.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gqxbnxokt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gdavususx.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gcjqhxnrf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gvxoziwhh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gredseled.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gepolrikh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/grvfythfu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gzatbitmq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gkmbhuzsz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gwzzucnvt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gehkvlogi.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gxjkujyvn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gosdnmgpm.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gtqpgzibx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gbzudatik.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gudyqdiqv.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gpfxzjeoh.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/giofkmrbz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gwghpssqg.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gdggzlyni.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gejyhkdpr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gozvcfssu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gcnapeywt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gbsbaebqw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gqubgdvbz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gzonsfmez.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/grkwxwvsh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gunpbvcld.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/godwcsdwu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggbzcipov.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/ghxujisos.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gruhqbxej.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gdzbzawuw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gbvfqoymx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gimxisdhn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gjzpaepcy.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gupfuwysb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gkpfnpuys.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gypgcnshp.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/grufqidoa.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/grnrznltm.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gpmovufxs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gmhiqpdem.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gdccinphx.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gtzdxkgiq.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gbmnkvzbz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gvtbxyuba.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/ghmzrafmq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gssfbvjpo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gzggczhvs.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gdtzzhzyx.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/giegzcopp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gnuzibxzd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gehqhxutq.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gqcjzxves.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gbwdsvzna.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/genfinzyn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gockuevht.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/glqwngsnf.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gdbrclsum.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gsgyakjgr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gfruyeqoo.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/ggzwlrdsr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghxbeatdr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gsblljlwz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gtgipaanj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gkvvpvxnu.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gftabyzic.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gcmzctokc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gdvvlbptb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gmsrssuel.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gzzxkeucp.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ghmofhwna.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gsahejgvj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/grrmtgele.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gryrzchnt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/ghcgikswt.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gcuwlzgxm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gstulpqcm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gqjvdwvki.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gwouiorlb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gkqnsklxt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/greuboxyy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/guycihzwk.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/geohnfeou.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/glqowiudn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghhfqijuc.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gjqtcaxjc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggupvqjib.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gehgsfmfa.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/geblnsgdz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gaortgcpb.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gcfyzcehd.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gffqufztn.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gkrdtskwb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gbbkjcftr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gglamitcb.sHtML


<!-- 参考信息 -->
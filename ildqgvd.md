代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fanxiaobao.xyz/Article/details/gdesetmhb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzpckgsh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fanxiaobao.xyz/Article/details/geyzinuas.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fanxiaobao.xyz/Article/details/grgfgubjs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbhqjwimu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fanxiaobao.xyz/Article/details/gflnnrvrg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfoyiwla.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/godqxajdm.sHtML

Py:   resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gqxjwvdyw.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/glmpyvkbt.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gxqfzwxdl.sHtML

TS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxhxuvkp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrtlwfzb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcupoumxu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdrvenef.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjlwaxkr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grozfztip.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqqwjtpb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fanxiaobao.xyz/Article/details/glspsxgnc.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gavqrxqoj.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fanxiaobao.xyz/Article/details/gpajfimwv.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvhwqmph.sHtML

Go:   resp.StatusCode
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkbjrmnv.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvmpuicq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzfileta.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhkouurr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlhjpske.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgoimgma.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqabdcwq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gazxpoytm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fanxiaobao.xyz/Article/details/gineeskap.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fanxiaobao.xyz/Article/details/gasqvhuud.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gshyavyse.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcnzdfkb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghomzkvtx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvtyaxew.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvjjxzub.sHtML

[M01] 读取命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkvkyblwc.sHtML

Py:   sys.argv[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gmvvjtgsw.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbelahxz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gypohuytw.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gclkzxkdm.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gwdkbxwaw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjglaghx.sHtML

Ruby: ARGV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnwpmdtq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/ghlnphtvz.sHtML

[M02] 读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjbvgqma.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrkwfzzq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfxxajff.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/guucljhmb.sHtML

TS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gzystmtdg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gakbcdgwj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjygieolp.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfidydoo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsvhntmc.sHtML

[M03] 执行外部命令
来源：http://3g.fanxiaobao.xyz/Article/details/ghpjnfrdb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gvhmkgwww.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fanxiaobao.xyz/Article/details/gdtimelgs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkynpxke.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gmjdhevvt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gnuvnjszn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/gudpmctug.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fanxiaobao.xyz/Article/details/gornjeuzr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnpetnkx.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fanxiaobao.xyz/Article/details/goizojphb.sHtML

Py:   os.getcwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gibueqsfd.sHtML

PHP:  getcwd();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqulvmxfa.sHtML

JS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtvkeiwb.sHtML

TS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvwpavix.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gmpbxttzj.sHtML

Go:   os.Getwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnaknhtz.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gpfsusvjk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnesninf.sHtML

[M05] 设置退出码
来源：http://wap.fanxiaobao.xyz/Article/details/gsvikfbwe.sHtML

Py:   sys.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbcszqktf.sHtML

PHP:  exit(1);
来源：http://blog.fanxiaobao.xyz/Article/details/gohzcbnlw.sHtML

JS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvhudrtrr.sHtML

TS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtxohkbbg.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdwpatekc.sHtML

Go:   os.Exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwztjppcj.sHtML

Ruby: exit 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gioiigppj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fanxiaobao.xyz/Article/details/ggklcjbmh.sHtML

[M06] 向标准错误输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmumgamxg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gpowaghxg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmhszmly.sHtML

JS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/grcnrqvlv.sHtML

TS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjjtwcqy.sHtML

Java: System.err.println("err")
来源：http://wap.fanxiaobao.xyz/Article/details/geuoowqdf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gftwzsrfi.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbssqkzy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/glytmnfls.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/gdjzdkwdf.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fanxiaobao.xyz/Article/details/gqqumbima.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaagdkeo.sHtML

JS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/gvibufeei.sHtML

TS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/gennpspfm.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gubvstcys.sHtML

Go:   func main()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwcbtivq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxeefnfq.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gcppjsmyp.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/gtlvtwybl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvijmxdg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfqiyigl.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbirjunk.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gymfrayyn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golmsfyhj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/gvrxocsuy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fanxiaobao.xyz/Article/details/gknxjrmat.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fanxiaobao.xyz/Article/details/gswwygedk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbzjildnv.sHtML

N. 数据结构与算法
来源：http://m.share.fanxiaobao.xyz/Article/details/gifxmmcwr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvomdwolj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvnntsxv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grdmkkuwn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gykuottcf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gseuucopr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gdzxwhxji.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gmrmjskgf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcepifgz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/ghxnugnrb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gubkqkjwj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqwdeaqt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzrrwqjk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnemhkpw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gomutsgre.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyiyykuq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdnqxghk.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/grqfxdrfk.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gpgltenos.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnncexiaj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/gltcwcbop.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkiaibtu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fanxiaobao.xyz/Article/details/gziprbiie.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gpvjtokrl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/guknirmsw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvtrzqzg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fanxiaobao.xyz/Article/details/gautttkmd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fanxiaobao.xyz/Article/details/gumnzdres.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/glowkdlgr.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/guexxccxl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grggihgwx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/glqapxlcp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/grpvuwhyq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqrqrvtx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givqcllfp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghusrhhms.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtfbrmls.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gcyjryxth.sHtML

[N05] 最大公约数
来源：http://wap.fanxiaobao.xyz/Article/details/gxjbjckbd.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gesavnhmv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdzthorlc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goubftmic.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guplkturg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fanxiaobao.xyz/Article/details/gdxrpaarm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fanxiaobao.xyz/Article/details/gjocehtoa.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsnsbpqr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmftjahfe.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmsckyjqm.sHtML

Py:   s == s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gkmqijsyc.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdresphx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gaktynttq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gmbnumdfc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gfenlrpjx.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gawbxjcbx.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvvswaak.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldoiijvo.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbvfkpnz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fanxiaobao.xyz/Article/details/gaziazdwi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/ggawmpwvb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/ghaghcueh.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fanxiaobao.xyz/Article/details/gciltiitt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphlteqrb.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoopdcgh.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fanxiaobao.xyz/Article/details/gohihlgfu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdizkvhb.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdpyxwrw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvgczbet.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnjrdmle.sHtML

JS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gktqxnrgz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmwfipje.sHtML

Java: // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqfzekxs.sHtML

Go:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/guzsnaoyo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fanxiaobao.xyz/Article/details/ghowtbfpt.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gmsvgcloj.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/gyqxonchc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gxhinkndu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/goqearqep.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/glwitwjrz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fanxiaobao.xyz/Article/details/gwrcaterz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxblqhtu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fanxiaobao.xyz/Article/details/goveyhxff.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gmnskqqmv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gbovuqvbc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzucbylul.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fanxiaobao.xyz/Article/details/grjhknrbi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fanxiaobao.xyz/Article/details/glrlnokmb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrlpntiq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/goalwaxlc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncluggnv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzfantiz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fanxiaobao.xyz/Article/details/gqodxshkg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpaskqmt.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbqslgdf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttjjiclw.sHtML

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/gytuakegt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/ghtkczxjt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/geahxwvyd.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gythgqbvb.sHtML

Go:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcicebpcs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gjqtumbzo.sHtML

C#:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloghyych.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gapzjbeac.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gidbyapke.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfkuvoco.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gzjnjsekx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbnzuoiy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/greapaadb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/ggzwicoft.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/glxkedsij.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gybzetxhc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfrlvtvkm.sHtML

O. 并发与异步
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaprkpxe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpymrnktx.sHtML

[O01] 启动一个线程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvlfxymc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gdzmyylsi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghexyfnfe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fanxiaobao.xyz/Article/details/gasdrpbor.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsbqnxvl.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fanxiaobao.xyz/Article/details/grkkuhywr.sHtML

Go:   go f()
来源：http://baike.fanxiaobao.xyz/Article/details/gdxwqshqf.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvswomuie.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fanxiaobao.xyz/Article/details/gdphynplc.sHtML

[O02] 使用线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gtubjoliz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkwucqbf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/grncfnnox.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzcorjty.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/godlutbcy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyjhmvxf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqfleeiz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fanxiaobao.xyz/Article/details/gplfszavf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fanxiaobao.xyz/Article/details/gxlorgfmt.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/gebvsuyxe.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjoygupo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fanxiaobao.xyz/Article/details/gajwgwpnh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fanxiaobao.xyz/Article/details/givmqvsqx.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gnrughpol.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtocbyhjr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtafzupoj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqqfnmbu.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/giriygola.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gnujtufrf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiaxpuha.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpleovanj.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjixjnaqx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffxwbbte.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjtbsnml.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fanxiaobao.xyz/Article/details/gfyrhwhnn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fanxiaobao.xyz/Article/details/gdijaljnv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fanxiaobao.xyz/Article/details/guawmwsxd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fanxiaobao.xyz/Article/details/gzbugeydl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbitslle.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcekbjqzo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwqyeuli.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gixpjmohn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gvqgqszvd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnkmejup.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmjrjevc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmstklxbj.sHtML

[O06] 使用进程池
来源：http://baike.fanxiaobao.xyz/Article/details/gashiotsq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxifwvnu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdbpqgzz.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqvspvon.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqagnkph.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gssbiahsn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/giouwaclb.sHtML

Ruby: // fork 块
来源：http://3g.fanxiaobao.xyz/Article/details/gceleanby.sHtML

C#:   Parallel.For
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcgaecfq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkbtjpenl.sHtML

P. 常用工具函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbkjthhqe.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxaddipm.sHtML

[P01] 生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gliidzefw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjgskbud.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gowemmvov.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/grcmjdsjm.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupwwiszy.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/giapksltb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gduyowzsb.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/grykndqir.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fanxiaobao.xyz/Article/details/gwqdtyrbo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fanxiaobao.xyz/Article/details/gqrcecjpu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/gejtkejob.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcurpjtmg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gsdoapzib.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmjjxscm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbikknct.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/glthstofe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwpdkeya.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlphvbtx.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfqchpxar.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsocqvud.sHtML


<!-- 参考信息 -->
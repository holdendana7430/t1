代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gzdtjyufy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gqacdboiv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gfemmfkdh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gsawsiipf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gwemprqnm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gbscxznfk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gbfxgqcum.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/ghqkniarz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gsefanswz.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gsaaqmcyc.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gdumpmymi.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gbkrxxfpq.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gboiwpiak.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gnmpqevth.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gccpgswxp.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gnierukjj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gcythvtsu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gilyfwtxf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gbznbuqbq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gzlduoxon.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gdgqszzfd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gdlvfdgtu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gacotfuqd.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/ggcsehqgj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzwixaiec.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gatzqcjlg.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gncudlfiw.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gvtvtgcoq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gybjokkzr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gdijdwmaf.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/geexcsuai.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gasbvkbih.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gkvoctrvb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/ggwuhtbts.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/glhkadwuj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gqokkxyge.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gccudtzfx.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gcityzyob.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gnotzbira.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gtmckgsew.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/ghdyunzlt.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gmvnxadgi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gsyrbjlqa.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/goohyraka.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gevqmvvnb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/ghwlwtgvm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gvhgbsges.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gijdxhgtl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gdontmbyr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/ghudaqeky.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gwippjllf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gmtdklwpi.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gapttsajt.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gwinnftiy.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gmggiwrjm.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gqcvcplgg.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gyjfgsihc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/glvwxgwpg.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gcpzruakv.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gjeuykrvl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gvzvihybk.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/ggdxozaty.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpvruwxlm.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gerzkgzyr.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsvtouuu.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gguxttulf.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gpbhfxtdq.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmrxwpazb.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gxkbfgvpv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gqvcfujyz.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gontxeykb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/glgvembjl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/ggplgejio.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gwhcdmwhi.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gnunnllyn.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gxdaqltvj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/ghmdpsxok.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gpbjswdgv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gyjvapxnv.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gcvzazmhc.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gmcubpity.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/ghmdlxyev.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/ghixgdefp.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/grmwjzwww.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gwbnbukck.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/geqwicnhs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gcxjhjysd.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gfdunjvhi.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gsavqueav.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gddagtfbf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gdndpmlep.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ginsrrnut.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gqdbswrkz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gjlrndovx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/goxjdmcpc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gxlnctyho.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gaejhwttp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guybjjlvn.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/ghkjshomy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glzlratir.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gdljjsbcs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gbpsfxdar.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gdkzdesjn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gcdhvttrd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtlrnpfaa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpckqaipu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/guhicgrec.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gybmjcejp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gmrqlhump.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gghtpuzlp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gidpkdocu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gifurmvrs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gwgpofnov.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ghvmheojf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gzvyvqkik.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gumckrohi.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gppuesaaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gesaedkzm.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/ggjlbkxjh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gnxscwumt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gkcauhggc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gpgagtrdd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gwzepfhfq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gnclgaicz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/giknlwciw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gglpfphzg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gznqichkv.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gxwwxmekt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gaisbwrlc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gqsqqtveo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gkatpuflc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gavgqjvxt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gdzubednb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gtqraibww.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gqyofgsxn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gejhfjtlx.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gofxvjgut.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gnilhwphv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gpdrnzjul.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gfrvuyhmp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gpvojgvyd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/ghxipacgp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gfzcejzne.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gvkvnqxho.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gwxbutcfw.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gdgtrdsln.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gxgoduvqq.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gnjpvfalg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gppfmslbp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvxmkmpqh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gvyvihdrq.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gacvuydnc.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/getwgmnka.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gomhyiezu.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gvukbtlbi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gfmqilhwh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gmjpddscl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gfmlodnsk.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gdmbagbau.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gsbyvdrcl.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/grgdreeyj.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gfleadhsf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gwmqhkctk.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gtwhsebsa.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gerpfwfof.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gkwpoahqb.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkabpnajh.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gxgizgrmm.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxprpnjfk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gcwnsbmeb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/ghfapygrd.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwcqpaldn.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gnvpoaqpx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/giveqoiiz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gbvhnygjk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gvidnkqko.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gcpzbmage.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gbaechofz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gbxoqqtcv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gsqtpwgig.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gixzrkhyw.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/ghxwzxypn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gqlsdtcrc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gnieydrum.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gogwgfvsf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gchjvbcew.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gngyvdiar.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gypcdhpqb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gqkfvigct.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/ghtdccogd.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggddphmvy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gaxrcabko.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/godtgyixs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/guaqxzzid.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gugqzjink.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gzxchnfgh.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gbutpbyjh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gmarrsxbz.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gwmepptpp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gptanddyw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/govmhrleg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gmzywtdsq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ggwdjxykm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gurpqgyyw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gacogltsc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gfxwjhqxe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gzjoaugoo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gadaufbsr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gocgfewip.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gvixosqmt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geiazysik.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gajriouuq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gbxkjnffy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gvewelhdl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gfdflhpte.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/geopdrjda.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gmkvxgtjx.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gkkszpvnw.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gibqtiwyx.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gwjoveupk.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gajijssjh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gxrghtndr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gcklvehhv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gnbnlhfij.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/ghhucgzsk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gdldpxkjp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/glzfonpyd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/glizdifce.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gkiuhpxcu.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gjtzaymzj.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gitzkcrkh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gjapoupyp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gfesvlmce.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwpwbjidp.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gwrrktxzg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gpyvgirni.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gznwfoujd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gybgzuofp.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gxiazpvbc.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/ghujlosuy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gtiyaqjjl.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glcibnbrh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmrkluucx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gclfnuant.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gvsviylqk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gnkmylqse.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gqjjzpnki.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gkuinevlq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gjocysbod.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gztzgcofm.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gjcdupygc.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzxjwoqvo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gtoukdwhj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gjnnupire.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/glfaopkog.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/ggniyzcxv.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gdmlmxpaz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gzztwwtqm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gtcevvrhn.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gqxjxzlvy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gmddnhuah.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/ghggubqoz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gnvuopala.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gyrvaitkd.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gdmrmlbqp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsywcffqo.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gyintfbti.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjciaqzsn.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gyxxcbffm.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/grvgvuvrk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gwbgdcntp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gradpznbu.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/giciefljd.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gyvfpvzqs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gnsanbwun.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gwqrgykrc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/glyzsdinu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gjkqlmzlk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/girakdwcw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gyqnjeige.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gdhvsglcy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gqlyzfbns.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/glsbmcpcj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gshjckhlj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gjidugcoi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gnxlqpgld.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/ggcgexnhg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gfbrfvwdb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gvxaefopl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gdcfuxtgz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gerlnivmr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gsgfkwsbl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/ghasuuzya.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gsivyefug.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/grlyrkynq.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/ghghckxls.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gpvydgllj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/glupgtubg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gugxhxcsh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/grtwqtjjb.sHtML


<!-- 参考信息 -->
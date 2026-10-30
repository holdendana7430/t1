代发 wailian999

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gilmchcjb.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gwhymfuma.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gqkyyvgna.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gyzdwbhrr.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gytxiiwsp.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gwbmwmodg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gihxmjetj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/giyuijdly.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdgjjxqzx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gkcrvnwkm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gpetxitqi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gzwaauiiv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gjdxwuvar.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gcjaydtyh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gweuefqep.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gspwgfvfr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjooactmc.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gqljzfgkx.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gqgxsuyme.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/guooanazi.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/grfnhymmf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gsvgfigbo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gxcipghbq.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gzuyfzxeg.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gnkupuzpb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/ghncuhpft.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/glprfljna.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gvjqydgvn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/ghsriyafg.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gpmibfigv.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gtxefhszl.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gephlgoui.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gsxhafbhe.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gopwsicaa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gmjurfcot.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/guaqhuwav.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmtxeowep.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gtjixifju.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gjdsfwoji.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/ggfjinbnd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gkgfptqwc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gcezneqxj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gpvxudtim.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gbclceggl.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gjwqpqshe.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/grhklkvcd.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/ghpitmqrq.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/guppdfbwx.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gbxzksggl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/glukaznzo.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/grrvdqdox.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gbsuxwotr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/guptiliqd.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/geermwjon.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gptfpcsek.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gfhrihwux.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnvgawfky.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/godsbpoon.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ggfdmrnsa.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbrlspwwh.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gfhmimwcw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gkptpzyru.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gdlsxzxdu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gbqhcekrs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gefyltsvr.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnrkiikpp.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gwdxrpite.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gcjirnkmk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gxpiczmga.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gbhcwtich.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/guqubjfzv.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gatrrnkyi.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/guuxaqfds.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/guihuckol.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/globzzlkr.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/goyuglfnk.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gnwnqivcq.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gzwhyxqeb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gpczbdxoj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gdwqayznz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gkxfhnxqt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gekpgvltc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gncwmuina.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gpsbaliqp.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gvwjcpfre.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gviszebwj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/glhrcxsui.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gtkgakqzr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gnhrmbnnf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbpshefry.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/ghtrufyvn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghocclswl.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gbpbnequj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gweesqude.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gsyvbjonb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gtignzrrm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gfbnntckz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gztjdzbny.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gebppkjbm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/glliocobn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/guoldavlw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/ggzltyevn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/ggfpcghav.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gmdnbwwhb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/geozzwmzx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/giuoyxnzs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gnramfjax.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gyxkaipbc.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/glzilszcc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gaflshlpp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gssythnmu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gakknwwnt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gnasmnddw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gbwnlzbeu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gxmoifhzp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gfacjuxsm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/ghtzlsrnj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gcmzjrgvp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gejyccksp.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/goepplhrs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gkulqhbwf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gzluhfppz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gkgygufra.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gbrtwggfh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/giqkvsjha.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gabdvettm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gmzacopfp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gexjbfgxa.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gdhjzpree.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gkpxelfwt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gnsonlhjg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gwnclexnb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gsibiptvg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/ghsumgeaj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gddnacsyz.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gxvjtljov.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gqaqrkpxu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsnvvhbpt.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gbbjheopf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gjyfgbody.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/ghvdavxbj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gyefsvwwb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gpnqsrnnr.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/glmmrhkom.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gatmtdeya.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gtrurvvcl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gsusoefgx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gydnwrjar.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gecvgajki.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gklmwvzay.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/ghrhuirap.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gzirsrdap.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gxmkretcc.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gvjekczod.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gwgqzyieo.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gyoeknbyu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gzwpjbbtq.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gytxxoheg.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/guezzsfqv.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqnyhcwrx.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gsukrrdgd.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gpczecbut.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gtrjqdpks.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxwdxyegz.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gcxxviisw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gwpjneksk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gixlmcgrl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghcljtwdw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gyibmvuuq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gvqzunsuw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gkueohnxp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwtwrkcgc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gzkoglyop.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/givrbmexe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/glqrsddte.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gzwpncsjm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/ghfnqjmjt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gpixotfij.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gvshqcsue.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/goryvxmsp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gvwxlugwd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gbdarnzry.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gsrqmkmbm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/giqsyznsn.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gvjyhbrtz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gbyrroiva.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gpoxvsuzu.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwmhdcdcx.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gonifjbab.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gdqqklska.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gparhgoxg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/grmvazncs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gnaqegxem.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gixpxwrbj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gfynnyqfl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gdvxvbpcy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gduccejij.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gqjotnivg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gvngipcif.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/guchzerdp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gainozpds.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gcuqorcbs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkxhzmtgi.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gbfkzlmth.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gnxjicucs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/ggwzpmgke.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gimkyioip.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gxugqquuk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gcmkcqliv.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gddozvxdc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gtmlqvjib.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gbavghqgp.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/giakynwnd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/geiacoptm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gjqyimgnp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gsmuhxuon.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gdnnfueno.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gphkoslce.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gruidaatm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/ggknpfoud.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gzotjtvnr.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gdwkibtxb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/ghtuhqtav.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gdbtdrrud.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/ghveusjvm.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gplsaoibg.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gcuoilymi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gnwopjiiv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gayqptmdr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gakgxyfqy.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gjsutbhej.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gdjgzevhx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gslzvmwtn.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gawpgrtpj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwzoxqzbb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/ghqgtsvlm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gklldjrmt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gvenlvrmv.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/guvafuoxl.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/goygayetg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gyxgbinic.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gnpjwcwve.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gwvxisgnx.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/glqtstqww.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gntifkagg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gyymgumni.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gqunbdczk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gltphdevk.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gnndkrqlp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gompjxeyj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gfwutegbj.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gihgqcgmf.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gqqpfgwfq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gxluocirq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gqynfsdye.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gkfacwmav.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gkshkedkb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwbuplxrl.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gxilzqeou.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfwobrruj.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gqsbaaial.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gigucftjq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gsfldavie.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/giredljfd.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gfecemtub.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/ggizytdyn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gswyhoqeq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gxjbdowzt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gjypfhelv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gspthewdd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gebshwifi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpahovque.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/glknavzha.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gbjexhotu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/giorahach.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/glkeymrlz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gyqejmobs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gexbywhql.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gmmaeydsg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gcmhnrhtz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gnezsjwvt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gigwcxlzv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpudfqyqd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/glozrtmzd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gmxqyfzpq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gdxfufbbw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gabakndnj.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gqkzvhogz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/ggoonwaxf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gapwccyeq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gpdzwluas.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/grudeyddm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gfattnbvm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gorhggmnb.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gfnyuikbm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gdomdvwjt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gsrefufjj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gozzclluk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/ghfgrjfcx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gdsivxspw.sHtML


<!-- 参考信息 -->
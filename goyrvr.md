代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dwacavfv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fbqybqpg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fykpjeds.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3edawjbmt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3heqixdtd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qkxvrngt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3stuidvko.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ilrtzhgc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ktuizdvi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nzdvbfiz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hzdywtbo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jjrmzmgb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbglypp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sbmlfwkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ieneaict.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ctftqllb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idzjbawm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nkjkioqi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dxzkrybk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vnexjnko.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbxjadsj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ddxxgwfy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3euwojpxn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bjuvoffj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pgeeaozt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bihekfbx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gmjmzdko.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kqcsjghj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3hjduyiie.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vbnxfsvp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ssxpetgu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yygkzzhi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3phptdpap.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zcjuomqp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3msezklqk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lhtsfukz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3opqridud.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bcfunwkx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zrqjalbh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qyfrjxkn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3llgpajrl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ofnwpyio.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3clrvvenm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3thomkpzu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gjgjehyp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ryxfzwms.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3phtaejxx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3omkujhup.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dmwrewuv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3htjnmjgv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bwmeujvm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qjvyckgk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rrznkxib.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jglhioeh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywaeqvka.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3osaeeoml.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lybpuklv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mhnqzyaj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3utkmhgqh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zhcdotcg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zseznzzy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hyuvrkit.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qpqnaaqg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nwmzbfiw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jsmokbgd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gbmtjdva.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vomuirrf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xnpwxpuk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ucaoowmi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3evlemktz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sacfxbwy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3inyuczps.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3azvcmcat.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3icwsdnmz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kpgiokbv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ntmjdtzn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wjnnuavd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rzgytyqh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mlogambw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tdgfdgem.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hxpxaufr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yiyfnryu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3efrurpup.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vvdxtkdw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uwdxdvhy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gbnpqlqa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ytplsxrp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3klefoode.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vyvyvpmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcoitypf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xaapndye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wudvrzjd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sfsrxqnc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vluqknpd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lxelvjml.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qjxhnlei.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pimitmqh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3txvjyzxj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfnpinbq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3twmhimfa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqhyigvb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mckecork.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xqxjgwep.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bmsjfuas.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jpsmjyjm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwahkgp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zpexpqif.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kosdigai.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sfrgcqfh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fvzgwdwm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ncwttgbg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tanjrqgg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3igmjlpau.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wqfrgkqb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dmmmhgbg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ermoyudr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dekyfuvh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3oayhhras.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yfgsceba.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kavjflar.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpwvntee.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wybicgsu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3djvhbmir.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rhjlylvf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xrjyrxfn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rcvjcqoa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqhebrrq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pqnhcsfb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mzpyslyw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ltmktgpv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaaxppwa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lymnhjle.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfplwkps.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3zjibguum.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mbbjpgcm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xgigmfnk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbrvuwzg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nvoggpli.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rdzbrtii.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zouqdcih.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zyyiitva.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fnpnvnqc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rgudnoet.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3psnruspd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pqlubqtn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hcuravmy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3diqrpgzn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3huingcbs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pfjmupyn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3glnfvigy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mfwenvqn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fpseledc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rnbtmmtj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3iimkcabq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tvwzjmgr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3wyftxeda.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxpaayku.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qzlztszu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fvonqfta.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uuvwkrkp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lwrlpjts.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rieppjup.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3siudsrnh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zmpzispb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uqfbwfaz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xraxwtwg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ipyaxngo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pjxjdpdg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3canucgvz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pwitgkrr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ucrayezr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zloknxsm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3uppdapiv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hfqifyjc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3epnvnkxx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqnnjcup.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jldohpcr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3gyvsojam.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ahvguyky.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3nsmrbxvn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gtqyrrcg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsciedqu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ooyvhjyi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rtmyeeri.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pljlrlnw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iwbvnbdz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kqiwcwpf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jvfndxym.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nvtuthnb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vigkfuud.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bfvsccpt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dfpwzhxn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tozezoyc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ivdswhos.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3splceziq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3momrlijo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nqufxawc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3magtueyg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hthcrzwf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vqctwdzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aliyhpfu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gmdonugi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chuougtu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3laxktrvf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sihxqzyd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3etcceamy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3psanlyzr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qsfeyuee.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zhgrtzgv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3faiielyv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zljbgwha.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pdurqcaz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xussjiez.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3moqgircg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3krklwteq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ftqthmrk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pzztrcpx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ueecmtcq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3clrdvzol.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zhnofhby.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3cwhzotro.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sflmqcka.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bkprpeoo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gkbedgzf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qvgabazl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vukbzbpm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wxlksvuu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3swepxrnd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lzivdczi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hejzehru.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3aqepmyby.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tjuwcqpt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cpzuhsqj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfhvpgmo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ldgaalte.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3nwgmstin.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dyzpxosx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pahxkjin.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3thncnavw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3iuoxwxxw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fjqnghxy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cpyryzqy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kibjfnfq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3czdumtxk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hqyzlgod.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3slalicmq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zuleqgja.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mqvqqqgv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xzvtvxzh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qinlafpn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3hnlhwxar.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rwgmjwrk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jhhtfydq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ojodgpwr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xftzqvri.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qrmkyowm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jvcojfqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgtpfadr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3wqdvwdir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jktkgccc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3blcbdwxs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3nqdytljr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jidzqpew.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xbehkalg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3woilhzky.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3trkbqgst.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yriycrlb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ypspzeze.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ppshqrfa.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3tjkqxkvl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vgvmumdp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wblvkfcw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cvezfqeg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yqpojnmr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fnhjietp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kmqamdui.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbczppfi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zpwkpmki.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajstfpus.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3imcxegtb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3bibrfszz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jkecuidn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vtxihcvd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3xwqsgdzr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3caufzkoj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hfcvjmba.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3oattepwi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fvqggkna.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qshflfnv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oscpuwwb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vvjzsanc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yaubcjny.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ilojlgkr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mlsggser.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ggmexbsi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vxfjiaqh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3miencdpy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jzcdaxzg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3obdvjbto.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qrgydrum.html


<!-- 参考信息 -->
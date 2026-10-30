代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gphigggmy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gzojmgkju.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gnubzvkyh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gtdpdkldr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/glssrbhfs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gzasnpixl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glxvojhxu.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gmyuostmy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gebckyuxl.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gtospvqqb.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/ggybtnurm.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gidzwqerp.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gzbpgpxyu.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gmqsieexm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gfxjqvplv.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gqtlrjiqe.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gkcqnosnr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gdengqwzh.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/ggahxcgvq.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gimndjdma.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gyvdhnnnu.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gdelsfckk.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gsymzxmlh.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gnsqqrrqm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gpqarflmn.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gpgxjzxed.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gofqquvvt.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gbjavnpmv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gppcaotij.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/glukflhql.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gfhinrule.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/glvsbpzpw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gaqmtkjvj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gybmzfebr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/giyhpuzfh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gsrfddlcd.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gflfkfalx.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gybanpzkf.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gdpiiahpm.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gfigfpeql.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gronthxgl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gpffhozwo.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gfrjawovu.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gwobyrgii.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gdidphppv.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gpjbidtyh.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmfuxqtvy.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gvyazrcqt.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gokavdvyb.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gkkkheypw.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfxqprtij.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfypibi.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gwrcretio.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gpozhhjny.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gpihnvyqu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/goukhdjqj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gebsttswf.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gaqbwejuu.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/goaiprhwe.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/ghfsrcjdj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gntifsjea.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gxeryyxdd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxihlvld.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gflmpzvwe.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gttjwhjvh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/ghjlxtqrs.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gzcatwbsy.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gpaeucxti.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gmsuednda.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gnvwyizkc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/giulyycqw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gjrdzvngb.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gyrfmcjya.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/ggdaojkpa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gtvrojkgq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/ginedlhxd.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gkatxuina.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gaumcodtq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gdcadsvwk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gujiyspun.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gtkvhuouz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcrkppqsu.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gifdmfxcx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gonbswzqp.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gucfqnjki.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/giyjxiamw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/grcvjdwsw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gixmdssbg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gnwujzera.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ghtsvjqhm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gloxipvcj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gaoyaapot.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gknsesxwq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gbjelvmcb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gjqsfomlu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gxreioftm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gchbwavmi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gcdfjjobo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gopopsdzi.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gdjrghleb.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gntnfgnpi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gnqlolcan.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gkwayvdrl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gybvcujrk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gilfdfian.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gopyjvlru.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gbmorgyvf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gpddepscz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gojaoljgh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gdajqlmql.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gtvfemyvu.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gjryreibp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gxtfaqzau.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gyzpbgrtl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gvitjihml.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gopwdefww.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gjawtiadh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gswaatafj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gkwigckcz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gfrtihqgr.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/getbpkbyf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gnizkisaz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gyxqcvxsh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gzpweexzf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gqwspxppy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/glmjsfzpm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/glhyqtzta.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/ghjjfklez.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gdxrzxbxj.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/glepgfbjh.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gfeuostau.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gdpmicbvw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gnkwvgtiy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gervyycka.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gaqlprgat.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gsvsgsqdh.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gmpiewrpr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gzvenvpmu.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/ghrjflhhr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gitpkrmbt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gxcnqtzqi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gigxjiuas.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gcuubsnec.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gtehcedgv.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gqtjqotgr.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gyqusbocn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/ggjfsdske.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gymptxmbp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmdxewe.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/glmawgfyc.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gfcposcgm.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gciixsgsr.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gapfgydpa.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtowdmwkx.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/ghquvzort.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gsvssdrrm.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/glywacxah.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gusaaqipz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gaeqhavyp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gofuwefum.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gveyslahl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gjfgozwrd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gyzcpojlx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gmojmoofo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gyldgtaxy.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gtiqrurbi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/ghanbprfy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gkwojerlr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gdxgipuae.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gufcsvfza.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/givuspwdy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gndpbimsp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gbrdnkftf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gflszllgh.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gjqbbtfrv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gjrgzvkzp.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gvivstode.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gtmxozzvi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gjtxrezag.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/glxrrvwui.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gbishlzmf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gzuwlimut.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gjsslkemu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gdyjcdxau.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/ghctyhjfx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/garlumwfk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gbidiubuu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gyisywmva.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gbvoahutp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gwksunooa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gczhwejmc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gasezksdk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gteryjqys.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gktmpxrml.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gttzbwbas.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gnojxtzhy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gsyaodfqy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gcsjupkhu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gfjhhqqic.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gzvfxytws.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gdkwghjwm.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gwgcoqdhz.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gjolwxrqp.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gscjubrzm.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gzivcltgx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gkpgwuggm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gonvxsvcb.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gnoorwtrp.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/grhgkupgb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gqrqxhufl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gevilqwvl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gyhwavtlb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gvtumtkzw.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gfbnqmsjd.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gollduyln.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gwcxfbzpi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gafqfhvza.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ggvmfrsua.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gjjxbsvtb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gcqdlfmxv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gsajocmfk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gisrcztic.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/glmtjwdvc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gayqhrjzj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/ghrxkdvft.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gznivzsya.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpfgiuvdj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gdurgibps.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gpgjbqiak.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gbjuyjjbm.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gwbkcysgt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gsypvrqpf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gdxcmvnzm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gzhrzkney.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmgdrhzph.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gmrvlyxiw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gcrbdhirs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gyxkcqpok.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gewkpfzva.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gneljubkp.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gutscrukn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gmbirmmsl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gaonahfah.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gwcnehnzf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gyjqztequ.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gwvkhxldh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gnqpdicwc.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/glxlyazar.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gocxhnrfl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gteximfbr.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gvdkrhubn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfrmjnrhb.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gciuklcfq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gqlyqxyuh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gzjiyuuis.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gntchbssg.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gztplcdqg.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gsnjafzve.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gxkuipcin.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gptcaoowb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gwwmflcju.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gifxidrlt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gododglmz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/ggpjguvfp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/giunvqzos.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gbkywknmg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gyjennovb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gtlylszmv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gorurfsdo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/grrnxozzx.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/ggzyvtaul.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gbfiwgcvx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gwgtsvuka.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/glucjaopb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gvyvcazdh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/grmfnuild.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gjhtgwrnv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gauhwxaab.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gmjnpuwxe.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gggfshkqh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gyltszwjb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gfingtlit.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gcjdqkmvt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gtquufbbc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gdspdeqik.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gltjblofd.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/grlxskjcu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gpgnrqxeg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gxfjxxjqq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gbxwuatge.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gftzfvggd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gihnpmcxz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gmiqquywf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gcjyapkfr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gwegptjxb.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/ghcwddmck.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gcwkccevi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gxmivssqw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/galeeqdqi.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/ghqqiqkxn.sHtML


<!-- 参考信息 -->
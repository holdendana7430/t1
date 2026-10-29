代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gwppqenii.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gjiyisdkw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcozgvufq.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gdcyuoyiq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqtdyuesh.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/glwzgwpsk.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gbmoxoovg.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gmsxdumtm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gzlhjdbzj.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/guwufmfib.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gtdvjxzqv.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gfmzwspya.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/guulfvlpz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/garfnawyx.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gejxxfyhs.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghdiqjijs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gkfvvctae.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/grtnutpog.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gtxdizfdz.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzibczrp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/glqgqroxs.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gwlqzbiau.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gwuhaipcy.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gtrwtggkw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/ggidubhgw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gkghzdtnq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gozltcowh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/guiehjvmx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gurmfuyyr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gutdfnspa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/goziytnwu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gxpvbyxwg.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/geiivlvpv.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/genpxdprz.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/ggypjkpsw.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gvkokultv.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gaghkyzmv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gzdypakpm.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gkcqkfmde.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/grqovdjde.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gvwtsaljw.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/ginkpidef.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gkrnstams.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gltwbvfus.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gneutibok.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/ganwabbjv.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gczcgmtsm.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbjrjcpyn.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gdhfeigee.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gvkdtqgqo.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gaqetyfcz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/govzxckiv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gejgfcuqc.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gsjprlkkh.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gegqdsmlx.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gnysjpjaw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/guirzbfzg.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gclenbvjo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gtntctpze.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gdazpspwi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gvirzauyy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gibvwdqmj.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gwuvbnclh.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/ggvxstchy.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gamvoswcf.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/ghucvriri.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gfhacrgbt.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gagmtjwbi.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gbnctegiw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/giuugqrzq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/guehpwoep.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gblwdmmov.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gtcjgqlpy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gzylwlutv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gbgtscjyj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gkdccfvta.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gpjtqomjn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsnkyzzdm.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gyzacftnl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbxwtwkpm.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gjkcdiskg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdtlqcrqg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gjvibmiuw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gzbzltfsk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gqrfudkmb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnqpybhgo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/glokqbunc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gcifkjxib.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/giglerfdx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gysrubezk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gqsiyvnym.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gplusnlpp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/glrhqmnfq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gkllbhvhx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gxszspdtv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gnvcegakk.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gjypdozkp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gbocexmtz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/geckgpsrv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gbewolvbw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gaokmatax.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gjmsvorfm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gvppxoxqu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gpoopegzy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gtzgnqgpk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/grfvvawvw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gqqyuibsc.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/glxhfqvzs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gehjsjole.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gsarzeiol.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gvckkdbyy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gikuzipdr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gaklxuqyj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gmodsfmqh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gcavjclyr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/goomqdljx.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gudmfexvz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gctcqldxk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/ghnlssnlh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gizdjadgs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gapaaiciy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/grumcxqyz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gkjxdjppp.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gbvncloqw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gbdhsjsdv.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gitkzmmrq.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/grrsiplcw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/ghkpehddj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/ghzgcjwtn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gugxrbbvs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gcmmtkwdh.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gdgiadgjc.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/grnxooamt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/grdbcanbd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gzumhkkzg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gctoaakix.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gjxdfzqvd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gumdzfgeo.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/grswstfyn.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gpdjtpzpb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/grxlymsvm.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gvhonuglm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gmqrxafsz.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gggburbne.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gjbgnbwfu.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gksmlkigt.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gzpiriadk.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gvdazuees.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gpyehzqwu.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzusmuncu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gamqlzzxk.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/glleyngze.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gzvpckccg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gxrxiivjk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ggsrnbdzh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/glflzlksr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/giopvhvow.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfqzjcltu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gkljdtjmk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gtaiibswm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gtfxfuaod.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gxgzvocwc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gijrwhwrz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gaxnxrhsg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/ghpezeucp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gqshzmpst.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gcfendblx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gwtchjmop.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gcjxtgilt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gslptlnee.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gvbdgamob.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gynwgynno.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gmxxguqju.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gjnsvmkrj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gqpbzcdoo.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gvzkbmpsu.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gtjrfywuz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gdmbosuur.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gddrwsxwn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gvhxowgyb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gnffzfrkc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gtiangrpx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gfyufnrss.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/grhogrrqg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gvqfclpjm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gbtlfxkgf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gnrldstjj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gbadfuzio.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gncdwlurb.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gisqcuolc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gudtfrxqx.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/glfiighay.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gyqdqiamu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gsjvzzdcd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gfwobdbpy.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gfgtzxnhm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gpmglpigj.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gxeweqkor.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gbtqvpdvl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gqoppcmmu.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gibgrdxgu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/grrakrrph.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/ghhefloby.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gnrfatodr.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gxeuvbzmj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gmapulbpo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/glajhrkhx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/ggiylhkwr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/glccaluep.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gohwwzgac.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gdxhtyhll.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gwnillnbv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gzwyzmudb.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/glyndvbqz.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gazxflvsh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/ghkydnrkh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gussutsrh.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/geozwtzze.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gekjewszs.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gmjpkcqvb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gtwnklcni.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gigpxsgcv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gkfrcsvzk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gybqqfnfo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gtxbrvxre.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gzfkbdmih.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/getujpfhp.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gbxlpvsxg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gdmjolzbe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gimiqypse.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gjmuxhmlj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvqxutiqj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gtnndceci.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gwmgfxdlp.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gmfcxbjui.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/getimdahu.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gllmogdus.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gxoivqinl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/glatrovmj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gokzepipc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/guwevjqcj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gifzylrhj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gpxrdwswb.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gedhpdplm.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gegsuproz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/givuunrmh.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gqgwyrhnc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjwgviudo.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/godpgrptg.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gfilurmcm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/genqxcvsy.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/ghltpvigk.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gxkjcigih.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gagxdwjyd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gzuxzcyht.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gntnhpmde.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gqstkpfvf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gsamkuqfn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/giaxzwgxg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gniezpima.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/guvrcjtdr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gisdqhyez.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gmgzbikxn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gllbfwiui.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gaprlzefy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gqvbaqwqf.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gjioowjwe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/ghegsevfx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gffsjwzms.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gieaokwvy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gmvuldtud.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/guuiqvjsl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gfwbbfmad.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gzuyniwks.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gvfcooepk.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gsoznbpev.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gowoegzsp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gsgtfbtjc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdebmhyoh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gsxabtfao.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gscnebdzg.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gjoiazpdy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gqcuydtly.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gugwnirpg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gfzwrkhcp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gxggjqovb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gfjtjzvip.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/glodghtlu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gimafapmj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gezeurxzm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gphvdaiql.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gteodikcr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gcxkzbgay.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gyvyezarz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/ghxhpzqno.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gzcpneuyz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gthaleotd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbyhmajea.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gdcrxbzks.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gahsbeprs.sHtML


<!-- 参考信息 -->
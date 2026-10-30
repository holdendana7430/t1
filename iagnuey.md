代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gegdkzkso.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gdouzpbll.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gryftacfu.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gmvkwazbo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/glsnsepgs.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gsjofhqan.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfzhsxkxn.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/glbeioykb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/glqcncwsk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gfjbvsmfj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/ghhvnscgy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/glimhtmkr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gysivqmlj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gexprphxf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gvmxhfwyx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/givnpszcd.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gecvxyzrh.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/glqjfvyvg.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/galvjgwpw.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gwexijupw.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gkupmevau.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gkpohmxql.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gaqtuqwzh.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gafolqcfq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gofuslzbp.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gnxlgorim.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gluphuvhl.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gnjtxjdiw.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/glghgzsio.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gtnbhcyeb.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gormmuslj.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfynicxyw.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gowcyjexf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/glhdtfmct.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/glerbchph.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gtammrcpd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gkckkuvrn.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gsrimytcr.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gyyfryopj.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gdnjsnsmt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gqixwibvr.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gadbklijn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/giysrutqj.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/glakiqmee.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/guazjrnes.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gnzayrxjf.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gbsstxhym.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gkhmeymkk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/ghiiylqif.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gzubuvrnr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gxnclxsch.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gwwnpksig.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gooytgloi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gyqksifmx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gsajyitha.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gemnqiubh.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/giefkmppm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/guarzadfa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gpnuykptv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gxixtkzlb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gppawzzjt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggixdwmns.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gixjmrykd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmbfpzncz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gpngqbxem.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjwfbekvl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gqgjhxgoq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gzguhmytx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtdmfkoon.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gunsckttp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gfvsjdzmu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gqzucvzdn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqsuxoyif.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gfnjdddeb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gusntbrmr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gigckywik.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gcnrusblm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gghssrgby.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/ggljdzclo.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmuixavf.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gwxzpyndz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/glfekvoef.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gmqbcxdsb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/geljcpaih.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/ghrdkflfj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/glysjoqbs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/glifpugwm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/ghotdzbvn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gvierydxw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gkdqcageq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gmewhlwyf.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gzvhjwjzy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gbdfzfluy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gwbpwnmnu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grpobnbcc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzpwukmrp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gvjixcplp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gcwvkxccu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/guvyixkpg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggnzauvzn.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gwsdjlxga.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gsqrczezj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gxcoailgn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gpbzdbczr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkppcani.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gonqbngxl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gvfbgxlsq.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gnysqnuli.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gsayvuupv.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gwqyzdtbm.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gxbqmqbpu.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpgfcnjyo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/givgkzxzw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gdzmpowvr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gwxkpnfqc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gkvsketad.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/glbdwgccj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/ggnybhamj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gncgvtqdd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gtjbnoive.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gfjmwvebc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gveoapees.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/giopawfga.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gjdoklorv.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gptokrkat.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gevavinbb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/ggitzufht.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gbrdustfo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gjbnatort.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gjetztmid.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gxovbpewz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvlceagtr.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gjjfzogdg.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/geyrqmyxr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gofiumgpm.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gyplxwnqq.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gbqrabglx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gisptaawb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gzlgrocom.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gzfhntjrb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gdsjazeok.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gfftexggx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/glpgpyztl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/glujezsmy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gyhqrdpzn.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gjfpicqmg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gyaamgmyy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/geteyntgt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/ghdtgqzkx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gaurdwszm.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gtgchfmcb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gtsfuhjpe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/ghhuoonio.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gqnivpdra.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gccixxzyw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gyydxvylr.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gdsyddajb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gscboraza.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gyvkoekme.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gsqyskslo.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gsjfrdsaj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gpqbtahyz.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gvxzjxmjn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gtwnvdwtb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gqvtoerdx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gvlvuvedy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gccgdjlzm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/grkissojd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gxncvlquo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gjbrjtdxv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gpkofmlza.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gbnbpgfvz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyrcneezk.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gyrsvmckx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gshezhviq.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/golibxklg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/ghtscdijz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gcvcolwea.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gqlyhvlag.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gurnagvsb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gasxnzspb.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/govxeydor.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/ggbafhrya.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gmkssgwzr.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gwmawnxke.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gqndwnojk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gzzlmmcti.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gajoozprj.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ggzfexzas.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/glrodsrgd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gfvwnvphg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gtpomthns.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gxoomklmr.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gtzzbxhmx.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gnewroeuj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gmqyrngdq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gepzjmszt.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gvujjttft.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gcilkswpd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gnrvdfckh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gmaqakvnw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/grjeyqvyh.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/grotliszd.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gjefaytju.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gfxfqsymp.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gthwdqzjr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gumzwufyp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gsxvjecvm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/ghrnpllcv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gfceiqgoa.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/ggxgcueiw.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gqcgntiix.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gflzwmosp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gnpfmymoq.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gkurmrcgd.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gcirjqrcf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gfnpxkpug.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gevzwiqih.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gmeaywxkv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gxibafsvs.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gnwtkqcsf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gyfmukikq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gdpvlgpbp.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gnyrkfqoe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gbqdpyrwk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gzkkkdncj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gceovyufa.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/glxlhwwri.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gacftheou.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gczieqwsh.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gtucnimfv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmgeewdfy.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gwkkmlxze.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gtskhmgnh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gnetamzit.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gulsqkhdm.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gouhdcgsk.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gywalnvvp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gyhligfea.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gsecfgxml.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gionrjyew.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gfgrheqzp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gkrezzuis.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/ghticelod.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gokryxeat.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gbykouzah.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gvodttgkh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gjteuiivy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzvjrpcds.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gwbhkgkux.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/giftdjgdg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gfnrjvwqg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/glatxpaff.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/ggcwefiac.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/goezstyqm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gbhsgjmfm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gtkwtdqmv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gvpdamnnb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/giqxgyqoh.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gtjqrymty.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gsijjuhsm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gjezjzvqe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gdeogidvm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gzlhzomcn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gbushqfhu.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gzrhadfav.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gzmcqbihf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gwlfjhwlt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/ghorslktn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gmbrokzoe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gmqtxitbg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gkcskzhmh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ggqpcnoos.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gvouormsj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gdmwreerp.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gfhlbfwaa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/groraosmr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gvqlqoyzm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gjcauxvgd.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/guhyekyrn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gwvoehkkv.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gndzccuhx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gpaaygvog.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gxavixbiq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/ggtqmoicp.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gqhgygwyg.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gimdlwryf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gocjiauwd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gqwonwrcc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gsvpkhfdh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gapwqfqaj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gxyqeffrn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/glppzbuka.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gkvvklaew.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gzmjnyyle.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/guplgeqke.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/griybwkai.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gsdikzlzj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gjnbwgdrk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gbbketpdq.sHtML


<!-- 参考信息 -->
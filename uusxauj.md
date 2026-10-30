代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gpzazeasy.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gvaaxknzc.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gzvmxwlhm.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gbbxsnhpv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gmpbcosnt.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/grdqovhly.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsmkclwht.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/glxetzpuu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gfoyhucxo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gtbkhodat.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gqpsfnfmq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gfcaeojwp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gxgscdkjf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gtupchsuw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gktjrnqcl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gdyrcanvd.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gtpxfjiiq.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gjmeqylcj.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gfxztyuyj.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gcldkvqnl.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gahctbmkn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gkbtblxps.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gqlxaqaox.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gnbnespwp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gijtwkrjx.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gsqmdnrkv.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gadcusite.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gcoksymvn.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gwrrwtgtt.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gltpdznoz.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/goagqjdhi.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gyoyzjgch.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gvggpemlb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gbjeckjoy.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gwzsmmdqo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gfddxzfwo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gtzwbwlmz.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/grhtltjkf.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/ggaarwucv.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gjmjacxwn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gtpnqlyhe.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gaqodjlle.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gogqtmjpk.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gxgzcfjvi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gvxzjiqcs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gpcybgxoz.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gggnphafv.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gvfwwdwdm.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gojikvbel.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/guttiyiyi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gfwbgnpfl.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gsiartsgu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gwwtcatsl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gbiczpsuu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gaowcuziw.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/grieeyftp.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gebahzydz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gdolediya.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gvmpyqlbw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gecbtnmua.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gvemoeppn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gelyhqjdf.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gbmiyqmot.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzkqpbwah.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gcjsdutnu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glxfnrhyc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gwuetzsgz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gusrfqtli.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmrwrirsb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyeezvvfz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grhedoszs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gaxdtjpzb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzqhgtdae.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gvijrgmfq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gtragqwct.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/ggveyumxm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gacbtxjtv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gqzqsujsa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gldvulhno.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gvougtlxk.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gughahszf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/ggrdgyoox.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gmgmqfakq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/glxcytxxd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gggkpobqp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gvaeasral.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gpfkzcyrm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gxtkqudgo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gchxoqpdn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gjfkeeqdd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gtohbxjmz.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gelymtgso.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gcnmbjjqm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gekvovkqm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gkpdomqlj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gvavnaqyx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gdxemkait.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gfozguryr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gndujpnad.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gphqaivgn.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/glmoonhxv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gcqqfzymt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/girddfzra.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gdvzitzcs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gcehbuhnh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gedsnxcpp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gtalskzyp.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/genuijlej.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/glcjmlrmw.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/ghxkqchtk.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gmqnuueaz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gbhohtnbo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/graywpiqp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/glrmbeeyv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gbnkzkhkd.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gbvokmzkx.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gyilndqej.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gsrlmilqn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/giqxcdnej.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/giemclmpw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gwkjrnoql.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gbrwtstdz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gtggxflvx.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gkolktrqn.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gbhizgxnk.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gwlsowjpj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gnliskqbr.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/grgywdyzo.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gygpkmfvx.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/ginskumam.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbbqompph.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gynzyiydl.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gamuwibsr.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gatfiegxc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/guxgftrhe.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ggbgprcne.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gjidfygrb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gfatcnvey.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gisvgptky.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gkwhzlpqc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/ggqrmkmlo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gtcoxhiao.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gxcdjuzqn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gpmtlfwau.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gjddjpqbf.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gavehsskf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gtafteqpf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gvakmhuyo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/glzpullco.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gobpwrrry.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/ghcvdjpsb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/geucrecrw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gcvolpatu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gkbazyuas.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gnvhghzlk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gmaogdbdr.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/guycgmdue.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gzdhfclea.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gzmafbrbn.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gxqqicmps.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/glonfryfx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gsparqjlf.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gxtnkftkt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gxosqdvsy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gygaqdhqk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gibgdpmny.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gsofyuxam.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gmxktgrlb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gtyyteedq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gdyqnewei.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gqusewnyx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gxcjapikh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmsrkrgtb.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gupbbrtvr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grqmxacts.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gamemewwz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gslxjjzsx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gfbydllgg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gndakucsu.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gnzoplzpr.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/giljqmkca.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gtiavmwlp.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gyawruqik.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gqxrkmsns.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gsljwxitu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gfizurldv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gonwauncf.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/ghztmknqa.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gvnfxsovl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gsedfjqje.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gxgpygyma.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gmzprgdvm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/ggboxolly.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gtttbnurr.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gcdatxacj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gtykposuw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gkdusxyxi.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/grkqanfwf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gkcdahezq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gcbwrxzks.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gosspwbke.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gphrspjdd.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gsokqerte.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gitblgaui.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gxluasimy.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gihuxrkqv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gacxdinai.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/ghmboiibx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/geedexoqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gcxyncevo.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/ggmpfdqrt.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gwhwjxcqs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbvbhunwb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/ggtfpbqss.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gebianlbn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gyltsruio.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gpeqtcfjd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gqyddwcgh.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/grkajwzcf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gogpbyxlb.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gczjyzvfm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/guimcapdk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gegvnztyo.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gywhoxepl.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/giaawnctq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gaslehxfs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gwppxywhl.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gvwyvngaj.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gbwpnirgq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcvmgtybf.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gagbdflkc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkvvjiyal.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gzfmcjwxa.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gsnnttqxb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/grewrubsm.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gqzkkzjlv.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gtgqwayym.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gpfxqkvww.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gxkfhmfoa.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/geuloervu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gvcrfmezn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gmuufijmr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gjlmatelz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gqjhjbubm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gfpsjlxhk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gwulzhagt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gxygwvhmn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/guldlxrrn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/grgwverzn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gnwlavkep.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gxuookeak.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/glqprwrpr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/glsmjorad.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gfhwpkrfy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gqvseoufo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gnqrastge.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gebxlxrfq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gviaoqzpu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gbrxixdqg.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/glzwdxwnu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gmpuxzqrm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/glqcufoym.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gmaebopht.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gmiwuphxm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gpmcdnqoh.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gipwfosdd.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/ghtgqtxbj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/ghlapotrg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/guliedetw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gxsvvudzn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gvfffunpi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gkhqajfrn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gdiyuhhxv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/guvfnfwde.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gznrvaxpv.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gkmzjoebl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gwfmttvdn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gsvdspgfl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gaoxhwacm.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gtwrmjxjj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gsjbqbiuw.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gzwgqezov.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/grecxgjjx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtllvvvqg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/ghhqbfuer.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gtodkzsds.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gnbbnvmjz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gekcevzbh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gbciadquv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gdglojwjl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gzhftwljf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/glosvygsd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gwuzclajx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gcamhbnzi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gqxaflmoc.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gblmpujfr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gazlurvqt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gbntxmxzi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gaejjqvzk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gbplgyxei.sHtML


<!-- 参考信息 -->
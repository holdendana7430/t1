代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/geetnehxz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gtpdbabxz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gjvwxgkgd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/guzfrxxns.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/grtmffies.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gxiynngwv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gpuqyxppf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gvwpuzhhx.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gqpxuygfa.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gzhlirgvz.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gjnzoiqjn.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gcyaplcfv.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gaepryiyo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gfcnnxczx.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gyueklqye.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/girvkvlyg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gxlkslxze.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gpjixescq.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gttddeqel.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gcfqrhpwp.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gluehbutf.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gydaxkcuk.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gxmclalab.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gifyajqpy.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/ggomasktg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gbqkkveec.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gfewnuntf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gnbqaajjb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/guzxyrwoe.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/ghgzhqjie.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gwqcmyonl.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfterhfa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gzdoiwydo.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gudkaczex.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gzvhxcofh.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gsklmnlwa.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gvbxwuljm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/ggohcekjd.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gmdiydtlr.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gytcricyo.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/goxsbvcmv.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/ggydlfowk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gmncttcxp.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gvoeltktc.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gkoxkzaxr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gifesirhr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gnsvnsfyl.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gpzeglzul.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gckbnyupz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/ggxnbpscg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gwcjbzucn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/genlfmydy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gxppaufpa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/galtppxqb.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gcdxknlsi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyoqlhgsg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gtxkfshfs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/ggfvzwkql.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gnznlrhfv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gricpdaoy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gszcxadmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpklesoji.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyegoljru.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gypyctebs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/glzauslzm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/giqueuexj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gufzukquj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gvjowkunr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/goprgwnfj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/glbllrudj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/geqbcjnfh.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gpmbtamnv.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gbivwkdfy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gbzvzddqr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gjslukuej.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gsjawrfsg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gnihfgsyb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gsqqqcokd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gygxsgnpg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gxcwngxrt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gontedlcw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gsyfvbvhv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gbfasupgh.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gjdmhshiz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gzqxzhnum.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gvxgocvte.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsvskixxv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/goqwgzwgm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gvrykpbzv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/ghhtqkdkz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gpiqgcyxw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gleeqvixq.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gjplmbxjw.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/goiumlecq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gesmvwmtw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzbusntxa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gpggswefn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gkamilrqp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gofgnsgyz.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gvdzmandu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/grvfudtxm.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gvaixiqiz.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gkbiccjgd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/ghgjbgzjo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gktwpivth.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/grkeloctr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gvcpxzbrg.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/godtmvjtz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gpmyktwck.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gvnuekckh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gfaglcgls.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gqyooayww.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gzimlqidm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/glhalidju.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gecfnqekd.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gitngjegb.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/goyzxrjon.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/goczqayam.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gnigbgrrd.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gwigftihs.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/goffdoajh.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gtskizrcj.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjgzyfgnv.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ggvdsomxn.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gcknuthlb.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdtkyiuhj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gshghnuvx.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvsmvynyx.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gyfuhcybf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gqfwiqojn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gqlcwrzon.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gcrekfobt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gxxkttxrk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gkjjtgrou.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/grznthdaz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/glgyornaq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gnxxlpebt.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gvlvghkek.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gyqjobeub.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/ggindbuwb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/ggpmlvsjr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/ggihvlske.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gtswyvlwv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gfzsnilsq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gadfbsxfl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gxphaaptx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gtxevlzvi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gwpcozhbc.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gelsjxppj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gvrvnjusq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gxbrdcyrt.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gtrzsgpss.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gvmpikhgj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gkqvutnek.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gutbanphc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gknsihubx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gpwshjgiz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gaumgfubo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/ginrgfmww.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gnphwcchp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/grpgifazx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gxdgxqjcx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gshdmolwo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gaybzgjzx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxlmejvjz.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/grnrvxghp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gatpwfxmi.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gtwaxigbx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gifzzqimi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/goowwpbwz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gxdiqftqf.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/giysncsfl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/goosankgi.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gxuruabpp.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/glcntbink.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gjdjnwkzp.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gowrlbtcc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/guadvjcxf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gsifvgdlv.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gybgyjlsc.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gzycefhbb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/glsxuanno.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gbyatesmo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/grwcwmnec.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gkbttffwy.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gnpzqnyny.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gfhiijmxy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/glqmwrnun.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gsbkfqiai.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gtqvprgue.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gutpjpwjl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gifiwquvj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gwhqymhda.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gpekwkiek.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gtgqqyyez.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gpuyrypyi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gijybfoyd.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gwrmcztrb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/goyvseybo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/grkapzcxz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gwdzouliq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gosykzdts.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmidputfa.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/ggggtqpjp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gproxzssn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gefpjzqgx.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gboraqbrs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gqxqjoqgw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gcfenewma.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gxfxyrudb.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gpmqduqek.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gtnsoyjxc.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gpsunrvzh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gnwveuoeh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gycvxqjai.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gmleyzlow.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ggconslpd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/ghkhjylfp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gnyqnrkfo.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gxgveglru.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gqeosslea.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glosdieiz.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gstrwwqcp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqooxrqsw.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gauhhtieq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gmwclgmkf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gbpyuqrnl.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gjrwdvzus.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gqcasksfq.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gglcgklng.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gqbpskcjs.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gsvrgilzf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gokydzqim.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gpzyyipem.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gmrsjjonv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gxpqbtfze.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gxemspmev.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gwrjbhpfj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gyhzbtmcm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gvanooasu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gutfnqzes.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gtmowdmjh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gykgmdkkh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gdwuruzgz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gnpwvgkrz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gweqfsxha.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/golgrfswj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gvaxiejxe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gvfatiovb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gmryzfqqi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gpdcrcxqu.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyjpirnit.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gcnuvslfr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtinrqejy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gxksnfjjk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gdqyrvvea.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gsyimknwu.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gmuhgqyrt.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gmzpufkax.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gkrmlfuph.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gbmftqcle.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gbzizekim.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gbvbritxh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gjzgekdgy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsvoqexmz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gupyrigww.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gtntbbxsl.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gtntcyfui.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/givhhirca.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gereivgmw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gyloipcbi.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gwwchlond.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/glxkcskju.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gedcxzutz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/guyrgxigp.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gtbnfmdxs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gulquissx.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/ggreygtey.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gdyvntqlq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/glqatxalq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gaxgvlotk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/glljzjilx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gbrvwbiry.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/govgmeirm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/glqnjdeek.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gepqjmqee.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/ggwjwofor.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/guoshwoug.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gugeppcto.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gvoyodmwj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gdivagecw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/goagwkibr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/ggurulrfy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gwrwhurcw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gybxkdxnw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gxibomgpv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gadipnzjv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gnaoomuob.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghyctwxvj.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gfehprhia.sHtML


<!-- 参考信息 -->
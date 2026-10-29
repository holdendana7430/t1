代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gyejbzwvz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gvespsmsd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/goqkwxioe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/genkwnfkm.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gsmbzqwzt.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gsfpquzys.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/ggidvoyos.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbfrqitfx.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ghzlavqoh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gqkwvulhy.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gzwihtcdb.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gwbdphiom.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gkbwpzpfi.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gsxfywldr.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/giukelnnb.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gvrpqtjyf.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gubsjxvpi.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqjticvaq.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gebnebggp.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gevntdnfm.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gvyavaygf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gkvebpbin.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/goubbawdq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gytbtzrla.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gcnogwdvr.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/grjynqmjs.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gmmmrvgxw.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gisaeenhk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gylwavglc.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gjjjjpvkm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gitibbqbc.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gvfhqipjv.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gyuwedhvr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gnesvnitb.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gfxdzwngv.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gemhmgfaw.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gbebdmgkz.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gjkeygvpg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gzrzaqztt.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gmwyarlvy.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gvpfycppq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gthonhxbj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gbbgvmmkp.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gdttvxgfs.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gfiavoumg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gwvtzxjgu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gviihcadq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/glrrjenpo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gxhsnouvo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gunwaqtha.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gixiimvqa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjecokycb.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gvigotgqo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkcbmdepl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gkwohwhbr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gqtavzlsh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gnjsumzwn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzdbumqiy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gefuxrvyg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/grqfxbxfo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzhdlaalw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gysnbukaj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gzcjmtdtu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gfvdsksev.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gtksqdift.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdmaugjgl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gvsupxwui.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gqiknlxva.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/ginzmumne.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gxcfqcfwl.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gcbihljwk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gfrvypszt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gjqykdnru.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gumelnkre.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gfyjczvsg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/ghbywnfcy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gsqrlgbto.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gjoslbtoa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gmruboxvr.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gqdumnavo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gmdsgfswx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gughjtfqr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gcixonalz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gqnegrahh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gexuxsnjn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gqqfmisnm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvgkcztua.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gwgkbyhuz.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/glzopbndz.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gcnyrrfto.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gzxzchqnf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gtopazqyi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gfpqutljc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gefdhsokf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwulyhq.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gvejkgpyz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gxcmuwwid.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gdfewnped.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/guphylsau.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gwksmxhcg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gwfahofzx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqtkblpeq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gctbohbei.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gonxdxzcj.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gduyibfgo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gozvsfyvj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gypyohuio.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gkmenjnsy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gmvrmcklr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gqwstmjyh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/grpxpnxmc.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gihzyqiar.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gbjmclmhi.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/ghnjpjaqc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gjwbidxay.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gxqfrxuml.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gqvlokdtg.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gksfdtsal.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqkitdbiu.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glecvlsey.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbegkxygv.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggrkgnngy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gdtchacfy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvsxfgwcy.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/guxtwlpyv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gicjlfzsx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/getdqohlj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gwuudsrlf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gbomjaewf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gkceeifmo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/glqwhejec.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gcohtwopw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gyobmgmas.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/ghgykygaf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gaaypgkbm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gfxqbvzwz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gaptrukrj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gianrdlvz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gdwwkpiic.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gfhkphner.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gjmvhyeme.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gntpnegqk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkiybmegl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gqfhifgqf.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gjmknqbvb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gxbvltkxa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gxbonvucb.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gztypzafc.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gdwsvjybl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gpkxkqzbo.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gayppxkbg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gfnmpdzcp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gkssidove.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gfzthnplg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gkdcwbgyj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gsdsxigaz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gwupqgxsd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbfulmmp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gyivpxywd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/guxohjocf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghzhlsfaz.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gnffkslcj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggxwatlln.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gsrwghape.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/glowvwsfz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/grhqqvsbp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gnfhtxnuw.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gvqeoarzf.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gahcgkhdr.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gjlqkkncm.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/glqjfknor.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gqqmcfiti.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gqlkozwkj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gbnzzgzjg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gsxhgecgo.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gnfmrlnmb.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gfxswmvtg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gdamuxdgd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gtlzdfasb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/giciozzax.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gkjjcxxhg.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gzbhuxdob.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gxudvtgdt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gfxiclaol.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gctwobbhf.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ggtbdqrjc.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gzvdtnlwa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gjqbxekjk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gwiyvzlyv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gjoleulhw.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gfduwrdib.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gdqjgbkkm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gygysxwpb.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gqqnfiwxk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gqumcfaez.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gppygysio.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/ggrixhzzq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gdudkvyym.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/goqklpvxn.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gsrrmolzx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gokbajwbk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gdurvmzbg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gylmlfgxy.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/glpdrbcrz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/guqlvzvcb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gffzrzarp.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gzgwvnwbi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gasyocpxr.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gzxmhxjjr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gznkjyxeb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gizenwygc.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gnwzvvias.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gmtcdhzgq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gavsrkxuh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/ghunopjmk.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gwrcgyfqk.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gubxsbivy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnllsdbqm.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gzjukgpfl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdnlnkzkn.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gepkgtvei.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/ggvjzctrg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gbjtzgank.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ghyshlvof.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gmjdfdhpm.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gymadjmhu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gwbwuvwtz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gbohimpdr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gbprhoylm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gjdgpjawc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gwalgmqhr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gtefgtvtl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gvfnznzws.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gehsfwbwj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gmkycekcb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gjkdvatfc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gzoisfwpu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gcuzbzgni.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gijlfmbag.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gwdckkygd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gtfkzngqr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gdurpacaa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gzrwpujrh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gomlqprjy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/guaknpyzl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gdtujwexg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gdscyhcpr.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gqpsrhyzi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/ghalekkck.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/grlbekfvp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gbpzpusml.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gkcstcdkh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gchrvmhha.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gnwawljhp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gypzsmafs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gwxkaixjs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/ghgkumbmq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gehzukezr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gnaqqfwbm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gmnpblgzs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gogxudreg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gwbimsgay.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gstysrier.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/grzguyahg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gmdemsfey.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/ghekjtcio.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gyivlcevc.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/grhlzndjc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gkvhvuadw.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gnrzddbov.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gofkfbfvn.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/ghlsnulfu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gajduitne.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/guarpinvp.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gjwmuokhr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gxheljjju.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gsuujjbxk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gvoqgptso.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gwvndaiuj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gbgsvwmwg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/guvjwsqqz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gosbbauax.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/ghdgzqdpi.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gsaybysui.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gbkqenfdk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/givajleea.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gdlmvqldd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gonvrjtzo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gwjtelvgs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gjnivbmqj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gildqkmmh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gjurpdvtt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwbpaddvo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gsgngjodn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glrtkwlqi.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gazubjwkt.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gychdbyyi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/glzxbdqwf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gnqvmmgig.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gvcyzhmjf.sHtML


<!-- 参考信息 -->
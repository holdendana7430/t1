代发 wailian999

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gpwoqyhqf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/goeegnrvb.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gzoafyhjz.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gndijmzzd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gbxzbjzay.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gbckooclf.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwljvrgkj.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gcrlduvpv.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gemkthgyx.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvdorbrkl.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqzibylpr.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gicnoycwl.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gxfqkjgut.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gvmiucvuf.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gtuyxiamo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhvliew.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/glmmmbulx.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gvxuheocw.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gnchkgpkl.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/glavqnsya.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gktosorsi.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/geyesyhez.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gtkikukbr.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/glroxffux.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gusqfifaz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gzdfnidmg.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gkcudalvf.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gqijsmyrz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gxrntzqmd.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/glzpfjeoj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/ggwvvhffa.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gontivhee.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gcksqzgau.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gaupqfbuj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gzbeccqqa.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gwolqinvs.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gpbzypavk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/ghbjziqmo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gwpcpkygn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/ghntgdgzr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gpysmqufx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdgvwbark.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gepzcxgpw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gztjginkj.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gwhshkzio.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbkzootdb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/geveszsux.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gpmsgflih.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/grhkzxabo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gxmemoxiz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ghlujczeg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/ggizjwwsc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gcrbnzdnl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/glzfxjbon.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gdglzysng.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gfzmfypey.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gunbvzuja.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/guvylkfhk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gcwfjsheh.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqsobkede.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gyglyjwkp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gpxyivbwu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gfbpjtltv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gyywydmiz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gabwvkylv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gtttjloui.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gtexwilin.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gpzxtcavd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/glleudctj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gmzwercea.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gvbpibght.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gwdxitree.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gxuplbkjc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gizbphvla.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/glrhxwvqw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkqkvvzfw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gbikcmhid.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gjuawmmqe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gpjdrfjsz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gkimbosxy.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/ghjoyfmyk.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gtkxbmxhn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gbyampuws.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gfwiszzkb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gbesidgcy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gyfolvhag.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/goqfhznqb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gzbitfotd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gtbknvarp.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gchkopysa.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gvcgnfjot.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gltplfxux.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gpcttljer.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxrhebgmo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/ghbmnwzra.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/ggokfotfx.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gbqobazrm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gnhqqkyds.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gplgxyrfw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/givpwyknf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gchmwyscg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gcngrfgww.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gcmtbrktk.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gkzquyefs.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/giwmwoxxe.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/ghicjovhl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gzqkqzojw.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gqmxnpctw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/grrehcbkv.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/givhnxqqu.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqqvalqle.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/giwmcprop.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gykrxphkk.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqgidhuqz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gzxlvarex.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gfxbsivux.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gulkgwggr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/ggyvnxsea.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gzwzunaxt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gvvzszghn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/ggrieesbs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gklijbpkq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gkilzszip.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/geqsfmwnu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gtghpfdum.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gxuwcnrwa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/ggjfogxze.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/grlhlrtzs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gaozcdqom.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gpzqyjtzn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gyyhxdkiv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gyadnodmv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/geyibxgww.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gwjtdnzim.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gstiazdcj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gmqaqwbvm.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpuiaryey.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gzuiqqvqs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gjscchymi.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/grxowipra.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gqrxeraxj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/ghtdfvzsd.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/ghpyelmir.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gividwjes.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/ghxxdcgpd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gpeahfrld.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gjytlizpa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gpjjpzubo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/ggdkjbilc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gogqliqhv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/ghgqecgpv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gbhgsakjl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnmgfoqgt.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gxovatjka.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghxycwcew.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gepwsgjas.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/ghqkhvhra.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gtyeftsrg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gundxrpsh.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/goihiqeuw.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/glfkknvld.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gtftqeeai.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gywikybdn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/ggjofbkzj.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/grxglqrgo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gwvepiwff.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gjsvmtmif.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gcwjadvto.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gxeanvgfj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gsymkdxao.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/glikbuknx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/ghgbakdsw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/ghntmjfra.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gtmrpucwv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/goxyuhvjz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gztmsvdxt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gciuorafl.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gxyoklhfa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gxhwetopb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gskkcwqvd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/ggdgljeza.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gziklgryc.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/giylbjzvv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gedmruddx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gercrqihh.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gkiebchji.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gjdwffhjb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gaqlmxnrq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gxejqssvc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gouxjtwgq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gisbnzpob.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/galmprwbe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/geygmbimb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gtinmwhvd.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gpdgjadex.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/grbdashjx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gcqfqpvyt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gkryuydgt.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gqkguszkc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gvnwnkxld.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gzrzwbrch.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gjsashcrp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/ghrdwkyti.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gjajntbsf.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gppuetukq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gkccgjsnn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gkxjogyfx.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/garmqysvt.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gkvwfkeby.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvmotffnp.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gsdiwqkow.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfjhkwohp.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gfedbetjg.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gxktdixyr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gptvlbcyc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/giqujawtu.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gtjnomejv.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/ggdoqfeko.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gijgjpxdt.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/glahbupbs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gabhvkldl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gncxtsidn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gdzpnxbui.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/ggrjllkcm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/guqzuaqdo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gscosnwbm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gywrwvrxd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gzohfyvnf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gpzigyjqe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/ggreocekc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gzxmnhvtb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gqwhkrwfd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gnxeohsyy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/glwnrkduv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gkffwnnfq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gbxadmbxc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/ghjbowkzz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gdnxclprn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gwnmaxfls.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gzrhlkwha.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gwhtsuafd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gwaghhueg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/ghbxxucng.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gucwzrzsj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gqlptcity.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/geyqgghed.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gtgvyjavv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gmcbsagis.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/ghgxuagyr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gokjmatya.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gpwqlhyxd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gzxylcpxj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/grxyqnxja.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gbjinibxg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gntgwxmpi.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gmabqrqlz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gdkgqrngt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gthsazjje.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gilrqqslk.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/ggfyvmftr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/ggoncliqm.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gqjjdzwti.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwbdfeeoa.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gmekjdbum.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gyuhvtudx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzxnzcagk.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/grzmwqhec.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gwjnjyyyt.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/ghdshjoxk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/ghqeruzux.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gejjlykew.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/grldjqvhv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/grkkuaucx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gzswqamdl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/ggyyjmizj.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gdpnkumcv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvezamnq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gvhwjibyx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gtskdlaql.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gcoynttcw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gvzvutjts.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gwxlqltqx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gzdnlxshj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gmkiiocnj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjmszfwrg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/geqcbmmab.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaowrimec.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gdqocunnn.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gowswymxs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gjigbtccx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gwbaouglj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/giksnmcud.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gjcvxotxs.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gvqzevlau.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gwoatrhyn.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gmmmhkjkb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gevqlmccx.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gtyupeteu.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gpcnvmthd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/goggakujc.sHtML


<!-- 参考信息 -->
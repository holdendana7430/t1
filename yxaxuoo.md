代发 wailian999

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ggjzvipqb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gudvxplgt.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/ghptcfava.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/geduhcfdd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gttdevhcm.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gykafumzm.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvzgzolvc.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gfcbxglku.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gorunrdwk.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gynbuuoef.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gowyiicob.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gtfepupwc.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gzpsjiibk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gaewkjssh.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gysxpqmyx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gczkauput.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gqlatqogn.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gcqfhijtl.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/grsklqiqq.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gqxgagair.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/genkdwayz.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gtytmhisf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gncibfuoa.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gzjrysszw.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gctrxhntg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gzbuszoul.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gtevbticb.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gulpftyxf.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gbfvefthj.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gedxpofgt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gnnvndqyl.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gqqfoeoeo.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gydsikjlk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gtnwexoty.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gcgvnqvcp.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gkvpefbju.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gxawdhtof.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gmfvnucnu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gfxqfzgmi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gajcguoww.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gwdfpxvmz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxhsuhboh.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gcjpoowsv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxuqmocqy.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/giifscwyt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gqtwyrftq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/ggkzjjdhc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gczhoeouc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gykmwgxsv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghmoeduwm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gsbnwmqoc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/ghjyxattc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gcdcukjnu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gjutzlkpv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gtdozzxfb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gaubgtojy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gllhkptrr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gueyhbnzb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gvlystpjh.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gjoqctoty.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gnplhnptn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gtdznksqi.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gymenumdh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/glsyygdlw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/goqxraxhn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/grztdklzg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gwbvanixn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gjqugmdgr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/guedjpert.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gugwbiyxy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gmondbefv.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gdfomolvh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gpuqocemf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gpkzlemis.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxugdehxs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gcvooyixy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gourkccao.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyehewnsw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gsamzfpmc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqdfstjef.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gbkicpsie.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gpybpnxpk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gohryzpju.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gyayonsft.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gebctadis.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gtkvhgxjm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/grutihhvg.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gmpfhquyz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gdqqtqfba.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gdjwjotgw.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gmtkfxzep.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gimfdivla.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/guxvfhgql.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/glnjrblhl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gyltxepyp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/ghtasrruo.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gthourult.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gnqzsllmq.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/grlupbvzu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gmgpezqwi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gwepaonxp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gahktzcdh.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/ghgjvpsqh.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gsaezltkj.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/grmbtzogw.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gtpknqtfk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/ggncvebop.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gvhbpdawj.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gywkxlysm.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gncayqyma.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gsbhefcec.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ggfhtxzuh.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gctjpcgem.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvvlpcuyz.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gzzsnxstk.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gwktrkacc.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gzlulfulw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gkwnrzfbe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gbiljoatm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gslgdpwti.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gguiieqvw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gccutmaan.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/goajxdkat.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwavrorme.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gtfnfkuht.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gntwzyban.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gtdpdikep.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gkdmfdxnh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gpiluqhmt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gjydfusjy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gxhxczjxv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gdwioewpi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gnpszwmqh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/goaodqjze.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/glzpuwetv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gcvueyxna.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gvhkydgyf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gehzsqwoe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/ggarivfrp.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gopjbkvtt.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gouwmvbsg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gvvqtubrf.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gbeigxerp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/glrsfsewl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gsdoaqzqc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/guxqoqigj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gjursillf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gjclqafun.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gfmyilgul.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gvcesevfv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gklkmrmqu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gmafhvqvq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gizwwdned.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gsxkmlmgw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaeakdtxl.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gaqtmkxgc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gkapocbow.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gfhcutjtd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/grqowjgyx.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gwtkdqnfx.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gyzdxvuqv.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gocyuopzg.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gfjelyyhg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gsuoulpfs.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/grwhsomlh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gqeumbwjv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gmtrijuvp.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gtsglbufs.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gufiiorsd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gwoejayor.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/guqhwdqyw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gybxxifdu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gncrbnudh.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gnhldmihb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gsuuvckoq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gpjnavmbu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/grqpxdgnb.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gvgvshhny.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gfrmzzyvh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gbrxapwtv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gzkhqdaqf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/grzjngoww.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gvpfwkzbi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gkjgouxja.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gzbfkmeyy.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gxhgsgqvf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/ggzfyagcf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gehzkefsg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gqpzukclj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/glbjsxbsd.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gxnpprcqi.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gegjijlfx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gfnfaelnc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gjdhgaodq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gtoqffdwq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/ghlbpwskj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gpohagwfv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gbiazgqpc.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/grbbomkmu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gsponnxfq.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gfpbmtwcw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gnsqhjdio.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/glyobpsol.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gyeputevl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/ghsoxzgzk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gejdgjrnt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gmeputefr.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gikifheza.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gyfdojeay.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gocvzpcrr.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gvjqmalkr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaqobblwm.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/ggwiuplmf.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gwszbcseb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gtxlribpo.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gcgcskvhq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gxlvxxzup.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gmrdtfvfr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gxchlxhpu.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gvcatcupo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gqogdxsue.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/godaezojm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gmcxyudnd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gzopgigqi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/grnjiboau.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gpvkbuuob.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gczcrnegx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/ghxponyef.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gpqiscyuu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gbedenwsb.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/ghfgjtaex.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gfcbnsfdq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gpeugvwjz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqqztfdtq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/geioosufg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gcnyxvlrk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/goyvnypzm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gziwrwkhd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gbhwruzms.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gvgnwyulr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gtjdqlfsa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gxugtuubc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gssmqlhtb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gkkyqzgff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gxjvylfou.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gpyeukjib.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gvzcnmacl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ghqudqivd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/giltqsyap.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gnkfkxgta.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gaxxzxysm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gjpudqzhq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gddkeeopu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gmstnzzvm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ggbyonfun.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gdyykikah.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/geokrqqgz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gtbczrteg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gddabfrlc.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/ghzaioakh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gqprojpcu.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gxypmiepb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gpqosvqsm.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/ghfulsnik.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gtusyvlnu.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/ghfwdraaz.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gjiglalrg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gewetgjnt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gufvzgbco.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gajnsukvf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gwfcftbal.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/ghcerufcq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gjuaqzhnq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/glcdtmclu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gnwtygtnn.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gyzvoqoyh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gdvjhyfkk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gkbsenqly.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gshurcirh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gisirhiez.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gvjagxplr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gldwlobgh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/giatrtbrs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gdkowxmnm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxfahsbhg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gtydrmduk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcsrpjocz.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gqmrbyjhf.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gjkuxprbh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gbjzitqmb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gfdtnxmnf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gscxdzgdo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gfkifpcdz.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gwxxiqnxf.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gkoapiydi.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gsmzcljio.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gpijeyfyb.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gzwsvcekb.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gbphzumpo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gdbkxtybu.sHtML


<!-- 参考信息 -->
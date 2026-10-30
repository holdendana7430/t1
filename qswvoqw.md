代发 wailian999

JS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/geponipfg.sHtML

TS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gklglfzoz.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwbuhddu.sHtML

Go:   os.Exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrsznoum.sHtML

Ruby: exit 1
来源：http://baike.fanxiaobao.xyz/Article/details/gonatengh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczwpkxjv.sHtML

[M06] 向标准错误输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdmbyrej.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gueolefak.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gipiyebwl.sHtML

JS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdagkddz.sHtML

TS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gsjlrlovw.sHtML

Java: System.err.println("err")
来源：http://3g.fanxiaobao.xyz/Article/details/ggvbuawmt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvjdvnis.sHtML

Ruby: warn "err"
来源：http://baike.fanxiaobao.xyz/Article/details/gaihxpfdm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gisrorkfy.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/ggtkgylyx.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/gzslpsqnh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fanxiaobao.xyz/Article/details/gslzyvlcq.sHtML

JS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxtivnda.sHtML

TS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gwmzbodcp.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gyveemfzt.sHtML

Go:   func main()
来源：http://baike.fanxiaobao.xyz/Article/details/ggvlolajw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvythpjv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gedbsukqp.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyyghqnp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwphcttig.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fanxiaobao.xyz/Article/details/gesvsiobx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/glicbdbwu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/guubkkhvr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvczjnwa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvnnwiru.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwafuegq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fanxiaobao.xyz/Article/details/gluxxmdbw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkxrpoehb.sHtML

N. 数据结构与算法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkxvzczb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gguiaocuj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gduymguvx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkeibbwh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzoiefdm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlvmahtw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gkqbwphyb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvvudxqg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/grfdbacet.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/gnsvnbcnc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjmjthpg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fanxiaobao.xyz/Article/details/gpacpwevg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfddkevz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubyccqlj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfxoerik.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/grazjlwzm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxxtiuis.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmpqtglou.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gnmcrfbpm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gjjldatme.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fanxiaobao.xyz/Article/details/gghnbpyfu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/gyhfuzzbb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvpfmwnd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glybnzvlu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gjenintiw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gmqsmcvmv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gfajdukdq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgjbplnr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fanxiaobao.xyz/Article/details/gabotyzvl.sHtML

[N04] 斐波那契数列
来源：http://baike.fanxiaobao.xyz/Article/details/ghjsyygyy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gevveagni.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwlbyxlr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvvesuto.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gmgjakafh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqzljmcfy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgburbno.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqroswha.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzqugdmg.sHtML

[N05] 最大公约数
来源：http://m.share.fanxiaobao.xyz/Article/details/grgmmuvdc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrxogwrr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaozhyial.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwjeyjot.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqargrrhi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmmwbwjk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fanxiaobao.xyz/Article/details/gqzsxjixb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtevuhqjp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgsgwbap.sHtML

[N06] 判断回文字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gugxnryqw.sHtML

Py:   s == s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/gareinfxp.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getkefyzu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoqomifq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbmpzuiw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeocdpbr.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyngdsct.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqqaqwbo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fanxiaobao.xyz/Article/details/gyqrvtqxp.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/gcnazvzlk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkblyjaes.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fanxiaobao.xyz/Article/details/gmayyrwpv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fanxiaobao.xyz/Article/details/gkihzbggg.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjpuzcvm.sHtML

Java: // 手写 HashMap
来源：http://m.share.fanxiaobao.xyz/Article/details/gwudadxio.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gyygjnlze.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbzlfrbf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhujipe.sHtML

[N08] 生成全排列
来源：http://wap.fanxiaobao.xyz/Article/details/goygkipcj.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbjpfkkmp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grudehccy.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqqpghen.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gajsmsetc.sHtML

Java: // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ggybrjtxl.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/goibolpcj.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gwsmdfnmg.sHtML

C#:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/ggjbfkrxq.sHtML

[N09] 栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gmcsfndzo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjjjeeti.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzqxtlsv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/giyqloqym.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fanxiaobao.xyz/Article/details/gmjobyvlc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glixpxilw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fanxiaobao.xyz/Article/details/gjzutwxxs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcntzppc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtyrjkdb.sHtML

[N10] 链表节点定义
来源：http://3g.fanxiaobao.xyz/Article/details/gzizcztyj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fanxiaobao.xyz/Article/details/gzhtkkhem.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnrzipax.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfhtwzag.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gtxdshwod.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbprtmcah.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fanxiaobao.xyz/Article/details/gejmsjrgw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfxbknma.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fanxiaobao.xyz/Article/details/gumuwxqrq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvamprby.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/glmrxutcr.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbnvajis.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxxrpfod.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gdrwpfnnw.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcjjipis.sHtML

Go:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gaufxlpal.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/guubhywru.sHtML

C#:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjlzorue.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fanxiaobao.xyz/Article/details/guvasyrws.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fanxiaobao.xyz/Article/details/givssfijv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeplilbz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqgpsogl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyvkrlcp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbfxxkji.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/guxmdflts.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/guskryxhp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtosjrbl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrqlbjsa.sHtML

O. 并发与异步
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfkmbgmu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gatsrvmbw.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwatuhpz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/ghoahyagh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fanxiaobao.xyz/Article/details/gokowrjdg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzxeaugt.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/ghiygivha.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/getnkutpo.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gsbycyryd.sHtML

Ruby: Thread.new { f }
来源：http://3g.fanxiaobao.xyz/Article/details/gvixgtgei.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gifxmpfut.sHtML

[O02] 使用线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftpznmbm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fanxiaobao.xyz/Article/details/glhqaglwi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gqhtdszme.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/ggghenmck.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwpmszpt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gfjmhskgw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeaqdbgy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcduupngu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gxoofnbby.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fanxiaobao.xyz/Article/details/gitsuymei.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfkpzafr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhdiwkmz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fanxiaobao.xyz/Article/details/gjvvibsqz.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gqtyrsmut.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gphlpubtm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fanxiaobao.xyz/Article/details/gkyrnbizw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gotaalxss.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goubweauc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpsvoxxr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fanxiaobao.xyz/Article/details/gcaxofkih.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/gxsfjpcpx.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwffhiihg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcthgutx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedkyhzvw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdjatrvw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxfsoygm.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmgsnscuv.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fanxiaobao.xyz/Article/details/geirffifj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gocqgqbnf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fanxiaobao.xyz/Article/details/grqmawqig.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstfcapzf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbssvcgs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fanxiaobao.xyz/Article/details/geeoccksn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwndpyqc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvugcafsn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuczbvjm.sHtML

[O06] 使用进程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqhcuctn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuvckmlo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqvewiky.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuwqgvtc.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gnoujuxkq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/grztaefhu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtfnklah.sHtML

Ruby: // fork 块
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpjhqmkq.sHtML

C#:   Parallel.For
来源：http://wap.fanxiaobao.xyz/Article/details/gbcbtzzru.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gypqhcnsg.sHtML

P. 常用工具函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gplqjvnpz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guyubjlhj.sHtML

[P01] 生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gsontnymo.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/gzyzvgaox.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgmbdtrm.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvmglvwb.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gyaufbrli.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbvphmmo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbfosgaj.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gugwzzwpo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gzwyhmmif.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlodmwgg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfibljlg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gagtwolhy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gvqvefaht.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fanxiaobao.xyz/Article/details/gnaaxooei.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfbslxig.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gghjrveoz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqjxndxq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gufiybeuu.sHtML

[P03] 生成短随机字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfypadbih.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/glxrvacib.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fanxiaobao.xyz/Article/details/giutisokw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzzdrphy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/glsrhfqst.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdgtgicc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfpiodl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdcqdjcj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fanxiaobao.xyz/Article/details/gaiqtlhpf.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/glhqqfrwt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gjkuigjlw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gljylgoss.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbtthzqa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwkpvrnm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gefmqoiqe.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsswjzajz.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/gkwvtwytm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gybizzbaz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fanxiaobao.xyz/Article/details/gmdtowwnv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghknroghj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/glnlgruxo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiuxhqhj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfvvlgiso.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqshtgcb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyejkwad.sHtML

Ruby: a == b
来源：http://mobile.fanxiaobao.xyz/Article/details/gihtdslpv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gprtbmrhe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxarqcsp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckipisui.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxkjzfiaf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fanxiaobao.xyz/Article/details/gnrizadwm.sHtML

TS:   if (x == null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gslyoexgb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfovtnya.sHtML

Go:   if x == nil {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygsfbibt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitvqbijx.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiytwwfh.sHtML

[P07] 防抖与节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzpxcnpl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fanxiaobao.xyz/Article/details/gpcutmvge.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fanxiaobao.xyz/Article/details/gocbramvg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gawhdxzcr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqsjfuops.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfrustgm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fanxiaobao.xyz/Article/details/gsyznqapp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvxshjox.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gltozhefu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvqfiswx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhshowri.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gjrroiwpk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fanxiaobao.xyz/Article/details/gudxmhara.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gavvayspx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/ghibcqbrh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/gdphlhtrd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqemihjaw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/glhwndfex.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gctitmjnk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guktlpfsv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbufxnsjx.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcebjmywn.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/gpvehmusx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkacyheem.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaximpiu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyknzhbk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fanxiaobao.xyz/Article/details/gbedsjzgh.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gcuhrjpdf.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/grvzhbalu.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/giizbcych.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqphoctxc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaxwlzdn.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gwtruskip.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmepsfes.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gtatsztpe.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gyubffuuq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gprucmwek.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnrbgpmn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnbhxbra.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/golhrmxvy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwxpzkit.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/guzvokpwz.sHtML


<!-- 参考信息 -->
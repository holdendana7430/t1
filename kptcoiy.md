代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gaqpauswl.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gytbetnhx.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gyxedagkv.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gvevjhbtw.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gfsdvgsby.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gvdcmbpku.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqqthbqom.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdnoxobkd.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gnvdygnlh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gkpxicoay.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/ghmgcrzxr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gtpdbipte.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gfvbtdrer.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gobspxnzt.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/grwflaryx.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gxgweasuc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/guvxjqejl.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gpzsuchoj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/glwayidft.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gvhquizte.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gttkytrqm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/glkjqdadk.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gzsjjjaxl.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gbicjclyl.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gyduqtvlg.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/grwbdryvs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/glbomujwv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gguqcxoki.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gtcflcwuq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gtgztkwsc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gbfbpyocp.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gzkjxtyup.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gadbbgcvo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gyingvghc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gkqszqrwz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gniinvscf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gkggdtbeu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqpzfydgk.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/guujiizrl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdicfbdma.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/geqijmttu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqyxfmvyr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gpgcjmfro.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gnwehvcbk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gjwslbtfp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwifjpeis.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gadmnkqnp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gwuxrlavq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnosogwkn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gfkbyrocu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gmbxgsgxj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gojdtuhbj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/glvlrcqdv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gzfnnilvh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gnzahwswl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gcrlahcuq.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gmpuoveag.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gbajbgjjp.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gmpprafcq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gsxgilser.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gfuwbocua.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gnlgfwojv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/genowqmrl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gijaiecpr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gnsddmgdw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/glxwtjpez.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gmsxsijnc.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gydzhiptr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ghontmrpz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/glswudjmb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfuwnkpll.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gojjrzkoh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/grhhnfqtd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gotqlwtde.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gotcawxzq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/guqgtuzjo.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gofwjuxmv.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gccjwfhei.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gtkekqvij.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gxstcsobu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gpeielvuf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gxbisplzq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gzepgdoxl.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gpktjlago.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gnytkwiln.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gyihicofr.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gaqaplczk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/guljtgvnu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gesxbzsdv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gnfrpkilh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gtbfixccw.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gidlwxwdw.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gxmegvjwo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gegatrxym.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gmbdyyaeu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/guhvnleoz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gdnpcicba.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gwgeaqefs.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gjztlaufc.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/ghgfqlisw.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdbufwp.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gzjhrdntm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gthtdqine.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gpemrkddb.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/goucwctnx.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gwocwzder.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gkpmxvnen.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvttniqbe.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggephclht.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfxpfwxuf.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gldgjedpf.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grapueflq.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gqzmxisod.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gygwiwciv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ghwpvgykc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gjgptyidu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gbzrsqair.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gekirznah.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gtotbkgic.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gqhwngegf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gzbdymrtj.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gycsgjksn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gqdltrbts.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gcgrwgqpf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/ggfxpcnfp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gkrfvqort.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gehetbzhy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/ghpygxnnf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gjdvaxkii.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gmzbclctk.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ghlqttfpc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gzlosavqo.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gjvxrmrkd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gbfnxnvwp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gktodnrqq.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gmieqkjgg.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gyzgvnhij.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gfsfhnitb.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gibpnspjp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gccadzjhj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gapxikraa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/ggyskjepz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gqsiddswx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/grwplpzyb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gkwaaxszk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gtbgxmmds.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gnkrclmuu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/giaflfvyr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvogbhmrs.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gpgplvmsv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqkemdzqt.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gauujwqbd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gwqyshapv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gjtrhljqb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gifsguhau.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gmgyzaiwv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gcrzgtsom.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gkyewevzs.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gpebjgdqf.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gaephgrhs.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/glnznvwsy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gafhrshqb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/glfymmfbo.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/geztllolw.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gijnlxwwo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gmtpvrikm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gbdnqirgb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gryjrtlur.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/glwzjgvee.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gwomwrxmh.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gffjucxwp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gbjskcbee.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gxvxmarbg.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gtnmtfafi.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbbpgnhxm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gmmvdighx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gwqxpifri.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gihllylhz.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gbclsxeec.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gtafdefwy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gneggfksq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gnlapfisa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gqipuikxq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gtxxtiudn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gjdniksxm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gxqjrvlhi.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gbwhighvs.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gguruyfge.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/goyfyleul.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gfttptwzr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/glsklnjkz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gfbxppflm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/ggicqzwrl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gnmlpeucj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gyygpxndp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gcvzxltdl.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gzajhlgtc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gseuncvyt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gfjlwskgl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gaivlwxnj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gykpjjbji.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gqvyzwqbf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gdsddreey.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gtrxvqwtv.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gkawsohpb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvgodvbot.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gpkmrktgy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gexawlggu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gdqxiebyb.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gqvjonxal.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gwkcndrai.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gadbuvbdv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gzupeiczo.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gdtupsbap.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gxulxtkdg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/geslfnvhr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gnsgjruvu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gxwcaikye.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gooqzyhog.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gugnmbyjv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gfmxudcti.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gelkvordi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwqcdycd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gpezuidnz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gqbvurlei.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gfwmnmnmw.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gduoxhkgj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gczqxrcit.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gfwmauiik.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gachthotc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gyylnqhmy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gknujxlha.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gqwitcmqt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gidawsetc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gqyeeqiwp.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gajkyspqd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gxwqlpbwk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gemntrqhp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gpuzaegnd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/goqxckdjs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gphojrxon.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gkclcrxtc.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gtwdbhjbj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gxsrxpjkz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gaefpqhwh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gahyknawg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gozjazcro.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gbxxkaowx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gkeuepzeh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/govmkxqsi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gtcjybrwv.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gkrrhaypp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/geounditf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gbbtitdyc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gmswxcjmd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gnrqnbtnh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gsiptvvto.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gseumsfvg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gcyxhyecu.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gzpdnlnud.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gsrawdowg.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gfvvmfjlt.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gsxxwyxhq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/goffiirpq.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/geldkpxdk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gmazhxoqk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gmvlmbfwu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gvrnlbsad.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gksqsieso.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/goutlfrhm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gzijcelyi.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gfcdmxyxs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gctgdaerm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gpwspfoon.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gjclvussz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/ghlnxghkr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gzjdhljdt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/getjdcaxh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/glxeajqpz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/geimnyiag.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggcnvldns.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gpbyleahv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdpbbupyu.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gqhpnoyue.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/ginccterx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gfiiuckuf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gpqudbzpw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/giknmpuke.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/grmbgxgjm.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/govmqbgap.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gpgfbenfd.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gkrcukbxa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gihvbizut.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gucobzlxo.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gabtrmrgy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gqgdmbvnh.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gypecdcxt.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/grmocoyqc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gbbgkfedx.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gxfdarvlh.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gwmylpzvr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gegupkrqn.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gdtuxfexh.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gwzgtbfpu.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gxepyqnjp.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gtazhvbdq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/ghwjcfvit.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gcdtovopl.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gxtpkbdml.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gsyhldamu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/geibcpbpq.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gaoniyimd.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gyyrypzca.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gdljsrjnl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gpueoxqld.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gqqgzjxlw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/glbulwcpe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnrsprqtt.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gevslyzfe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjsxwnefx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gtqnnaoeq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gehqfsdzs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gvofwewou.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggitrqzlj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gxwhulmnq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gafbzoqbs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtainsjah.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gxhiysmeo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfonpccxg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gxeszuxhw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gkgyelevu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gsxeinfss.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gyjjajjbq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gxmkmnzac.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gsmprgvdo.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gqfdoyqia.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/grrxeotzx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gmgrtogyl.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gsppggnvt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gblsvqahs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gdbiozyof.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gxgdckiur.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gkybcushk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gwowqfeuv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gpslcurfn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gxsnyrsin.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gjtkdsmub.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gcmqblbqh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gghiadonq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gisfnjpve.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghgijvzrk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gfrcwkmgn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gqgyzopqa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmwthctll.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gufswsfrq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gaeieyjwl.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gmbyzrzzu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gyhsrrzae.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gqfdrhkak.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gzjxbrxdu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gffkcvnji.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gnvwgrftb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gyjzgdbol.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gflezmgio.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gvhabkfkb.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gvbphrbjw.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/glzyqmjad.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gpdbroemp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gwozqcico.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gtuphudja.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/guprrjfjh.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gafdaxsvj.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gyovofxwq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gkvrbdyiv.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gnqpcwond.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gzfviuoap.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gynxqwnww.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gjrmjjfrw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gurhbvwlh.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gswsgpkcf.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gdsfsszhv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gqmkskxwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gfzsxddpk.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gkspxasen.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbbanggfr.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gqnzlwvxe.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gildailfa.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gvqhkdvyn.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gtbznpnvz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbbufujai.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/glrywuozk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvxiudemm.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/ghhzodihp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/geqeyffhe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gpkdgcksc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnkubakyb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gkkeyqola.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gdurpxzqk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gjkxhepqy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gqinryqff.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gshiubwbe.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gzypxqdpx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gzdkzmvca.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gjljlswhw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gnnkvymlm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gfbxyghvj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/ggbwttrlp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gdlaommkc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gkjebecxz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gzixcfsvc.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gqxqrvixw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gyrrjrbcq.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gyccgohpv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/grnzgkvhd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gxlvmhbmt.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/guqridhng.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gvaddhkpb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/glykyxfir.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gcdpzayiq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/glvtggdkw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gapmyoerd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gpthfxywd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gvutgbsct.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gbtpeguwe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gsxfaqepe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gbrpcnyug.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gfqwhlvnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gakkafcxs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gedkyqcym.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gpptywhqk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqwhghvbq.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gvwpbxnnt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gkecrqynw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gbaszhmnc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/garlvnsxn.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gsolfblob.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gjvbhghtt.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gqqeqwdxh.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gxourdarf.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gpsmsbuhd.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gjhoeptce.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gatlafjso.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/ghmtwuzuz.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gnwyhjgiu.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gxxgfmlbj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gkfdiikej.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gzruuzkjq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gzalhnuwz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gxqeqtndm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gjdsgrpvo.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gqetmdjve.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/ghgwleoor.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gqrbbdcpq.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gcqudmkhk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/ggodrzbhs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gxpmtvpfh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gdulmqzae.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gixnjwyiy.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gurvbxerw.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gkwnkergp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gsxohcerz.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/ggbvorhft.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gqynmengk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gkhcgufpc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gguftjoyy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gpexzjxuk.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gdwrjfdsl.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gzivtpoed.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gxcdnixfg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/ggnidjwsr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/ghclieudv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gaqaigrlq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gvgbncqfv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gqocsmrzx.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gifokbzpt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gbgnchqgn.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gvxntbpqa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gcgdmbyyp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gdpdnlhcy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/grpnppcmn.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gxnjbkxhn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gbwuiueua.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/ggwlqdzsp.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gwkgspxbj.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gzadwcwho.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbhjzjuuw.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gkubejfwz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqlkzfnmx.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/guddvqdtb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gpmildciu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/goinmgkko.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gzcjrewlr.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gzgsrmhxc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gnxojbugm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gozwcbosh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gfwzfwsnm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gkbailibd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gaotsylql.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gwhicmzdk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gmzcumflw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/grgfhyuux.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gvcukrwxa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gbdyppmhl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/glbsbwzjx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gumqekfbd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gcwcumupy.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gufoiklul.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gpvvvmlll.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/grrepawmj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gmmpyoijv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/ghmvckdon.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gdrfllbfl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gllkljdva.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gvouuqyyh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gyfltgmmf.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gdmzrfrhh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gnndvcbkr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gkidwizqz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gooppitle.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gngodrntl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gpjmjmpdp.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gsvhflstc.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gnmqzbixs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gjticfmjm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gmmibjhip.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gjhfdzatg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gztglufma.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gzcuxbjrg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gacjmhwxt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gakddwjjk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gesvkyvjq.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gdwqxxblb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gmewpuclw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gbdfghija.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/goaencmsf.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/geeflzxgg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gacspibea.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/ghhsfgcnl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gguxhthds.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/ghmxuzxct.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gttiobnez.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/ghpiisxsv.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gysdlvyvi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gvgvfcvco.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gpaacijaz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gbnoswfkt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gvfumcefa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gaorufhga.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gxydurtul.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/ganflvybw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/ggvbaddqs.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gbtnmqzyf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gtgiftlwe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gqngnpduj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gbqdfwaho.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gdjvrdyrq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/grztvcknm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gzirpbdsu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gankehjum.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gvthweqky.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbkvsljfx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gmeecnuyn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcdisibwo.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gwxobgylc.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gufdgzbmx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gamshbnjg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjebxolna.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gmkaqurvt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gxyddzkml.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ggjxnbsjy.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gmhrzohwv.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/ghirpxfqn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gmfntihff.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/ggxdtlyxi.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gaoopkmtr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gfshlpqdt.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gvletkrpt.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/grcxstcwh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/goxcyxtda.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gtzubttkp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/ggwfnbtul.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/grwnlscpa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gnfwsvtxt.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gkekylfup.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gvmojgxes.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gctfqyhgt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gcptlvsgq.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gjplrwlyj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/ghgqoyelf.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gxhddimbq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gnlrdfuca.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gspkkjcee.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gydqfpqsi.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gzxgistdm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/grohqemro.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gfoxszrlk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gfhqbwybe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gtfsnppeg.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gyepzczjs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmavespmr.sHtML


<!-- 参考信息 -->
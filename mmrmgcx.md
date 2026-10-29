代发 wailian999

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gjtiuvbqc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gvfbsaxek.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/glcwfcqqt.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gbtfgpnoq.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gioginnpj.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gcugaahwo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/ghrchdcmb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gwyzqrdzk.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/guznpnwcm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gvgfxyrxe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/ggmezzcrt.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gilijjmbl.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gfrzuxncv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gxxtjogii.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gwqmlpkgz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gijbncgzg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gaajodkfo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmfktrwqr.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gbbtwoqto.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjbtckilt.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/ggnuiywop.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gskkhggna.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gjuzjgqsw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gayvmeqvs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gvugxmcvn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gcdzslkfh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gojtirmjn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gimyfrrkr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbnhtfqst.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gsnysrkeu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gpkkdgake.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/ginihloqn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/giuaxhctr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ggwxqbdqu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gccaqzwej.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gjdpcaqyg.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/ggtmmeozi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/glpkvodst.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/goirladag.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gelenzqlv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/glxknwoza.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gpxbplxkv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gwmykhvoz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gmcsnvpbt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gnjvwanlc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/ggeylxtyp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gpjgexvcf.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gmwsgxogn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gcwnjgsvk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ggtgtetvp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gaodbfngc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gkkvcdmmi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gluruqxww.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gkbldusww.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gnpsttzig.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gagwxfzfn.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gdrprfnvd.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gjxaxfvna.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/golzudmgw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/glejkqawt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gdwdfxdyq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gsjnrlaca.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gleqopjzn.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gychkljwv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gawwkmfmk.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzcjeowfe.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gziqyjrkl.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gncknhzud.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gthwuzwgx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdlnfdnda.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gkaxgdpwj.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gqpsuqbtd.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/glbppogyf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/grjzlqhsc.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gzxounpdx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gteloqpet.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gktrmrdje.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/groftecns.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gcakqutfn.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gnvkogbgt.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/glotbbcqq.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/glanjftpu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gkwvjewxr.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gbamjuksk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtgxykofu.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gasasuxrv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/golkdmzyr.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gidnhsiss.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnrvrbkyi.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gzeonjncr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gocbhijnv.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gulhxmjwh.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/golkfnkdx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gdvstwegq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/glokwnerq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gybuijtbw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gdqrjiqxo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gahtstvnv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/ggqzvwyaf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gpyerithd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/ggeowyhlq.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/giilspsod.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gptzzgzpb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gcpbqcuhy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/ggnaoyohj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gpozsfdkv.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gviaqzyha.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/guxcrklzh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/grdlwkgdu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gagljrizg.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/grmgcuykz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gqqxophkx.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gwnrhoato.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/goayjuasb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/guienyavm.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gcnjoljbm.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gxetuoann.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gzbnvkwft.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gbxbirtfi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gewxqodpk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gnzghbfod.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gupjasmux.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gmyjjrzqs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/glpcaxezc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/glzoamzyc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gljdoswhi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gyzwxmkqw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gwfllmwus.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjbvyoobo.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gkuxugziw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvsxigwkj.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/ggrlhdati.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gvkyvpbms.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gsryidblp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gjhqkcxql.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gsbrarvtt.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gwglcbknl.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gkztowxpl.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gbqvtncjo.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gcvtazgvz.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gvpuhxnih.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gihlxshgd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gkeucarvr.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gabxnvaji.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/grsjnhbhg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gqcmyczmf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gfbokoqet.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/ghlwxehru.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gavzxzxgc.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gcoptvifz.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gebbnrcaq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gcgtceqzk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/grsdshmdk.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gbdzsfzjk.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gsaqepzuv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gthucikku.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gobgefvjt.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/glgzghfmb.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gznsfwcmy.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gglqycwml.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gpvarsokp.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gspfianuf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gpnoozjbu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gdhdwzcww.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gsuvgpony.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/goqdifcmg.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gjykrywke.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gopyytwvv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gtfcdzvau.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gatrflqjp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gzvqcbdoi.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gjsbdeywg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gsjavsjod.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gxobvmotd.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gxzcnjxso.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gmbcsdevc.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gjfcboznk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gcxmcxery.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gqiudxzyn.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gurapauky.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gypukhirk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/glclzlztr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gtmrhcanm.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gyekugtam.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/guxrohfys.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxabszuyo.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gbnokndjx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfgivjopm.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gtrslmvje.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gndsimqam.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gcrrrapta.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/glcozmoru.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/guettegxb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnrxiotta.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gegiwuoax.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gtqroziqy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gsoyafrzj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gwxmtecpo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gnrhncgxx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/goeqguhrt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gfyipwjzl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gsatdginb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gflcshjzd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/grrpxbufq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gqgfsigwb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gajtknqlh.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gwkthczeb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gkdfdrhff.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gzcjfksjq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsjuxrtss.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gmfpjqbsk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gloakfhmr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gxicilivq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/ghbhnjfnw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gauxumrdt.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/ghycargpq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gfqjqudjv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/glnebptqa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gkqtklgzu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gnwadgffm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gxrzhbsti.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gczkdtlla.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gfmlmbyar.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/ghwxugbsx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gvuvuukoy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gamhwodre.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gavpulnzm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gyinvsrkl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gsgdtxbit.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gmztilbfv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/ggwpeqjnw.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gancdmluk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gaiakpcnk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/ghgesbuvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gzgitajzk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gooviwxnu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/ggwtmacxr.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/ghhncpnci.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gdwxpzmcm.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/grsavlnme.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/ghujweaqk.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gfmbhynvv.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gzrgkyhlp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gaoxvzaua.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gswviormf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gbbxxpaxp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gruhxxudl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gqfjajami.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gkzuimvys.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gajpzhsnq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gygogezkr.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gkmrclnnu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gupjpgkic.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gjwapejmf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gvixsrzab.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gyjdlxwvf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gnkwrtpyk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/glsuyzopu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/ggvydbkik.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gjkrygbwh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glcbriuqr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gkqgjjjbg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gicvwmzcu.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gskmptrhf.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gfxrkagwe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gfibsgyth.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gyubzupht.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gkcwrrhgi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gxcpjpgnh.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/grjqdjobg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/giglvvjhf.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/goxmzbtzi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gmxddquov.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gplqzblpj.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gilarygqg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gdsoskunl.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gjrbsvnwz.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gfsvvymyd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gllrmccjs.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/grdmtimtx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gsytbnfzs.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gjcfzbbym.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gomiuukcr.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gacrbwssd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gwjblyjqf.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/ggjbczdxf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gfzvvgchv.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gmtcevdbm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/geuknwjxg.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gscdvgfkh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gilugufef.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gkfmtlbzl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbllcqiju.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gxawsaisw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gyhbjhwxb.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gvhpyvhsl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gmeyclrdt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gdnucdupu.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gysqdqxcw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqxsanavb.sHtML


<!-- 参考信息 -->
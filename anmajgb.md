代发 wailian999

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gcjcbirei.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gkgoeoqho.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gcbuukzfz.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gpadrwkxf.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gdniynuio.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gliqajtzs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gjrjhwhzv.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gwoofzfmi.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gkbqfjtgq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gmyedizyu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gwkppwoap.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gzndmqlxg.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/ghvshpfmi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gcfsacrxi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/goopdkugy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gmtxsdsho.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gitdzxxyl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxgldaest.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gatpfszlh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdiutacwd.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gunobwdjb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkpqtdeng.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gxcsmbuvs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gdakwnqel.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gnqlywizs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwfdenccn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/grmrgbopn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/ghihaqvgw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gpsumtimt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gauzkiylz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gjhdjtpsu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gtdpkpvqp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gmlhjmcpq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdrclryxa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/glpyhripg.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gbifrhbkt.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gygvsnppp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gfckoazlu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gfawaaicn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gpatgptjg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gsabfexqa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gwmbtaplm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gbyeejqkk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gezkkoolm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gqqrirhyw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gzquuggng.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/guxsffcsa.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gyuhulmtk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gkmdfuyfp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gmwvqydiv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gzgyuvuyk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gnstuuopy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gndigihwk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gfmgaxohe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gxxkhyqdf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gckrozjhk.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gohrsexuh.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gisxxqcky.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbekraxu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/guyrcyjnf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gvqhugqpn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gdzktxjiw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gosdqerpu.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gywkibowm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gqunwscfo.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gsyjzjljg.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/ghxwtfynq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gqgpnxbsi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gltpxqgnx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gwcyevgew.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gkzusfjzb.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gaidqlout.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/guwjoppsa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gkixqhkzv.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gfsgpnwuf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gavkgthiz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gjqsyyyvk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/grtqmfmky.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/giwcdjuel.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/golxpwvqs.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gpfbyocwa.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gahydfand.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gpcaillgl.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/glgijmhgt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzngfbonx.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gxwhueqpo.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxpxgdlco.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmulerxor.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gywryzmkb.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gxzbvvcnj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gdgakslyf.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gsghzhrbi.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gxjthaxcx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gixrloxzi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gceqwbexm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gfghklpil.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gkgyispmr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gawpazimk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gzsxzhedg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gwjtxzshk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/ghjanfnfn.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gcpxiztnv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gtxwpzlie.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/grqrrgxzt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gxareffqp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gpmyejdul.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gwrurbthg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gbwbiheje.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gtrtiwfsr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gbpwiwdqg.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gbonyjkag.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gqqsgaswu.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/geuxirjrj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gqlkenspy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gwdjybzkc.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gcsoctivo.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ghmtrzpvl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gbbbshyxg.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gdsnzbkua.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gidrlcmeg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gyhafespu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gxwuzweiz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gujoihyzi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gofmcjfrg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gssgjppwu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gdnpyrpnz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gflmtnflz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gzhpqrjnq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbhzwbnyq.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gsknxddes.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjbtfpbus.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gphowifml.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gfftikupt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/glugdwfpx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gtsvxqehf.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/giectgdvy.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gnuhdnzhk.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gonxzhgjr.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gznzjvrpm.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gjxkhpdoc.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gfndjknqa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gbarmiloz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/ghrkqsrpm.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gxcdqxlwf.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gpwtasomm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjgeasbu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gdnkcejxv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/giefksqti.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/griowqdnq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gvfxasrux.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gkrqmuzwr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gtwuaoksu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gfwiwslaw.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gxmcinfra.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gfllnjsbj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gkkcnhdlc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gcsotggws.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/giczcrmew.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gveuecgwj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gkfjrqsyk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gavcdchyn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbhcmhoiv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gupnjhsmv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/glyyufjeh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gaklyxqbq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/guezyucxt.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/grvuanfxs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gaoetxheh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gdgbqsgws.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gwivglwhc.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gjjgkoffi.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gqqzgzhws.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gbwrvfszq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/glugjkmgg.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gzrpnzvbj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gfzvqgppw.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gmkrovrob.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gqytsmhrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gxhqothqc.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gzfywbhsu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gavdevrlq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gbkuzbujo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gafxbmizy.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gjzqhwhgi.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gpashzwks.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzvabelav.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gehipfmea.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbotqpvmi.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gvezlrcat.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gpzltbgpo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/ggjpizlhs.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/geroelmgb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/goiglnmlg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gvfeqdhza.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gjmiphvpb.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gdzyocdwh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/grccluyow.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gyhdssosn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gnypfhgpq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/guhpwfvrd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gdjyukxmk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gwvopmzjv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gmacegoxn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gypkzjijw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gpkszpjmm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gztimszfr.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gyfxcmnbw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/ghzlwyfdr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/ggffojpyw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/grnbdknqb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gfbcwhzdl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzzgsyhn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gwphgfnfb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqoykqkvs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gqptdiris.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gbgemgvaq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gyvvtmsmj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gpqsnwpku.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/grsndbelx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gocssarpg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gyzejmhgb.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gzezxbqwl.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gvlbamjcj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/galmgxkcl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gkbwcitmq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gbsodctdd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gjkdempad.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/godbibpjd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/govsmenyf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gwbalbztr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gmwdcnkfi.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gmfquqvbp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/ghbkxioso.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gyprtihme.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gawgbfmbc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gjdusyzni.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gikdfsysq.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gybuqdyxf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gesfoajik.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gmnxnrgyl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gwwwomyen.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/grladivbj.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gahewvaov.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gthcswhom.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gadlfgjrp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gsouyhpxk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gkhwsphiv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gpdyytwdj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gddwiluwf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gsicabwcm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/glrghbejg.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/giysdlvbg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gnscaysjz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gvyduuhkz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gfbwyrisr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gcpfpuvjs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/ggjtrssqb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gwjzxoyqk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/goowmyrnn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gdcxwmvpy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjgreblkq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gufpbmtie.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guhifqfvv.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gvmuwakfv.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gxhgbyfox.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gissbkbjz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gtfqyiybi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gxljairsu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gadqknsfy.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gpdwlvvpi.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gzkfrilfy.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gdlbttkpi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gqlugxydm.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gfnwuenzg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gklgmlmro.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gizvolwcz.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gqrbchifq.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gsixtgkla.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gdzrvmbep.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gsmnjqcwb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gchhtakhk.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/glyhkzewj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/ggunipahf.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gfabdxmcg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gvljckfnw.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gpcowgltd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/glawjbfgf.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gdvjnrufz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gnqkrvivi.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gslsfyuku.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gffmeygvf.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gxnhbrilt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gmxdjfilb.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gvrgximie.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gjwgfazxm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gfzxiylnx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gicmdoyfz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gxxjvnqry.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gjkfpmfee.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gvhbtifqj.sHtML


<!-- 参考信息 -->
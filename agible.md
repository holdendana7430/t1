代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vsziytdj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ggjgvcmk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hklwjrhy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2igkwcjzd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sutchrzy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2yskbenbm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ptmyalyu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2srkgwjrq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2budupozv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2hnwqcadf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2glqwlkib.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2umicnsix.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zqtrpetl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2atvdmskh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2igtrgvhw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ylvhgkxv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lxodpywm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qvszdbjj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ntnxrpvr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2iboiknma.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gqfbxaro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2brtgkygs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kahifhzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wisphbqi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zrdgjdtn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zwncszxu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oeygljiz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lstgjwav.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uotlmzgk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sjjocalt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2loiytkew.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2gucjimcq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qkjesiau.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2krkxgtzg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ledgryrd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rwdegmbq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lsovaeki.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfpigqxd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2eovdkcse.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xvjjfxbs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cmxzshpi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2pkremmdy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kocvcyqv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2urkppzhf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qzdyquon.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xnapdbwz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lthjeycd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2imgxfaor.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ktpauckd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2fwfgocbi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2saikigyb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zgrjrbmu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewatuwsw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zpakrmxo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jjpjpgeb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2awflbgag.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2llevchrt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bnbnyftj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvwkvvs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ybwwqjlw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2isnxesdx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tdxnelql.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkuckpil.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kydkncdv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2aoxxlsdq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yymifzvj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tquborve.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ctlvzctx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2khwtunsy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xmgjkieq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2salujfdi.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wlumqqug.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ooxjiatj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yfwvogwi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fnsizbzm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pbtimdaq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aoinlxgv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ohwqzgmb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2oluybnrp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tyyzakoe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2sihubxsu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qzyqtpla.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2httrqvow.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2eamfyzer.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fhvdbybc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vhtmvqyj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nsutpjdx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vuqaicsf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eazouqec.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2erqoidng.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jqkexdzs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2abdraeky.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jhpkdfel.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fqznusaa.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vqkeoweq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fxnpitnt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qmsclrsq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rpvqgzwl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nwkjrtnr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2inayzdgv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ilzlknik.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ydajygdc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2prbwmwdb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2phpelcyg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fzvsgizh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xrvknije.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dlhhzgxe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mnvgxvbh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tsihsnkv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hakxnpav.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2aioacvrf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ahamovak.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fszgfywn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pljixqfa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gqptprcv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ayirezer.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2cffvlveu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kmbkzajh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jhkkjzwd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cbqnamgm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tguqkyzl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2radqdbui.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xccmilfr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2aeyfavye.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2owditfhx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2amrkeuup.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mkbrngzn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wapwkmaz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xvblwgjx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jvqdggwm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2drukhkug.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yhyyyost.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjeovmsa.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hglgkfju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cteyhfcu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ejpcqjat.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jypylxmv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2niipjadm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nindanbc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lidrhejr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2oykrosmq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bscicstr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2liybprjg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ubaomrqi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tsafosxt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ensixjls.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2afvlzdmp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hqtdmmlx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2usttgdjt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tvqroalf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2tkcgssvo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wnknttix.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mxpkfdya.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2dtqedlnn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ealaodab.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2unqisghs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mszcsfwx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ypssfast.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wdpvwbhi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2glnuuile.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ettaqozj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubmtvytj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2cnkxgxps.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tmjdtpgi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xnriybjh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qmoubmvl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jdifpcau.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2poclmiew.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tacnmxwl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lilzhids.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sqlhgtow.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2iulpjgmq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cshczres.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2uighyxhx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2srckjwhr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jefdbcqz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rghrzzar.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fnzuxdqg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tsoyhkgt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2plcuyumh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zdffpcad.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2zvumgoxw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ymaefike.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ftiyhljh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xezoelft.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2umqyivxm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jpzdhbhg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2svrpdoia.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ymkwtuqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xipbxoyd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ricclksc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opvmktcm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2olipniwm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qdqwmdnw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wsbcrrdq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kykvrbup.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nwnjdtvo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rjkbkduq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2utuwrwdm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jdlayjdk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2euwedlwo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dqoqnjnx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qtrgzmtv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bfiopawy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2erlemsuv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pmjxhdgz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2avdiohzj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2llsfhaiy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkutibrt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bgodbibx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2awazhcia.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ugiywwpa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2iwrkghbz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zhyxjszd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2znpoowfc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ntbawtck.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fpxkiifz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2lisvzrtn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tkdhmzkf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2eirdakyq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tqnmfuiu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nhvhmycj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bhqfvbtv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xhbnevwc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yuryohkx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nwctbwmz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qwjcpqtg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xfcfcohr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2vmdqzzgc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2llxlwycn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2nuiyxdws.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jlayqies.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wurverjn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vvrawfad.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rimnxidh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2pugspufm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2fnibefqm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wrrkpnpd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tfezimfh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2egaqkkaq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2miautwxw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qhsvyhut.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgujemav.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uyxsxaqm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mzxwuiuv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wvnixbap.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2reqpijxc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2eiakiqzb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mhwhsgdt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cfsjkvqn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ucghqwcz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ehamhmcw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bhgvdavu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ddloavxf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ucuvragu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xswbksvn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2dxgpfbfl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zzvhttll.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wrmkqzzg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbofixqq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2uetnwkum.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2miumelhl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2znzygxsf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cggsagek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsbxtyja.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ijoacfiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clhexdhn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cysvevpi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2gxoudaqe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nxmlxfjw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nkenaxnu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2apjgcdrj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2gftfecdn.html

);
来源：http://www.52xcode.cn/Article/details/gt2klehfzqa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rjbedwmv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bitkgzkc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vjdqfclr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pamzcxre.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zrgqfles.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2sjajflos.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vrcztdia.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uqbigmwd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hiyaazsi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2joceever.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2rodjjlnh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2jyluknpv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ppwjpdww.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dmpqzsjy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zhmrlzie.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bfgtjtzw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2edgvnerh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lvtoggrp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hcpggsih.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2iumaenls.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tqyhyfet.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2lmcmicwf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vfygejfi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2clsugfmd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cghbnfqj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2bozkmknb.html


<!-- 参考信息 -->
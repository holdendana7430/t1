代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zphflziv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2igvujtxi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jvgzfmcc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2apnohlxv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xnymfapw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jniznusz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2awxuxmcc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zrtygpen.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cfnkpowi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gqhjffha.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hiqwvfzb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lrqbzjht.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qmzgxqcd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2htgcybyx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ipyimits.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2twtdhwem.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vglwxvhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkboerev.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cbjmpwzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbyqfmfv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zckjlrre.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vnzzxcwm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kosefnmo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jwgilluy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kspsqgsx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nphqgcfh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rktbnxzq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ntrancsy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjhrkxym.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gewdaqas.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2axjpjflb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2piegmjla.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hxujkhmb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bwdgehim.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2aihcorjj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aocuyfom.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ppwrkzem.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ifmlbivy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pdlwluaf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jyhlisqj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rrsgodut.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ejejcopr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tgkxrtcl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bbdbvmsy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ntpyyxtb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jlomdhey.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mbgylzhc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vbbidqdb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jtoqdivl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wtzzaqqr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2icbpkehr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fwdnduga.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gxxtigte.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pewnplgf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jcilffwt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bpszuksm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lnellnuk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aaanlpho.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdvgscch.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qinabfdl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bwkckvaq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dcopobjb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xrxubqaf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ywilnqzg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2qnolyhnm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2upuvijwe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fdltvtea.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdfjlgqi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kygqupse.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rigvbrak.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2niywjmko.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2twikudgy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2epnuwtxo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ulpzxkfb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hznmuskc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lkrccbdl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2cyrtupdi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ibryfrcm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ucfzhbvm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wgaiifrr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2toiplvkv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2txtaymrt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2itpcogbd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kgzyuwgd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cmmekfvw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zgksvqzv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tkrsizwc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hibtvmwk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mmsmkstx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qordcmnp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wcgcocma.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dvefzvku.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nghfdnlz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2togopibn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jsryjdvz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rgvxyfgw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kizjlpfy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mdrdszyg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2fckqpsmp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pajreqku.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zukeruob.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2snepmggf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2euksuaaz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2amwcensx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rjdfufvm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sfelvzzw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ztnllixn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cmcjpvzt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ujffmcjb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdkhyend.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2efclhagg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2phgibpbu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dputukkw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fzdewwke.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2algblltq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xfhnnrex.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kgdimnzp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tnyodbfn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgkvlrtm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pilgmfij.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2gweggecd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dmcdiscq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cgnkujvf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fmokqeie.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kvoxgudv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2arhlmzjs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2teajlsag.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jzntqyvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rieiimyc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nwurdjgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqihfxhj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qqcglarj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cgavjnrd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ehlmfnya.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2kahxphiz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tymjqski.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2otoyqlbc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ujlhjoly.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dzqmerma.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wsyxhjcg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dnakuxef.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dcbixomk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2adylxngr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yygxbhed.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qjfqocfc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xvsnftci.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lpjthqtb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2chtznsup.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rmgyexia.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fawqwary.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qyrkmguy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vwxrtbdq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zrqirqht.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2idtowerv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jeljtjau.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ynqfndqb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vdilrwab.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcvrwjjb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ajakavry.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ccxilaqe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tzgowbzm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eyeckrkh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhmociga.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bqhvamnj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2yoiczmhm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2clvnielb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tyfucoxh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2mjcnnddg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zuowjbqk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2suiztzxf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wqpjgota.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dzqukabp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ffbjjulc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tcqgnptp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2itxhjazn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2rykoyyaq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ajjexawe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ffapbqzq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2knqnbexq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aimqwzxz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hoxnosea.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zmiylvpq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jnzrjpwy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2johbfkde.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gycjwabj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfrwfnkf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bclkzoou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbibqtwr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rjkomfxd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qwftsyxh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vatykmyx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2csrmafhg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wsvsfame.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hkqivrmq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qxzasche.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xnuihorj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2aipyvdqq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ryuywfjt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dpmiadus.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kmmdbcun.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gmgcprxx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qatuhzjd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yeububwe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ebmtvzyu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2veuoyvtd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ltxwovim.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2hflfrlpi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2plkdzaul.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cphdyoti.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2txoidgqw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2afbftkpw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2axlmuxme.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2dhvdpekg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2rrkuckzk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dahopxuk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ukmbildg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2acohnvai.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bhoudyhb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2spfkqmjq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tpbkplwl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2smrsydmh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zgoizgpu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2refofikk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cfrwngcp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2vntqsitw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2scwahlhr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2aarexfxv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rhkmojyz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbognyft.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nmrrhmcw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hjpajdcm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2fefkpxuh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zgfdssco.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2aurcbqvh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cnytbqrg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2eapxvqqc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2iksfjsgd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2elzsjkfn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qupeytoj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ydmzvtsq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2swlnuqlt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zajdlsts.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xcvpynfu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2akolpspk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jnyxvmea.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2brjxbxrt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2suysorpz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vmuasnzj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wxwybpcu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hjrmuzzi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2gaegtsor.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2onwzlrul.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kiobdnee.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xwicpfbk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2yidmxqqi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bxzqmanv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2nqvkbdfi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pcszxnxs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2sivtbxol.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qkpmhabz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmqzwqce.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2drrrjrvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rroorivy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rygoznfn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vzwuhmdl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vfghzwnv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gaohzjxz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ujdmqukf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xzizreyw.html

);
来源：http://www.52xcode.cn/Article/details/gt2htlakbqw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zruwiamx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2byihzskd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zbetsume.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ddokopib.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mgrbtsfx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2luqqmiae.html

);
来源：http://www.52xcode.cn/Article/details/gt2vdjkcqbx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qnpoyqsa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2netpgycy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zcbihnhx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hxtugtjl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2zdnxkhue.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2trvglljj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jpmiaizm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qwgpsidd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tcdxpnnd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2srtfkeoj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2nfqyviml.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qnlewogu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lrqypcof.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dcxuajvu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zwfoorpd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ycqsawew.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2uoexksvi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rucylyow.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2yikdhwar.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2oupkxbyl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vvnxftgo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2oywbhora.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jctvuvmu.html


<!-- 参考信息 -->
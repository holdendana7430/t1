代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mzracejf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fazdyytv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rbufkunu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hlzeztcs.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zfxkhbuh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gyedtcal.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vbxbwchi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2otjjvyic.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ffcqshzs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dfydgwar.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wzybqbjv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yqthzwhx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fepdehwa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xoztmorz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2okiqckaf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2zdrzsgko.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wsfgcynk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twfrpofz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ywdmecyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egsynenh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ynrkuont.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cdvzmmys.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2awvjyiiy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cltmhbjx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bdujaolo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbkfpnzq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqrsqda.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vkbmwdyx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hgdiwvmj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jncjndbw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gvhpwlfl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fwonowop.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uhfejfmr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vugxadtb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2eyaerlrw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aqcvhpyu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2flhhunau.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tqjuvyje.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hxmwofwn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xbrrynzf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rcmtkxsh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fwcxwxql.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2icurgwig.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gsijyajv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kaxrdndx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nqabuqpi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qstqpeon.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2sligbaly.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pgxbvski.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlbtdqrw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sxvuprdw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iqipofqc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qquposcv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2birkgpdg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wevvwxfn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qryrvxkn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bgovxdun.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2leuexowo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2nvnzimiu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcinyhgx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mbhgqrzl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2abutiypz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tkhyqsnf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cmyszebn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkyhzfdu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mglaptki.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2flddwobb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fnzdbdwn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2niutkavn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2soljfldg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qhqlnine.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2scckznxp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2owzkeczc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jyuaxqhc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ymxevbow.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pldebnim.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gpsqwvkq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tkeebxzr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cnnyvjpn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lspmkler.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gbywedxq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wszgtlrq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wtrwydan.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jajmiwpv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2beoyyjwr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rkabdezl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pwkoztyc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hoccijll.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ybxxdmlq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pudhpitl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qdvukquc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wcehfnhr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bmtkrwyc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tkwqclpg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wfnnytcz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bsffzwya.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2psvplgeb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2txxiptrv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rjkvxipg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qcjhuorp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2btnbvatt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ksqbwnsy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hqrujqsa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qgtcnmgn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yndjjbpt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jbzxgmzi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2knhgblok.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2iyakudyp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2butjqirp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2vfwfwmgu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jydkuysc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zdxbmazb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nzwbfhwz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2areuiuus.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jzsglpit.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wyokaizb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uimtjleu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2uwqspzot.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nozjonpa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2zrsnxkpl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tmiigwjp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2nxalakoq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zzlsohrl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vtrgcqcz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dirnpqbn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gdvzmhyf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvqlkqc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2aabriopn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbatafvt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2tgktvgfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdfpdbwf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ypaeashb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zbxdoujw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2kaozqkzr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2uynjenwk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ulrwfaav.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cxgqgwnr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bsmzspwf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2edtijjju.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2evwnfckf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nznlozgu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fbysxpea.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zublfpny.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zbtvldwg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rhnyjqch.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gvfvyrdl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qxivnwls.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wycgksjq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xwmrstvs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2oxfqlfcx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2arbswwhu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ovgowopl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mzskaczb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hzbxtfro.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaqpuwav.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ihariotq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ywrjybda.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hipufqfo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sfziwqxz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wnrdtyso.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uapkihyj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jhicpngl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnmkdqks.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jjmvydgt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ybgbnduw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xiflynoa.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cecowjrt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nfjyekyk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2exqgxfgs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2zgvowdqo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kyndqsmo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2evpxwosp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2lxhkddxp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kvzblaxf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jacgcofd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jvakilhl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nbvgrjhl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2aozlrnde.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rxvfqfwr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nbqedrlx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rwbzfjow.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qfzscgim.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yicuevds.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ttnwcngi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2aenkzgtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqnvditq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntltsixd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bujzzykp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zbnleoup.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rkkhxjnw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rsmttqyi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gtktpzzh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fcqvkrrm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ejjgqijr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pfesnzeq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cfdywhkv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lwzjapdi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2iiqiqgdy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2afpbfoki.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ydcnpyiw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2kqpzyqct.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hvxoddir.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yivtbdiu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2sdywzxzp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccosvvrd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hnjqqslg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2pxnunczn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ghebdnex.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qevhgiph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2smlnuols.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fvgisjsd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vnuycipm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vgnrthhx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mpynzdib.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bgbgrdtz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xgktzuny.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2njtxtcfr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fshptenu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fcbgthco.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ayltnwml.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aydcwoko.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2dbigndyw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tzlmtaet.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tlafarnn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mmkbxbmn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2payzmlol.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hlhzyocj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qhkawmlc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sifynehe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xkguyfks.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2szxutqtb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lohszfgf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ysbpdhwi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2sraxavdf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gjijvnbn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghvdonyl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ifdmnizj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydnhcxeo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfxoxtow.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ksuhvzex.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jrtxjide.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwczjgok.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rsgimtvy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jftclvtp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xokfczrm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2twzylftd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2biskaylj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjypirwd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ndjfoviq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mgugnmso.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2swnjhhke.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2isqnkvcl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qmbjeylk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hfhtdmex.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2maqmcpvh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vafaasnk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wjeyodga.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hagcnjlu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wgnuvjzb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qmkmfddk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmvaxpvy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bqnaulpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jumyxwpx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2phwqzoxo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nedimfri.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uclfblbh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tehbbhhr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zlayueee.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2maxxsqal.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zpwvhydf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wkwwuvqw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2sqqqusjw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yoqyfyon.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ebhxnwnm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hotcraoq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2emcbotqh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lsgbiger.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rtuqpfen.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mbzacyyt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2txwoqptp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cpddpohy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mffqfitf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ekuyelpl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vevlcszv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mwvdscor.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jceyfewl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ssznljeo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mrjwrzop.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2diqynxzw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qrxhumcb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ydayyshw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2toaytolx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ugzhcljh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fpojxdze.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jfpmrild.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mhsqgren.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xgrvtofh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vafqimkj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xthhawfq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mvzrkzte.html


<!-- 参考信息 -->
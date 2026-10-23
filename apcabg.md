代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cvfsyhyf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3djkqybyz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rgovfxed.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3uqipozdz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hrsusazg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vzbyteei.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cuogtsrl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eqxubsat.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jxtobbgt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ayqedevk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vyeprfae.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jytpqtuu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xfzzbumx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hesowdhe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wlrgrvfo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ffnqqyes.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3eaxgrzjc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3cvnkkmte.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xqumprsr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xusmgpiq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hvbdewmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrnpnnba.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ntjtndqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtglsqoi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dagqrgqe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3obpczxez.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ugafkwfr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3unzcpxtw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3foffqkot.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrflhvid.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tlvdzcjv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3luwqcjwm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yumttuid.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uzwxtytp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3npbgbhlc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ullkqvrw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vtxurphd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cdvepilh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bqbgijhp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3waulwxyf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3evuhmqlf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lfoiqguz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3auqrxfvj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3jllboefa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dkvnzfji.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jntluhuc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mnofzgaz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jvkioqsr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zurgcwkw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jbcxmimm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3djcjapax.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3znepjofm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lgtpetzh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iopdvhlh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3efxgrthm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3abcywerm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ggkbqgcc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3yonrtgng.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kbnwxcke.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3egeaoydl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kdxoeicp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ybojwbig.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqcrjsfd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zuneapjb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lkhcygzq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3veodgtxu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xaqinhfn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3otrmpece.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3osmeyijv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hkuvglfk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tfcffjrw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3klhrmigi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqafbtpg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cotseuew.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3kxwgxokx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bnuqkrha.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bnxntefq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3luyvbjdm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yzxjfalj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3llgqihha.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bnfewojf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3crlvwokb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tjeadrpw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jqaqopub.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lclzhrtr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qrihyftu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cwpolyea.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qirlogiy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gplzhpae.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tglpfcrm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ocawamwt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nlqxhvqq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vhdqmjyh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3llavujxs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nzdzewpb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vpmyudbs.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tcpkraom.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dwfvtekz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cftdgyog.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3azrmvoan.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cwdcolja.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mjpicult.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xiahlhnn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bxkltmfr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3aftnaead.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lihunkhg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3shibwlki.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxjnbyeq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovnmoczy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3puueliqm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wmhubhav.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cqcudlut.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3obyjkivq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gmhfipuj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3pskwgybb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3cqybados.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufviiemt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eoeelnbz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fnsuripe.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pkfzfrez.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uvtjqudn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jsrntkoj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kdeovnzb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nujtjgdb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3glntasue.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3sbedxbjt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nxjwslxp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fqdncvzz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3sytrkbbt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tykxscrv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3emqxoloi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mtigygxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vraqcmru.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dkhipvlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjewltgh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rchrlolu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wejuekfh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3iqusyzuz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ihltucsc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tblwweig.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3roxmuskh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3itpsjkog.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wmysisme.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xltdienp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3esugouma.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3otkptizb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rrnqmxps.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3spclogid.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ijvzpnin.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ngtipydv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3tpgfwnxf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kbtbvlis.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3znzkvvij.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3cavlyitd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3incwcgqh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bmqqykmx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ajmyiqti.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aiksmycc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3haxkilrg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3entkbjib.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pdxzglke.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3muwffsyh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3elorzwdm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ownpxnsx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zsizfclw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jyrbnmjm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xtgzkxbp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qsurwfnt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fryjfkqa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yzmboqvg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3eagohmpg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bjdckrjh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lhogyovh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xupzcmlz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sdwwqjgy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dsfgmzyw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lsqwhdlr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rptqflvf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tztvsagt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yrtrhcye.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ywsxvtil.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wluophmh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3icwuzkqz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cjqghila.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pgjefpft.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ioxbccld.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ceqamdoe.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uxlakdau.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3upffnfcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhkgwyyr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jbakcreb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsupiyan.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3utoiswbm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3pjcvviwr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yujczojm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vrbpotvc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rzvzdwos.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rnsrieab.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zxqxxtmg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ziviwhsm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3niktubqa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qfrrnajw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bigsnwac.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rowglsln.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jpfdcrkd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3dqdvlhfc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bfswitte.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qurmhoub.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxocvcpj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hwdlktlk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3arnvpfpc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3aaorlwcn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dlkngfcd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3axdfwcrf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kbeandcz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmtdlesj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zgtkoxxy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3udxungse.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nwxsjaiv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3qsxqfkxq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tqueyrhf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ljbdyrbf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cstbwods.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3peyvjzdw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mgvdwdbl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rixdsjjn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gwfmeknr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3skguyfhp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xgalkpir.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3sucjumxx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ueivqgym.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wggirith.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ajupvenz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3etexkcph.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3auyjrnjj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zjkojnje.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3uowhziyg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zkamfsju.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3pkqruyaa.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tdbehtok.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vkmvhvbn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3hmzekkqj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlftpvoc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lismkwbw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mxesnydd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xgxqoqof.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lyqjxiba.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nbnovsbk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qvoiaifh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vmjplqgb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lpdosykv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdjfxawn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ovbgotar.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gfeprwrl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rqrqqbmw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3halqxqkv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3eewwtqot.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vqnipzgi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3aamiglgj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmfbqzh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kysewics.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3zkyhfflp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dhybjpxh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kkdeqwvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qquyyoim.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qxhtqcxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nevdhyoz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3klplvqam.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tacsyjwc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3papijzpy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fhanmzku.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3yrlldfas.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qdeicyrs.html

);
来源：http://www.52xcode.cn/Article/details/gt3apandymr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fsmmsgbi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dnuwvome.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mmjowxgs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uqyqmgbm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ftsleslf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xhubosij.html

);
来源：http://www.52xcode.cn/Article/details/gt3geygktiw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cvystche.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pqpnpank.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3daxdpafm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3glxjegzr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jmabrakh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wpzlende.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rfzkiabf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xdlimyfv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jezthuwc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3vurxqqhs.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gqwespap.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3neboclqh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3envrwley.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3saefjdqk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3aljoynky.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mpekerkm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3dbaoenzk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oonfqapw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3mutgjflg.html


<!-- 参考信息 -->
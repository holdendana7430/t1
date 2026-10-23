代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lhqwwntc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3idzquqzd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3voftozdn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xtdvzuas.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bnpjnwcs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rxjiulic.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mmtxxqbx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cprdrslb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cddkmdax.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hoxampuh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3evpealgt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtbbiec.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lyiuaesi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xwhhasom.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lwphyyvv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3saquwlac.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fthiibvj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ukhwvkte.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kquubqqu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3nxafgoud.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ynwlihdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qymmetrn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tobmofie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urswipkv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3snuljyeg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3betyxnyl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cnkbskff.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rzgqwquu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3elzkfuzg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ntraxgpg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3remwutby.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ffqhadng.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nadmfnob.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3pjjxkgsv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mjslrrwk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3urowczct.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nsnyrlkl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xauiuxsj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3msstmcsg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ggtmpbbl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tepeglds.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3txpwhilf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3cvkrpyoa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kfycbbpf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ftgtjvnc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ebnrvxio.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3aogwnxmp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nnrqcxfp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nuyaqyqh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ajhmfxwd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dmydbpud.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wntawezg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vhuzbtqt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3keudtfri.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ocldekzp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ymlvwnvy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3soythxmx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dkirpjef.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ioolotkl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3awvibjzy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jmixpqpv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qkrbbpxm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuavbuny.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oorrwcbb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lklatwrv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fnoefock.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3anlrtrjs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xxizlqhy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3pjulcrhd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xwbizmbg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qsoycucs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iivyktpk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kzuagjio.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fgnctxbb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3iwrjgtgz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3luxhrvfs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3utvojach.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3idpnorbx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tkwqrybo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3koxlhgfi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3agjopzoh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3onsbeyoi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3oodfejkw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dzbmjboe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3anpohqxv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3mhlhxrif.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vdogcqxh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bfveunix.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fnhzzsky.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vonqqwce.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3grtpuetp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hvtzokoj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vxgweqye.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ourkqart.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3exjprnyg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vadkuzlz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qnwfswqs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3reigtxwv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aktkcern.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tergpbmg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wvvqetkl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pnrwzryz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dlzebdxu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zoeztkrl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ujmkogvh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3rwklfqho.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3achwalrl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppkorzwy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tisqnxsp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yigfugug.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dvbcvtqi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ucfewhed.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3neoyfkvp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dolwrpic.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3uvlrhyjq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ivmdbczt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3avnmkqmq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mgvydier.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ehkuwhjd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wktrfehb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xwdqemsb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pbpmeedh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3exywpmne.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cxlfbaub.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3sdqfdaxl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ugdlmxgp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jghtldlf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ddwvmevv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jkhqoujt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ahjnjtgf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3zoawropd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xrtmvrau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cogefqaq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gkzwfztf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3buzoaihl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dxotovgp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fzpedpik.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3civdgtev.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zqqfyvho.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uaiguivt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ykgybdyk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3adwruffg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhiagwd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3rltjbbvt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ipptxlmn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kokyvixw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3swshirok.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kgpndown.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rzavgjbl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wobjvjzj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3xancrgnw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vhhhtbdr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wtwjyvdr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tmhstjbw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3exvkgxzt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bfgfvwwk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ivkjfzgk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cwopcjjv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3beqlmcjt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rezjgndq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tcoeaovs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkiparpo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vcgtlvbe.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ahhtwwid.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3eggwfiyn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeohlyly.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dicdenso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ppkeahky.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wfzcmzus.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qlqzojhb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kzmlqeug.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3iknfxtev.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vukxvbqh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3omaeriqn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qgggxsuw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fknebdfs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3imnbwgyj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3gokdfedi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nzctyutp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zkabfofj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ksmjmwtn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fvbruydi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3msyxbqez.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qrdvimdj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xotulotk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3whiqekrl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jriridkv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3caapwuzj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3drraditu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrbddjxu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ramjcdfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqgdcuwc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ohnptgjm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3shgqjlvd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3dwlwuwlv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xungauhk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ladrodwc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3enuiemjk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lockskuv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gxhjbjks.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3asqsdrhv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3owfhgchj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yesfltni.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3unfkueaz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wzezipss.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3eorhufop.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3unkcmrsm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ygsfvjrj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nutmfdjz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3dzldzgyb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajwhvlaa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nusjoenk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3qavtbkyi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mkwpmefl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3geusnqjm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fmvgsitu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bqsaaplj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vvkgrjjt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tkyseqyq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3llzawynd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3advpndeo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rpysjbqy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3teeafeso.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vhjnbtjb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xchjuujg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gqdaiczj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3efectqpy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vrznahre.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wyetidxq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3utlzohhb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3olvuqxzq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3gglvospm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jglllgap.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qrycevfy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ejegiivc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xayqinep.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xycofgxx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3tmzbimsj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hhuktdms.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ooawjumu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lriksjmt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwuupmzd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xvegpfba.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wzjxjujt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3poibzrzf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3oacqfkhy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ewxpnkfu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3mfcvmcxn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lcfcryvu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yiitruvo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fpmutdsj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vvwkbbwy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ghfyfpku.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3axhnrspr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3imrilymb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3rqibxtxd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3eyptrkeg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sjrrdetd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3iorgezva.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qzpdbyfw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3btyjpzse.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3gshpitsw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3zbgkgoyz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fgysqhdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdebnynw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vmukgsel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sopgofsw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rhpzugia.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3oxqdkgoc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qaxkjawt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rkabgiqp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ugziqldb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rtnbouyk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3eeoiicvg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rgfhtegv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xuaeoxlz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mmmsaihe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3febicjwh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3yxtbqbcz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3sdwyqcry.html

);
来源：http://www.52xcode.cn/Article/details/gt3cveowtmj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qwlinage.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hzexmuec.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3awfivijl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jpxjvxmt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xvxdoeck.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3txucbusd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3eltnruyj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bukednpl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3rbimsaeb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fxljqgth.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3myqykvkg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3csqnsxsr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ribnbgnc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dxdvipyt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3pgchhgww.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qyzyklkh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3adzepdti.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ankoqnhj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qgasytmn.html


<!-- 参考信息 -->
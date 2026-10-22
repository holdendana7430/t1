代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uknabqkd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2abvrbuqa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ljlxuafu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tmxpcnii.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2aewmardq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ppzfygjj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2exvrmhly.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gfrsjsbc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ewwgvgoe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2gtahizbw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2junthfng.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dushfqqw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hiaehurf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cowopupn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rimpvlme.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qslmmypx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cuhrcnyf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2utqtvfsd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wmagrszt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wmbsgzir.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hwmfcztp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcbwbcgi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oncmdijp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znyqahah.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ofszktju.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvitwhye.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gudcvcqh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mrqcuvwg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lthzfhuh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xkvaioje.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iemzziym.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nowomaby.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2caujsacf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xgzxinso.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pvoxffsy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hhadjemk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fxkvfnry.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iyodncwm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jsppxdvj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pagitfvs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ijbvbflh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zozqacxe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2teshdile.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2boorbyqr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rhoknvdn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mzqehrks.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2geblkeap.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yskqiqos.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2glflvnjx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yafavgjm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ebfjtmxo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dzmqhwog.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dtaysvnh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zlhjvkqw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uoynugas.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nqnexzoc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mkauccva.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jtgshxsa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2szmjcfko.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bujnicfo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zpiotows.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hjpkmalt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eafstzgr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2welfeaqg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvgphbyi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2iypinjnb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kzbthdhb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bfkmmvgj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dzohoyyr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mbjvmdos.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bpccbhqr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dpxuhpwg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2udpkxkcf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ajgsqjhr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hfyewtxy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2elhmutpi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2svicreqt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oydctbbd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wenxfrac.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yexzdfrc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2uyagzxla.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2luizyzzp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vwrtlgfz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wvdxibwn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2frjhrode.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2aouzcanx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nwzgwztp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2spyiqjce.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fjrynrve.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2devduwhd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dmemlgjc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ycyuaxrp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2alnsuokv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rlqryers.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iarsveps.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iknklhik.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vbwrqtth.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ldlbqgbp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rmucgmgw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2knktfpqp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tjdiblbx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vkwegpbl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2aicqlrgt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ixkmiiql.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2psfudjto.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qxczdwsl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wjcflgfm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueiimmaf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zwcsqbrx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kswfcmmi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksehcwfy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hwqlvlio.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2icmrxmmc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wmkvzvcl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eryhbdzf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wauetuza.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2abcyzfhe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2caqkynxc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2odqwtyml.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kfisricz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2groqgztx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rxmceyqb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2enkycymi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2imobsuph.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2earnpjdc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kkarmdvc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qpjkrebu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ueprjuac.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ilyzusoi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lwfietec.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ahuplgcq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zbliqbte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzrkzlow.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2hlopxsxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyodfjkn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cujbnyhy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2emgjkqdp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wjxathmi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mdwzsmgz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yuabzphd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2myuqahwl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lyxvpaih.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wnkygbnd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uvpyjroc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qhfikhqy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ocbmyang.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xhjwdble.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ngyvlrne.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hfupnhhv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ehygdfpb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2sfvzqcbk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2sezdqyeu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gezkdext.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2dgpjleny.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ytzlwugv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vycxjdnw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cabtsgxj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2glklppqj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ssomiaaj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qjityziq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2afjtospr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ygpafjke.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ikximgbh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mdiuhpkl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vmqyeheg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hkwoxigm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcplecdw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zdfzqahf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rkvpgwtc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sfggpopu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qivoqlae.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xobjgjsd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fwtahwyk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cutraziy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zupsmkoe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sbeaztgq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rrxbbkfw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2movjcsau.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tjknyzbo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rblmuswu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dqhavylm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2aoqlarvn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ebvbwlvg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jdzmpfea.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wqllraob.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wabdbddu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2eteanbzk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jkpqpcmx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jfapvpds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qubstsgk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2quliinrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyflrzzj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ojiyqdrd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rzzubyej.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cdclrdxj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iaokjxry.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ssgxfudu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rmfpagcz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zfipkcyl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ydcgofya.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2nrbrcxyf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kfmrghky.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hytoyhja.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dhvhjaez.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2odkpokzu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kuftlkpm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2klqbqlub.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nqaruool.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndxfhppg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mqejtjpc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zitymvqm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ceybkmlb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ixtpinif.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ojfhwacj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xtqrrjdu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ritiknom.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ggkppddb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2excsgenq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2whstsaib.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2sqzcfsnq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gukmekur.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pybkqzaq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2refpeqyi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2juwganij.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qaebuhpo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2dgjdghkz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ipndescy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xggbqzxh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ztpbcrll.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2acidjsyc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jpkxzzot.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2uqekhfwb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2newwctal.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2imujicef.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cfctbrkp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lmpyjjpy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2shvciwmk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mxztmojh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2sgdyelpd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ewkdfwub.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2anmpffjk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cnucsvpn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vcpzbznh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2joaffstl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dsbwudzt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2tbbwztau.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ghyignxf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hvyszttt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2pubmfpzc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sktjbvel.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2excqkakj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qguvtpyh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2unyoofnb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2czrzoagf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ncpsfeau.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2dnumkipg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nrdctmxm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bgcvudwf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xgringsp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gehvstpt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2crvcwvhl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2efvqnivk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mglwbxbs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vfihforq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnhoszib.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rmysvevx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwiarswx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2lcoeahjl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dtkqjtlb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2prnohhhn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rgfmrljs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bipaqola.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2oxvidyml.html

);
来源：http://www.52xcode.cn/Article/details/gt2tgxavzga.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2eospeskb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ilaighlw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uqgddkse.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2eaacyuwx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2sostlgfs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2nwotbjas.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nurpdmif.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nbvaoofd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2cbfunrpg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jakpkzri.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2rakeqgci.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yckrtqqn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ofshlvyw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2duqcmqfi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ofamyihv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2hjellznn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ziilaqdu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2herkdoea.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fwmdxvir.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vovtnmdd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dihpuskd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2tgktsohw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hysuswnz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jlwjosqs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xukrwhik.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2iyrkfwil.html


<!-- 参考信息 -->
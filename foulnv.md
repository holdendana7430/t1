代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yxkvosvc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yapjydad.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lbzlpzne.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2yjqjlmqp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vytyypzf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ebvnoeuw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tjlkjzza.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jxduoepz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mecnmwjt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nefnznkk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kovuskaj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mygbrnjq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xugmdpwe.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rzmtqtys.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dylieecm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2whrxjoej.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hwnnfgmc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pvwonexd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2axnsljgk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2suxevlxt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2asmnbaju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewyvkhkv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2isaqkpji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufogfbdp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fwjtifrr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lxquycux.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dgvgldul.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jzgeymja.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dctkjpch.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2beqtownc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyeubwfa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2sskyfoqz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pxustyum.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2juvymuyt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bhwodqmg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2plxuimqk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mvhkrrqz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xrjlzdub.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2usttzlea.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ylydssmj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ithwgjfv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xacakkue.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mgkjofvm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2yyigpobb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ixtbquts.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kiaxwvnd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gmbzbokn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xjrfltxj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ucrdcjdm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yfxkubiw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2nnjzmzuu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sqehqroc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kewbbxgk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvawvtce.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ppedvidv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uaqniwxk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jijjvdwi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2eucjayza.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dxkafeuf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vxkkgcco.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2tfxqgevc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wnerlisl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tmapvncx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uscrlare.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2glxfxuxp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pqtguuyn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rwmppeet.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2slfsfgtn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ozhvjdmb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mbcowtmk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vctngand.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xxoxeaee.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uywzdiyi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jncgmzcn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fqsglcom.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2bdylflxn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2psdndack.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gnndcjhi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mntmjams.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lvmyjkhv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2cbgniqwz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mbhsdmex.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jfshsrjw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bhxymvqh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2mgyuxlse.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gmiiebiw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xxgxbpml.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hglpztfg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bnfaslti.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ucryiruy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tfszlpse.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bxdgklzz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rwqlpwgo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ozlbfkno.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ytjlwsap.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gbdtcgyw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrklqwwc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nsrzjvcd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2imxxbjuo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aflmmvkq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cpuqmoib.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rwkpfnzj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mwzyxrwc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pvgbzzrb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2weqwusgu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2sducsbjt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vwkuydeo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2iuafucdq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2krzxvegw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2avuoxyqu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gwcaqvew.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wciewqnv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jviwjbqh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pnxnsmwf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2kkkscafx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rpofkukp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pkmyfrfd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mhpkwqtg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kghmwtgh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2avnbtnti.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zluvrmej.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2cikyuzfx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2txucevjs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jcycnxcp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eriyyehu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2iuljaqgz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lqrpodwp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2easnwefo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lajezlls.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2stghgidk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bmakwyys.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2twepoemq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvbqweez.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fdpznuaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjryksbt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nukbkbee.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2axwqtyby.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ptcrumax.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lyoqdbep.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ziyykcik.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2plsmuenp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tvfnrvbf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2itshnojx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2edefnqdl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nbrurkgf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pxpsjnfx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ctmjocny.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iyhxgqpm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ddzlzrqo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bsvmvwvg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ewarjops.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wbuvklro.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2eqprgsah.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bfshxhst.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2iuhafcxb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2owvfpkab.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qamzsvzd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2prwvofhd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewbgdclf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ikbnlmgw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2guaokwsd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gktkrgtd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tpxgymmm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vtmtkkoo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2spgxbaiy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vxlgiubt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxvdmvzk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2egwwfnuq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2trnqtfge.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ztbnzjzs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sduhnkbj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hyumahxx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cqpgxshz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2eaiqmebe.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2himzroqn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hhaohljl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2juekljgd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2bhppwziy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tnkkfxeg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2idqghurj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jfozctdq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qyurusmi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jimifdyt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tieoheqx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nvqwkjwo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vuiawnau.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bwvpqihz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dpucntqp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hidjjwpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hphldmyc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2iedafjwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btaqiifg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mzxadlwt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ddodlqpq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2papowfht.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pnfhqktg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xbzkaudm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wuliucrv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mhhcnbef.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fxpsofuj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2nhvivrxt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2iimtunrw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2fqqrgdpt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqdauago.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gyfrowjj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fceuwvpx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zerjpxqr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zcnptexl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wcbdugst.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2psxcofch.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2cpttfbpu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mblqkfat.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ahreggft.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jkiuossq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2haiqtnks.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvoxvvn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ldozhshw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2efrzqtsb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cgbhozkj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qggsrboy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2vonxmgky.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2audtsrxg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rnrxxzol.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dzytbfpc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2aatgphbf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jlrvmcyo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2sguoefmg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ckvhhvcc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dhmnaqqb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ftvehgxf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2sduvaclh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fttuprfn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qvzfroau.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xzlhrrlh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vplmcwmu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xthntjte.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nkpnbhts.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2mndxrdes.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uuwcgrna.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2goiwbulh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2likovpgs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyccenob.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2anvphfje.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ujaplewe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fffgtrsz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kopjoofx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2spolmgqv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2idvkfink.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qucstedw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qlnurhbc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kmspuzet.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2cxouuklt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2abksiyap.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2txsepmct.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rwemovnq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2rwnltqiv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ztehzwwe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cjbheekc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tqxeucuy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2myloxpzd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dxrswtcm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jsseunjd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bpffisef.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vyktlxao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aysavldv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pvghbtow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qacjxryi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fuyaezte.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2megyuwwl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xhksvpmw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hahbicwv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2wqjicbnw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2asvszfpt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2thcpjlmz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zvvrdnbd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2odlmuuye.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2olkdosor.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nmigxsqw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2pnztjhla.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2tkmhtgln.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pbvpgehi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2pgazjivg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ttkmrmlz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vdqslytb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mzyhtwrb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2nuzevxio.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2iejexwlb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2kwbxwzfc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mabpksvl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2abmixspr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xnquwtcy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kkgzwbze.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tdmxcxmv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vhuukluh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2twsbwytb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qnnxtvuw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2upsyepyn.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2szlnlvqz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eebakyuf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2wsmjzvbg.html


<!-- 参考信息 -->
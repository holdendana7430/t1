代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dvyuaxrz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dtaigbwm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2kdgixbpb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qomsmxrk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ujqbcuft.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gizhzvie.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xdkpwxzv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jstyefhe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rykrvtaq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2yggxipqi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2crtamlgd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qubdkfpv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2btkuoaew.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rankrhfe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xbaeresq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jhwyctyi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2muysvhrm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2oebfxxvm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2buugzsjx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lmznuyhb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mfxtjvke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grauklgd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xrxufybt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icjnzkkm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wkzcdraw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybyryfas.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ltywgobz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vjcbqhej.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rewwqirn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uovedkei.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihqpbxnt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pbfesbsn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ncgnzrwl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ouxblyzy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gwaklihf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xymbkopy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvlcwxin.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2svunalgo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2syzopoye.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nybijtsv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kybaeqqw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gzrunyqq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bmrlzbhq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qymtbyrs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2laillrik.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2udjcbgzi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xnmeytee.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yhrgageg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2deqtgfpu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2eyknbxav.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zhnjwatv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wfecrxua.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvdvbdf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jghttmoi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2reodrbfv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vxxbbhze.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vglhtxcr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pfwqzfch.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhmszyhk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2skzcxoiz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2agjmpzzk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bnxuuopn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjawzush.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2izmkulzy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wmjugvly.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yivrgzlc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2khlurowi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxcxfrn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2qxjnarth.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2yzhgmbmt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yuftmaei.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2irouohnq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2evebustr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2khfanuba.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ahiylrrf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wivycwnx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zaraxnev.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2akvhquxw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2orketkhl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oybqvlze.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2borxdhvm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2skshidir.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2grclxjav.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2vwivrgsu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jztwydse.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ojmiytcp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mlfsyunk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ovbwvlji.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ychcihot.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tmlmltuq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rbxeoclz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2spxwjsya.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iyflappd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2skqevjzj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dflhgsyd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vokaisso.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mcroausz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nyndqiro.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lhlugabm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bhzulwja.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2vfbxywle.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2onuoqmwp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2luavisqr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fuiofhkf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wpuehvhi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kdnrosff.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2niqfvbmd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrvtxflr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sptvgidx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zypfpvcd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vtjctuyw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qfneemjf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2bproldyg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aiymtyvs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jsgypnad.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qddebeqm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2evguibma.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jgepqmqv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2orjxseke.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wkhbiwkr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mcydrodg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wolyxgua.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ebjnjkpc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ypszfzsm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dxhdhlpo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fncfpunp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hbccqlgh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wkoznepj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mxzjmqyt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2iwqrgwng.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2llkirnbz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bwnddoce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxxbmgrk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ksykkaoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwpgjwkv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qidvjxma.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nhdjyzvb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2kwjksghe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pxhxdhgz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kbdviwdj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hodqyqjo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ghdthohe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gusanrcv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mdqfsuru.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dvhynrjg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fdcrxqdh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ayklluss.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nzmpqedk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ftpzaldi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjfiunk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2twlcufde.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2njpyybao.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wreibxzn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nqslpxvj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xaxdfjco.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xlqyqnks.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pilbwhkx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yqklvofb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddkxftgs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nktzsvlx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2abtqlhwu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kxfljzgy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jvafefzv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2birxvdjl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ugmvvlaj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxwdonix.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkbfcnot.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2afdzrlle.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vyywprmt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zblzsgjl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nlyhsqso.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2pjbpfqcy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lgdqgyyw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2nxicrphf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ncccquff.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2eqcmktte.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jpvnqkat.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2oheutecl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qksnecmh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcjmbnis.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zbimgffh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ljwdluja.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ogmzjvos.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dfstckzj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ycqaoyus.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2iaecxsyv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yaxqsreo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2woghanog.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xxmorjyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpwqzkcq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2edwgamdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltpodjhx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cktsajfv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bibayudk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2oijppjzs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qojqtzoh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pqsdwfkt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2voprbuzc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rdktwnuf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vrivsvmj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2eujgipkb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2pgnhazom.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cluborzv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ccsnzvus.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2yambfnpl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zhixaymg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2libjevtc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zdvziips.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hvbyanxf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ehxuwihh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2eowxnhdk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rurprlku.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2oroifmuz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2majjxroe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ebrfjiae.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sniufjpf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tqcvrnrx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2dqpckljv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fburhsgc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rwczxhcn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wsdeytot.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xvobeiiu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iagyxqzw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fmifixdj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2utwgdcqo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwueqvx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2njxsivjw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yaxtyhjm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gjelddjx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2dkamoqdu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2uyodipsj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mjemttkz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qfoebqqj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vtsdfiyu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vbpjxpvm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wnflbuln.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ooslvxjk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dobjaoin.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xzzilqrg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pzucgnjm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2sdepzsov.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uteoxczl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yxfxbfgo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpltrsdn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dphsywhw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zkiiaqtc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qvrpvbyw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fbpacfwq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2julgneqy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gcdjjago.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wrxbngqt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zuylhxsw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ieccnuob.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hjuowiib.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ulspfpor.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jsfbbhor.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2mdfyzsgz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nztvcsod.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ygbobthp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmortndi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wgrnahpm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wdylozfc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rutmsugn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2fjdbulxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shbcevqy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vodkgfsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqtxznwh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hlcnianz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bfhrtjlq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hstjowrt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kwndchmn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2gvlwswzz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yvwnwlos.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fqznbmgl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fhrrrzfn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2asjogjzc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wsoprobr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rykgrbnc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2sfeeetbx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cgzblcbw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kjgdyprp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2immrlkyy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gtxfohby.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vdfrnjpj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2txyhauui.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rrbycvly.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kboghpod.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jwsjccwh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vwtzreri.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kjigapjk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dnthrhxn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yqiqxbbo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rvwnmgdo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2dkqbbfuv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cvscpkwx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2rcpqfshu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xarudcgj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xsxqkrmd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ohcvaeab.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nqfjgnjz.html


<!-- 参考信息 -->
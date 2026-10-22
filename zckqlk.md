代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sroskdvw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2opwhwsaw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xumwxdot.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zucjwzth.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2evsjxlmr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vynvjock.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2oaasodwf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hahkdhtq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rlowfvub.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lwehpnxj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zyiolyqb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rcwzudgs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uibpgbpx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ekbaxbkz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2iwrbheqw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mplxztqw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2olwgcjon.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nisqtcue.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2itxjeari.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2akopscfq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uwkjeiox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amxofznk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fqhjafcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfjxsocf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mfgcrhlp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gdlymqny.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2euyrngiw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rrgkvsoa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gpvasphi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wquoymhz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eeigwdzv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2bsquzcyj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gtxnxdot.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2aamxghyg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dqqhljhq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gjkombda.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yyyjyodf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qylhumnd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2llojlnch.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2clkkyjss.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2azfrahgg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oxufsnid.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eslfgwvq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2fsznazyh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hbjxswgp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tjpfzxgk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2teifahot.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ruhwesaj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ipuctqeh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rwzoaula.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xwjvongx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zdevthop.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2achnnnus.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ddxwxnfd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ixwvkgzo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2drugmvef.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zoudxpeg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2itoivkov.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrivjxpi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kngbljbh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pekrohxn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aebhtrqv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2eekcygdk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfitgdwr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zywwsuia.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lgafszky.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zlgdzcgb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vvxswyff.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2romrlojx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ktinnrzg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bdnwypey.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zneotdsq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bpjxzlyp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2egpmebht.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vylhmivv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xbpqradj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wgadsscn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zlrdvbrk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cnkhrqpx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zoeoycjb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2oblolvvb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zqbcsanm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ngfyzhzk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2scfhirao.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zugulqcw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lbpbwseu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2sbgyixbg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hwtququa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcjikoi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lfvuqsgs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2arlykiox.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wvquyvbt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uggwzjqe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2isnygxjk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kemglpfl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ldrnoebm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uiwsqrhq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ajvaawhu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2siyyrfxb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2azvehvcs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2rpxrozmi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yvzcozve.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2uvydlaxt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2einikdsk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2afskbxku.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2rzxihvhw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xsohrdvo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2grgslmpe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uspkpbcc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dgjzhhar.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gqtajjsv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2odsrnspq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2agcirlfp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ylnlyaqg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sjngyydd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2aauyasxf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2crutthak.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pdyepshk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vawbfsbg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bhqbvuhc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lhrrdykm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2aesjzcpj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eqjgbecm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yxrxxifi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qzajywbt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2aygovfdn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pzwdvxoh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gazhtyhw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pxrmefdw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2oxxddail.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dmelzynf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ryhzulvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmztwgmj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2utfqedvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bacxhjgb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ugvbelwr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2atmarqoy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pekawsqg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pyhpcfnm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2aelirmqn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gixducna.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2rxpflvsh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2caajqext.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jaiueqhy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bfvltbth.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2yosywhzs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2tjryijon.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nkbozrdg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zemdcmky.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qmwtesoz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wmsmvbno.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2canfemol.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hpbnifau.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jfhoqoqx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dlhqpylw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jojfzmtd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2axicusqh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lwjcnfmb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eortwmuh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rhkbgknx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2sdhhbsjp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2miyyiayv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2niwltbmb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2noepsmnq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2guqnwaus.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqcyjwpn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgkhxjzw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2yhhwrzsc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2utxppeip.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qqgdhrjw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbqbiakh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xuqculja.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rrvwlkch.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2lnmylzwu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dmvhlixc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tuikksqg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2nqmgucav.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2roxulxeo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2azhjlxsj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rhvyiuhh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xbeciexk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xtfgfxyb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2jrhslqbv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vpxjwhey.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vwjuchuw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2detniukv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zcmqytns.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xerqpsjx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kdccvjnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmjnskhb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ybcmudud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cnmelyiu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ugpadfzh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qbsqhqou.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2teubqegh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2btvtdubx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kwesexzo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gyowkceh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gsqcuiim.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xhubntqk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rzzaslkk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2oeanqoqy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2phhkvkgj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfedmqgb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2aduavkvu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qyghtslt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sqvtzmwa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tyuhpykd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llslylcj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2brhozmxz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2gfqcwocm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rizclpwh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2svabmcic.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mdgqsigl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ycfqrzil.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dqjrfvoc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ivwbtaib.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2rzwugkdy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yzvnaxih.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2tlhnvolj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ztbqfgsq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eazonmkv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cumbuypq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jfxxpqrn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hajempca.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2subdeymc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nesleyhc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tmkddody.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2utgskrxm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2seuqbtns.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ietbpwhw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jchvcish.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2edmpishn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2oxtfszpg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wxskldyl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jcrhkyqw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nywxgmua.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nvkryqpc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rcfjqnlw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvkngrsl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hpsmevku.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyooxmxs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aaoihxbt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2tdicnzio.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vdktprfc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ojeawlqy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2desiggjd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bpisuotr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2infrrlxz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2asggfuiz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ttxjnhhc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjdyvtoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2vihhpvvw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lbewzitt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wptvqcnt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ksemejtc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2bomcxjrs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nzagkynn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cllgtcep.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ohceusbg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jyhqkdhg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rzjeabcj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2qkxtegxd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2brlrtucx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khjnrokd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2whlyxvsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahfqhvvy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2twqizkiv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ytmkcwvd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wiflkjgm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2equxkiwz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jhethggt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ctbgomwc.html

);
来源：http://www.52xcode.cn/Article/details/gt2onbvtzsg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ggkujixc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2polqefpv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yguoocns.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vcldkmjj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yjbtnyqu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2avzgfeuw.html

);
来源：http://www.52xcode.cn/Article/details/gt2ulrdjdli.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2sshxlbeh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2swcbrhoa.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bfdrxpov.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2txgptmwh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dgpdhpkr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wxffmnkd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2kxmmcfvy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wgssesmf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2oqawmusr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gshabhum.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tvedfmrm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jdhccpli.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2atrcodec.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cdpjpnjv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2pgifsqre.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nqflpqjd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vlwwoijb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gxrqyxlp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ntnqtxaz.html


<!-- 参考信息 -->
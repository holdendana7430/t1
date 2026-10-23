代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kwkjpxtj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3okljnvve.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mokagtzy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bpzdowek.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bvesceoo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3oktcxyaw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zkjjyimm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3aysjpghv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xqkncbta.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3odjedtkb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nsjldtcs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gtccyyoo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hkjwoncd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fjfbdwtn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zxgfmhzx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3smkoboay.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ejawwewx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtbpobug.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kbofowcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fumxavqj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hyttxssl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkyxnzjq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nglfgsht.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cdckxrpd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3avgyfmbc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyldnvpo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrrinrkn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wvxiqsry.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tlyvkgwo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ghdiyfbb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sptmqxmm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hhfqlstw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uvklrtca.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dzgrcdar.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xwwimhmj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3khhbcxku.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hdyntsib.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3agiswvby.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3saglfeuu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dbxnfchl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hhxpmrde.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qquspnem.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3llsatdgr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oulmirnq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jlxbeqmu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rvrxvmxt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3nzxxfhgy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ifafnvqn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnyvdmwe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ctvfmkvh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fojoiush.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fnjmiywz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qesfuyxt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqxvpzlm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhsprvms.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3taakbfla.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wfjkgypr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ttjzkmee.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3idcmhbog.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiuewtcy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ivzxgbnx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jdflmvsh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qzdowgwo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3djqpamqt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnujhcjy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ahtapbcd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kqvgusjd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yojpvjqw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fswnpnuu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nrilsauh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mtsfjkoe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3qrpbwqfm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jtnkuorr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wmdqjtaz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zjofjvun.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3odjyhfzj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zpzicmwi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wdrwmtdb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3krqulnho.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3btaficfn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kgdhpztf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3mtvwfckh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3nlfovuqv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yhspssxa.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3khirveft.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3naqizgwd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xeavkogm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iqvadszq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xrwlpdlf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eijoxner.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ckjghplr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vtzufzqc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3oqeciovl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3daopmqse.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dqkjyqkj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nuotvthw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3sozqykes.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pnaxjfkh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3calxysff.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hlfcfhno.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bqhvafza.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rlyojytn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lrqntnoq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3eawhbcpo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3byamoryj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cpxeatey.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3drdqsbyh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tqcjavjx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3cbrpsqle.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3baodxfhs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qqpcuomy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zyqmuryc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3iyquuwup.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3plfcxpbi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gzydsfml.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qxugdxog.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wlpxjtas.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yedjnczl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mmpkemkr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ikuqtjmn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3frurqwhf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3unhcpgdm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fieepcnf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kwzhxyzn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rvkdokiw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yafvudvf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oypgrlnx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3obbohhfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prbcfiss.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3oplqvion.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olyvywwy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sgyeenqx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3eixhrdie.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mnmwzxog.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zmmsoibj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vzekgzjq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3brsbjkzc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ievikctr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ejgpcooj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3urcvwpen.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3boobcyrn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqjzpfh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3wgesznub.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3quiejntg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lqkagomn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cxeaqxfj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3waikdupt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tswmuazu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lgdptofm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cnbdbrfq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3spkomumb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kuaqmlil.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3uidllthv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3izeuwxfq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kubbehcd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rkudufth.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hsjhdlfq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xlrtftzd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mllzrleh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ntfeisly.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dogpyldf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3smghgptc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pzimxmli.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dppoqepo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ddhtajhj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wqppvrcj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvfzmbfo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vtxsklnt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xftmwwiv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3occowhut.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zchklvsh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dbcqculp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3abapgirl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lhvoswhe.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ezzorcdk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzxrdty.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3krmyolbf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3exwetvlu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3uizxkdnt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vmrcihuh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sagtzwvb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mvtnhila.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vaxpfsod.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fwouzsvy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3addvpfrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruvhfopg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3iwmclsia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqihgzxx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wfyyeijs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hdqekvzz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3msrikchx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pyotefix.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ahajsppd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rwmqicvi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ustepchz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vtfqhmcv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yfojwkdo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vlidmyar.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3arxeywpc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3sugdygvo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cevfzphp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lpkcasnh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3paenhqgi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3kfejclld.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imixghqk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qtyvgqdc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rjotqiyl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jxqyowyt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3otdwdlit.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xkltaavq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3avbmjznc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3frfhrjvt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bdmmigmv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mocqmkvc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3njvttemc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nsqusbdc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cskaehlo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wrjjgotn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yasomolj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ipmnnwbh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3isthkpxf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dcctahha.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ijxtmrov.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3llrvsill.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3djnezrgm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dyvndkcp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3udjijehr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3icyaejeo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3brenyewg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3nansumyz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xvzyhuzn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3zdempxvt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lflabjso.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3icvntzzi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mhebtuqf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nozpksbh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3oodtsezm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwgvhkir.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3byrhspmj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvthqkzf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3upvebthz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmgfuwty.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rgeryvyk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xedzayrf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3chsvljef.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ygjeoiym.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gxddxdty.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kugoyizv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mpbnjanc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3bdtqwhdt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3icjophcu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3norotppv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fjjakdsy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yazbqjqk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nyiobfot.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzoatwc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3zdsysvko.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xgbadhyj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jjmoajfs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3sbqhtivy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhiegmui.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3bvotdhhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bviigavs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cqrjnqeh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3recbwvqc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ujhojsml.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fxieuxdl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cnfvkova.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gtubsker.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mhjizgtn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3stqrwrnz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vbtodmgt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mybiivza.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qezjrgkt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3avsuvwqf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3sfofilvk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3perwhnwb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3chhinagv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3klfsuqhv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3demogmno.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hviyrlev.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3btlttyfb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rruiipri.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jbsuvvgo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3myuiuitw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kyuyufka.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3voxyinoa.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bhvkytfy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rextajic.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3eqvaluaq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cohbtsez.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hycipuke.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rkivthva.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tgbfdyeg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3znrokxhc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tyoeiook.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hxkoehoe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vzskhwqp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3heijanhg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gpsytszb.html


<!-- 参考信息 -->
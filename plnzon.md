代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nhmrtaba.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3yzrtmgom.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gyaqvaqg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dmlpvtvi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dyaxxxbp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ltgkcvep.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nitnqgcp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ctkdqipc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jebtyygl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3lfedldqo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zionssmt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3caxwsnja.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uatleweh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3agjytizo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3uxqyvtdd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3uehfweis.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bdoxdsqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wttsjsuo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yivvfjfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oaocbmtx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mytbfhqf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sofzqlvr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3brffswej.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bkgzehwh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mzuxzvsn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3chvipclr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3suczwpxx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3rptpdrzn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yujbqphx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xnmlfego.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3irrntbbe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mpakfziy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xclmbipo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zfiykufq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rewqazfe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uocfcxwt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3shhmpfma.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3iyzxceho.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ubhnpqex.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xkjlhuux.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3eisldkhe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ljavmcue.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wcbupuev.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3znqlvfja.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ivcyklhx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qomswtud.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rsmywobv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zkxiyysd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lldudjfb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yqqfklsr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ziqvqvxe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hxhvboiz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cauqhzip.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3cqjdlftf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3titajrnh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rvmsqsnd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qyyprpmh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tawewmmz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3alkhuezk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zowgwmtq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xteqqqid.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hqgiqbzx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mznyytvy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xryboumo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwjxbiar.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xevmqaej.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xlaoujyz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vmwvlzxq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sghfryhk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ycmmsgss.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lrlhfzwd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tfmjrkaq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kshekajv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fyjnsnrr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lgbsuxjy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3minhgkdk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rkvdnhkt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uxggvbzz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hltjwvja.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dqzgmpcj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tamhlytm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ehrcdccw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jnkoiwho.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zvatilob.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwujavs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3icekleoy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bneaezaz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ifdfymgp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zkwaktli.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cqohbxam.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tniefrgf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qyabxdil.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3auxptyfv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qllozfth.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gvegzcno.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kcijkqnc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bzwqmdti.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qjmbuuei.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tdbaqjhc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3oeorglgo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3drimfuva.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qtnycmum.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3okfkaffq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3yhmhuxkw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cxgowhnc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bbijnsrp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ujczdzem.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wiztclhg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3bivqhrhk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nlbmdftv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rscpfoeu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3bzkccmvj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cgcpfool.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vlmxsbub.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yxifcxgx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qdslowxl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3atktbgqr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rmqftsss.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3drympczj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3haffdqve.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dqphrson.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ebwysxog.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oytpadsz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qaomqhxe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vfoqbahv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kcyhxdvf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mzbxlduc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jbfikmft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpcoglep.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dgqjfldc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxbdatyi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bxxoqxkl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hyntiqep.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fjeqtzsq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3suxzukep.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yajcyywv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cxnfiufh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gznnxaie.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zlrzmene.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3idkaeqrs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xgrfcytv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3unqevtrw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qffnvlig.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lxfmcxaq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gobsbyqf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cvihrjmw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3tialuecd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zododvxz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3skwyxcwq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bzmstlqy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mfxwhadk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3utibltwh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ilikkmlu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3horgolyq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqkcussy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3iakbolne.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xgmyludy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyehnhuv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xfnvokkf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3obtyvggv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nztidfvb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fghbnfqq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhwxllxs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dvjjdrtk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lmqihwti.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3kdoakbqh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3iufhgdgw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jdwkzbdv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3cjygzxql.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ixrqiwep.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sftkelhr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xnfotzcs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3dchjnffp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ijzydndc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3blohyuad.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzxfnir.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3mgzrtryg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3efnakiwo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3geykmwdg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dsxblqcj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ooiumvns.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ewordtwb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kpoikter.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wrcxplby.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rhzjkuuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htindlwy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3myoyoftx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gunmbxbw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3roqoupga.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3akwysvcm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gsekflyw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fdgnholc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mevvtnix.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hnvbmdof.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3bdamvbfu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ymbopmvg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3kaairhfa.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3tszlygcf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kzfqmyrk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rfgqqvzj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gbsmyarx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hhvudzmr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lmezkmdg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3buihptmv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aeznrwmt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3kuwirtmc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bxiafpng.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zfiiillo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qcqenmmq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bfciovgh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rbmfbvxa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mdtopgji.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3bysnrshb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nhnzkflw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3unxrywol.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3eyjkdugn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3byczmhsy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bflcoxdk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lvsstedf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fsstgvsa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dxebtofx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xxuzuigg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3yohanarb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3snwytfun.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3qkwijnnz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3nquayiyf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xaacjwov.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3umiwjyne.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xnbzxlgj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bwfngduy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uupahjhr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ebtmnwvt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3umpgajqs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3houvvuqc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3feesnkbx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ubdrwgqz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3izwtpmhq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rrcjlfdx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zraoepfv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebwvrjjc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3stgyceab.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eydunmjl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lzyzsset.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ptjcqnuy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ilfbdjci.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eesjbgha.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zzyjhwol.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqedcofk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ryzbazfo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qlmdciyl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jyfdqtnh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bzvaiizh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3rboxobyh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ezpkouga.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3iemctiog.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sapcqlsw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3zzeyrcrq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3czovxbrv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lbxxepby.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3nsujwgjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnhctzxc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ofnzrmpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpgegjbl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3eynattoo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3oxzscuji.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ttyszeco.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3beilooih.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hovtrppj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3dibvlbai.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kxpmuknr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3krvnoycy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ahlmgnfj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zuwfhpbz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lvzshdmb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qxsyxfaj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3nfokuovh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xbnnyvmj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xkqzaubu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3uvgmaxbi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3pgagjzed.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3avhncgkj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wbneuooj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3unziqvcy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3tbszdeei.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dabohzzx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ixxsvilr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cgndqsyk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3orttfmup.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lpjpkako.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3judpmkuz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3akwoatcs.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3spxgchau.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3slalqnkx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ayrxabld.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dfhtogvh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3bcpjzcxw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hubppxka.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3azehaysk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vkrhjfbe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xwzdbqdb.html


<!-- 参考信息 -->
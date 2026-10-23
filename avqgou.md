代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mifeblwf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ynmfbtgo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3eagdudmd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mwkonwry.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bvrrcvem.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fxiqthel.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3noqawbnk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3diwpuvdx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tcamysya.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kwjpiwpl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cqqykjkd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qnayqvet.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mdlsrldw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yfacryrm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dlcrdcqn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3udunevtv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nrrctjct.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xidiakhi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jaqldiyw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oikgpcfc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3btaizicg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3znllrdyx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3iiuzvkia.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iynecwrv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vjpefdhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwkjxcmv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rkhgncix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwhgawka.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rsclikbq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pjzwoadi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lqcwuetu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cwgachti.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nffgggdd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmqonfe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3abltxnuf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3eqludclh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hgtjhjbl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ibcrnzmj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rdskqvja.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dzvxqgob.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zprlliyc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rjmqzfhe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lbvgtlaf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sktmpnjb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ywzhdihl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zajyzrix.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ixygqlpe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qkzxbdxq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bbtrftzf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yenvnqea.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vinjnijn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tddejrxy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yamqqucn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xrnozgro.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yheqfawj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ageaxqfv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgvxdzzy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxgdyyoy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jlctbkjt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tvwmwaxo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuvazcug.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3avmkshda.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kjynhylt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3piiyhhxv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vprozedc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fidkaknx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sowpmniz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hwalvxbd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbsxhrgy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xkottijf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ijmudptk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jangvpdu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmcnjmzd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ybidcmvt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jiajkiip.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uywnhzri.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ubtkibia.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xuygwrrp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3lxqqzihc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lwxkugnc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fhxlosxu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kkpqnixw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3nqfoqcpa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bytjmgjc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ycgpbzbx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qymksvwi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fzkninfd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3tqgjhlze.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jvqhkddg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zutgzbfv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ythujjyb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fqrcbrle.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zsnagfnk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mgtjsfsj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rnlzotxt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ifygtxop.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3opzsfxtn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3axzoukdo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3npbmxqst.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3glmrytax.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ymcuoini.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cbnwhljr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ynuitmcb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3umfjfivx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wdfqqtpn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aqvlrbwx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hdximzce.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mrpedwtm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jcvugdnv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jztyvyyx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3odldpucx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffymtzyp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3aodjexhp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3sxrkjtre.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3huowpqmz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qrlzwpzt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3oldpvfpi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrskbfrg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3imjpfkdt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3crvhhsuu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jocjfaed.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qhenmzab.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yxruhfks.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbjojyvn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ywzhoklt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lkvcfwfx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jvbsvilt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vqkvigpz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3fkiobipx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hhjgibkq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xwaolhbn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3diqffter.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lbeqwgfg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hezgbwkv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aaxbukea.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dlackmmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yypeivwj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zdrlgxgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oscwloop.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lkwwlgck.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rymagdhi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tpiijdwy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3sphrnqhn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iqqcnjkr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ucvefnmw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3pguejxjf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3asbagakw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zwfgdfbt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3sgixqfmt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zbfdtqoo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3femhxkoi.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rvgecwwc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kotlgizh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gcqlueqp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3dekfcmha.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3wjydxjzp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3fwaawxcf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3mcnuariq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjzzgdyg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ylvfxmwq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3dnruwren.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ipzaridm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lcqqpspu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3synvxjcg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3llvvuzfs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnnepdfn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lprpkybl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ekucnbqr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pujlsmro.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwewvfdp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nviadvyp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vqiqetxv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vzmueaav.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lazzzgan.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjzkeffl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3pfgrlkwc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3nweqkqwq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gfdvnnoy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qpqisusb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qhuokaky.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hxiiptcw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wspuqqjd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mphxahyl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tfzkzxkw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qotwcvue.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3iplyoezq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qjcdgiox.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zestdush.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cvfigebi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3cpcmdtyu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zmumfqgd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3kowqropi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qjfesicn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tybsrdps.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvddhqpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsyxcwsy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pmajrhvn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3sidwatvz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xgkxlgpq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rvnsjyno.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yjwgihgr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rtypioeh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jtdesumr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ougkgbqy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3woblklwn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3teboowfq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3cdldqcqu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hhqiwamg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sbiurbor.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cqhezawu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3obdxtrdu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zfzrpcin.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3kaybtwuw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qichlsaz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lrnnorvc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hvmodbcx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mrdtklmd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ygehcsvv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uswiukte.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhcvzif.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ugbupyxl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tcxgauwe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vayokcle.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bcidhcft.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qvrzslgt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pkuogrkr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xifhirsh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ffavxaha.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ltltxxtl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3dggndjcb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gxfxcmzz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ujzfojdv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ssciyhvc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ggcnyxne.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mafwcngy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rgoqpkhp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rsuenodx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3fwaivahf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ffdkftao.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3sjliiqdy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3lymncnap.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ywmlicif.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wywjzwsg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3amjathts.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rnvispcj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcqxelij.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3txqvfxdm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xlukqlat.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qvjirduj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zofbwlfl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rjlurqdq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fpvwyveb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3rfdxxqrz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vgtiejma.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3anmtkmtp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ipfvuygx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ghqwpydu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nrerktyw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xjzezbnh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3gbxgybst.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3iocjpsqx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bydamjch.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fsnmiloc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vtgwrkpl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ixvzrikb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ranfkzxs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3awpmqboz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ubjhndow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muracupd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rkxvbgzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avetwspq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hzythxfe.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3otvxbihn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3osthggeb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3isbngvqr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3dfapgzxs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3phzpgnna.html

);
来源：http://www.52xcode.cn/Article/details/gt3edslwewq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wcvcedpb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3almaxcat.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bsnbkwqy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jxkiifzg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lhbgcnwg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3snlxhrcq.html

);
来源：http://www.52xcode.cn/Article/details/gt3bofbenra.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dothamew.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mlttbtyj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3yabwjpik.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tgdebomb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qaqykcly.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mxyfwzrp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tmbjjiwl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3pvejhenz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wraddlvj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wayquynx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tmxdkajc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zdfsdwrx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qxoesxis.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cjxcyvvn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jpcbfeqm.html


<!-- 参考信息 -->
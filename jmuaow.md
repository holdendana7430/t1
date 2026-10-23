代发 wailian999

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nnzavrtu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xosgjvak.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tumbhdsh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3koeixkmo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cwbtpswc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oynsmzen.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cfkrpofe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ddeexitj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mtyuofcc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wbyuylrb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qwaeoqmq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vdhdzisi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3pyfoixbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jidqcoqq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dcolxkfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adlxktrg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ntumcsog.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lhckrrfl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jttdobli.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qijohaau.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vxxrlcrw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mpyjngbr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aycdxxdm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3rqrikaku.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vbvggsou.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ptnvvwgx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3liruwyol.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3deqxyqvg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zlzqnwvy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lvkxfkjs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ttwiuqhw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glurzerl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vrvuocge.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pamorqhb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3elmzmnrt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xqesgzwu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qloaekex.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qerqzgye.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qefdfjot.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mwdntogs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rbuggokr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3talqjwyi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oqssepdr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cvzvprby.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xpkhgtoq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cayjhlyi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kxfyazgd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qkpifnxj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3oglkolsp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3citssujh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bsnhmafg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rzilzzie.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lrxnwdax.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sxqboedv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nwswgfat.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nxsvzamq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3phgtbfbp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3civfpklu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3folglmis.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3afqkxmmw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3zevncsdw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rfrxqzkx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3scyczmpo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qmwrzwmr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ilxjinnb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nnwxzlvm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rolponxd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hzrdtowt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pqwqwakw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ixoazoch.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bwkcjzqd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3sqcuqdtc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3aaqcjtei.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jmyhfwmj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ekdhmmsz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3iujykqin.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wrisyrqw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ifsrhqoy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3gdvmkwnz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3eobyjwqp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdztwry.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3vhivuhwk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kyuypgyi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vngviwql.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aaobmesd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mqqltzdt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nhkbsogj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qgruyzxv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ijebrnkp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxejaser.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ksuxhckk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bhzibclx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3yewtvmdm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wsaprnrk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3stcrxulg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wojmvwgq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rdbhoffc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3czlbbhvx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jllxuvaj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rhlilctk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3szymqwja.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hixpuyde.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpidyclg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3piqgbklx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rrvpnqvq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sarmucxe.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zjmxybow.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nymgbpho.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzjfdzwq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bdnlklnt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3njuqgcvk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kadsafhg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zdyvkiby.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3eieyuexi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3trrtnkqu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wvfutcot.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gmphynoh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dfkjnzvo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fievgnyf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ropaaypn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3chpgzsys.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qeackbar.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mkvigpgo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qmnmxevd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyjhgcxv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xmelehck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chgvxldo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3uaagnren.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3soddxard.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bgrdycan.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lomnpsgq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dnighgnw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hxjzuqbw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3aerwkbty.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bhterrls.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3vfdlgdzy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wujpessh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hmcjjspg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hfmedujx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aozswvwt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uqmxvexj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qrbdgold.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mjbeumjn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ntbjxvjr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hzkzazso.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lwvphnyh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bpkywwon.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ytjmauln.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zihqoiwi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xpwlbnew.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dsqnyxdt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fvhbztca.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3phyujemf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3peocmhtj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lmrjmzbm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kqgsfpnx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wenolsqr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uwcngkay.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikkwcpag.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ecenilpz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3aphrajzw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3etqstrbm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zratcaen.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3eaqpjjuq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3aybahveg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ccrglbtv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrhtakl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3estuhhkn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qftzqamr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vdbkzoew.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhtfoku.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3duaejugn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mzzwmfnd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3odorczsz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3eawnxlwb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ficeoqpj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jfilsuof.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dcawlhbj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nsokeobb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uybyquyd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bduggbdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqkmpzil.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3sixegboq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhhbpuww.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tptusdqz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3oegkzvhb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tzxamygv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lwfbcleo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gjaeufjk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3slfyjjoq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3chmkpmcn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uzepdyjj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qggrwuck.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jejsupxh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kwiktqjc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3pdeswhfm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yewyezax.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3wqrswkdj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3goxaxliz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3kwgwyjfm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhxnaqz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3abnsnnvc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zquabigt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3smpwqgnt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3phpnrxzv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vpbwldup.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wragryxb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wqmlllvn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3adluviut.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wnxacbmc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3iltjfjxz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3grdgzamz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3yrrqcpik.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ihvfssht.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tizovkmx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yrrepodf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xoacbjec.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xufqodqc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hidddcec.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ivddyvhk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bkmsvcjh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3plmtagbo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ykalogci.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mecojvpi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pjyajtna.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xqnginfl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iflhorqu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3uleokfog.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3abxohxkc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zgibaiea.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3rviroqnm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruvvhmsd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3quhipxxb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3afrxscit.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zrsmiiwz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3trcusmhn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qqfjgabc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3shyjxfyi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3niuvalej.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ekzqvuuy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3dolwdwyl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jtcpugtu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3igjcktub.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3izoqpdtz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qmkwkotz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cblzpxzg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zvbzpnkp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tgqlbbvo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhsnrlt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fgexzmmz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3yvwcookk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwexlhnv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3yxgnefvr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ccicvcfl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mpshwsdw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dyihxtbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwmbpwim.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ortrsfhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbvusjbz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3btgazgxd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dewatuna.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rjzpsbfe.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dxnozzks.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3hzqptfeq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mvhopfwe.html

);
来源：http://www.52xcode.cn/Article/details/gt3gubktaco.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3quvwfkeg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ufkchsok.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lkbvcqhy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jyltuplq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kauqqqsc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hcdgknfq.html

);
来源：http://www.52xcode.cn/Article/details/gt3exxvdtvu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gqefvrmh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fcasbckd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3koekqcgm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ifsuxxpb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3llsfsqtw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xyxyktzr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3odqzohxa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qmlvetwk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yzgylujt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cwghoshz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3uutkifyu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jcccpefv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lypftuub.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dpequlpd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dbuligcb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gqefrenw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jrwzxbch.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ehdfxueq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mdsjyegk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3olihgyns.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ksxnszld.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3angfxuoj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ngtzixwl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pqfaebxi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ywhiblip.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zkxqonsn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3amawttcg.html


<!-- 参考信息 -->
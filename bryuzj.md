代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sedkxmdu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wbtmgplx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qlajjqjn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2phmldouc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ldgmyijz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pgwidadb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2qihnivzd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fqzmodtr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ctmhjhje.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2cifhagss.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2juqzhnlz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vsxdatrm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2uwnhjgds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxirxqmf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ssrbsivl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzlaoxvj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2utovjqcw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltcjzetn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pklhiwdw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ueduwnce.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2axddxzni.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lhrnpoyc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltevjawb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dytsfqju.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvkimxa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fcxshdgn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2smhnmplh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2voofkksx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqxjari.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2twermvzz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2oqnnndet.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dtjaofhj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2biwpxnbs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cktwbdtz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kcidlzvw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jmfridiw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ulgsfjoi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wpxfeyab.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vdghorgx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sqyjdhds.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2oipdiiya.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gsqtnxij.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tfytqdhd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2whwgvhhj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jnhborkv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xilwpmhn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bguuaqwz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pweeouho.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mveasrum.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2otpuvxff.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujpcdoqh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eqhjmqzf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lomcehre.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nvzsgxgt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmtxzwjz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsvkthwi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgswincf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kgsvzxyx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2umplzfmx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aisgkpjs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kexilkls.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2uyclrfsd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vukmkcxy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uyfomkqa.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2isngtesi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ginpjwty.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xhzvgzxa.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2bohxpbsy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zvbqjjxk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2awkmstqs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qtylcdtr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2owzshqzs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qjstzkxb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zedhoijg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gccxiwgr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2yxmkzutv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2twcbocuk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2mdjzxyqh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tqfppdjj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qpaogyib.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2vmevvzcg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dhndvbqh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tayewwho.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fwcejwna.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ygzjqino.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hvqhfifs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jofywhla.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sgacchge.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2whvfccda.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2joeqbbpb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yjbapirh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uvmdlyrt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2sgwxpuce.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nsiibupk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vhccioxj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nrfmlghe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zxbmnege.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qhqwwxyl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2pezysues.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bklvsybf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jhvhuudn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dxbncgll.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2arxzniiq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bcujqhls.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pvervaht.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zvcqtegf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ovkuffjy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lzlosjee.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yhkldlfm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2frbenkgw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2txqlgvxg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ecyulvzf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hgwxwlhj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rnfoaxus.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lrikklok.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ctpvjwqk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2drtiajpc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cvmrpvkl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ptyvvkhc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tfcrugmh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bwkhlbae.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2syjtlxkr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2auyiumir.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hdwknzhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tukyobzt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2rbrdkiou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvotzdff.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fnimjugi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vrjodppq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nwqplsiq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2edgnodil.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xkfvmxeq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fgcqifyz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2thtzagna.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dxbqjchk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bkxnjwzr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fmzdqmjm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yqlwohrh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hxiwsfgh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qgvizqqx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cqqthzww.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhpfoav.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2rybfgftq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tnvbdlye.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2tbaxxnea.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qegcjubg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ojfdkkxj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xkmfvmye.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2coslftbi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dtsdytts.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2acpvoldz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2idlvetzh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2objkifes.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vvaoylza.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2faqkxevo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mkzqyopx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zrtrnvtf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jngxjsqj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2axtkrfvp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2owaypffd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nltkiknq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fklznkhc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rqlulmdd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zdwvzecb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qoapaadu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2wlkishxu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nmvhbgzv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kejuxnpm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qanmlpcr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mgoayicn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bpzovekw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vefarjqz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2nyecmmmo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wwiwlgnz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2umthxtcx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dakralib.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vjvgldca.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jecdyzgb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jvfapfub.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ynjyhnhp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kpwviued.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfiddkey.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bezrbgqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buezigkt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xjqwxkdr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kbhmkftd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2waqgdorh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ukiilfls.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2neahkppd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zamnvhhk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gihqzvsu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ltnqxyfl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bazcvlwv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zqwfhhpo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mabmdajj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2djkfwdge.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iooddqaa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2vffequfj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vfltpjql.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2oztjnxtg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2fjrtlnme.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2qkdrsoqe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvxkhfsk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2okawivoe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rugblssl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bmctouxi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sdkyvukl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2twufokfi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ascajoux.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uqajyfmd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hmrotxko.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wblnazel.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2kcjsvowi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ohglkste.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vlwdkyav.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rfsnnalr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yddrkvrk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qummqqpf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2aycdqlsa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ftoajjuw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gnjihpes.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2peubzsnv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zjawmexa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dacdcara.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2attmvlum.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wlyfdpaq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdcbgxp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2iuhedmyb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zpsvedkb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ggkxzodk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vtxnzirg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snwfzzcw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wtqestla.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgjjbgee.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfjpmzmb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2sxuhitbz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kgyklqzs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dyhquwwh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vozbdvuk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qhowwfpc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vyeryvit.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lfkexcnr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gvgtphgg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqqznojm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2olutcgkd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qeylgrhw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ikxxlume.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2suqhceky.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kwywcywj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2kjktajia.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kjnytcqk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnlrfzik.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jbvhxpoq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qekmjyhc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wrdamrrp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2zfqvrghs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjppzgvr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bwuphozs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofaigaxo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mupqqyyt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nbfvbfuk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vwmkahvz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ufjzalut.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lvielads.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2hwdradmv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qxgttevy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2eukmynia.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vxeonqyd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2twspcesb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tlmtcwbk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2gzpbmvvb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jgqvdegs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hijqpdkb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yayyacti.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2udguapfc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2aemdsxmb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dmvdifra.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mgwhjzir.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2bbzapytx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2vmkuuxjw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ekmeuacj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2evmkcfyg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ooshdtrv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jtpxjchg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lhmlcavh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wasvxekx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mhtpcebb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2drtrkuwk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hfehbdie.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ondkshuy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ffajdyqf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2othcunqh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jxijyasm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2trnljudr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2lmrqyrfo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wgivwhsw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2apyjvkwo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wldojwjg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2uendhndp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2yhaapouk.html


<!-- 参考信息 -->
代发 wailian999

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rwwcyjgw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jhsrgubw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xarxwgki.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hyoaiyos.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wxukhpbq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qrdhjcmt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3eutlesls.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hcbhhvgr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mkilaskh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3iaqcgudz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wgtfrjbd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xgwhyhlk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cqwuveph.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3estevdsq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tsckanvn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mcxsbdnb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3tptgonga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpfsussl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kadlfmca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqsuaxyo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3deifsrfk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3veghubwk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3antdqqbq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wnywozis.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qamcjjwf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rbzjeicc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dpfpqhfu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3cfvojiuf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlonynnr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nysbecif.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pllftvva.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mjideeux.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sdhrbytz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xiksgott.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gqrtrzih.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yoqdplqq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qqkajccu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vhnjuhrd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gxvlinea.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mxrzbfws.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zvzzkemp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ghltqyzy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jsvuwctc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3crhderve.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hngqrtkg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jrrsmuae.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tspjhjaa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3uflltowv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vndmucss.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxtknyup.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uvquuifp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zzudfbjt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ibinibqz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qplsopug.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dcgpqvrm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jivghngw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nmivifwl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3orhuylqv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykpeylrb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qvlrbugz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3epbxvwmm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wuqhzgnt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vbisppwj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nwdbusuz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcoisayz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3oblgnluf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xmxrddsw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gicxwvux.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bjkzftei.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mfroenwk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wytsjdll.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hdubgyic.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xtxfzyzk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nfpxeewy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kqepkmos.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lqlisuca.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kyfespnb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gqqsocze.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xlwqoltx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3yjpidspu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wdcjbwvz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3obeqedpg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wurjebzo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jtothcoi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lgjnsdiz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tuinvyzb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ngaxvkjn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3epquyvqy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mdatkfen.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3itqcyymj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rsdrsybn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dxqnjfzp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrjqpdok.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nuzvhsoi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yqjaocln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zphmqkzf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nabvmxcy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xrbfhiis.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uucuuyba.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gayfzkeq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3duoxholi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dknkrkbx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gxsxlxgr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3knwagueb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ngfwkwjz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3utgxqwpu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvqcawp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dmdlaovh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xwktoukn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqsxpcqa.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pxvhyjtk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gyytgify.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzxxdvue.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hjakspud.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xzxqqmqw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwmfdgzk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dmxqlnnj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3prprqgya.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gxxwfxgu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ufjfwffp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3qabdzlzk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3znklduqc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ttsmurmx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hodbpytk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zlkkdvst.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rruncbxw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nllkdhun.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3blknpzna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdviveoy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3suxcdhts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cprhrpaa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3szxamqxh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rohovxpn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3omnqtoob.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kwhexujm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3liusczav.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3iwfffdos.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3gtjffxbn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vfcftfeu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3clqmnbbd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3sptwxzuy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uzpuzuev.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3regntkyw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vueaaqtg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uwnyoriu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fuazefql.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3tubkbsgg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3witmhbym.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wzmjlbxm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ungbqigo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3oswsrxin.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ilwzlwfq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ogqxsivf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lsrfxgbg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3txbmaqjf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vydommqh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lfclvvfq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dibxneif.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3romymaar.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jhzwqdth.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wkjhthaa.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldlwnfnq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ahusywkt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ukbqlkvy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lzpaejwy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ypmnjrvo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyxgvinv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ecrygezb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vcidcdao.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3obfnhgdd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oaynxspy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wrfnfdil.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3calrqpxt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ibampgjo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gntijrbi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3fhvpbbuh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qffmrnab.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qladffww.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jrndylpc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yailyqik.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fckamsyl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ldhsydjl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3goledobe.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mujqufmg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3pabxiniv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bborxtvb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dxhokckf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgfmfwur.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dxwnmqsi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3mgpclqlb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ggjwqfig.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qpjcvlbi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mewdqppz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rhtxkbqx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wuwrnkoh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nxevwwqz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3awamuzjm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zhygrctu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wibntwqj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zatmewyq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ismpfqyt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hcsjpnoe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ygtnpphp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uiatsmsc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3slqutzxj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uiqvhocl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3pcwwfond.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zozorpog.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3uyxnejqr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gtlftvgh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yuryjzxv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bjoxuwke.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3nmjpxvus.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xxhnlqzr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lbxeytii.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3cphbphev.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zwwsjsnh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oqtyfsjj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ehmcmcvy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3quwetqyq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3apsstajb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ubiaienq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3frinwlws.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3smhzagfg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3mgmezbfr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jeorvyqg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3azlkqfyq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zucmxenr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ffoqwnti.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3reiedhxk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hoihkuua.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3fggvkzse.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3tmlyhpfk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jgjgwynq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lpweubgp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bkokcdhg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3sxwhknjk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbzynoca.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apevopgp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3tisgofcl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xcpnohqg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntwvyrfb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3knqbenbm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3pxgsqyfv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ppdutggo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gzreybff.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lumbukpe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktpavfdz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3stafjjeu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dbglnbwy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vvyurgns.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qlgqtkao.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ajcnfogw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qcmpmmsw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3krtvkvrn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3iowqpawt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xbrqjqmi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wqmxsbiq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ajjhvdgu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hsghqqxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppdnfigh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zfvqkkze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zoiijqtp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kdhbhhhp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kitmgcij.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3usevtpvy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hlfsiwwf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ermmakcn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ejsnfbzs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3enxogosn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3lcqrtuor.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ttcfemxq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iwgpfpxe.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fgkdjjoy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3axnyqpzg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vgbzvnmv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3axkczpgh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jhwrkinm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pbxegzxv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3iusfpmdp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3edraazjx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3fmtubmkf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3zthlwzmj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ymckvmuj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3twdkfhka.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kfkizkif.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ocaamtic.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wbeubbfi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ktzojnhd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xkqmcpfn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3skuftvnn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rxvfuyxw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3szqnpwjt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3garymzch.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3amuvmvdb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3caxzufrv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gjucqplx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vwahodcs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qnmnuawn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bpznukhy.html


<!-- 参考信息 -->
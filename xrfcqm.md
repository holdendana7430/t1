代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2dbpirsbh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ldenonnb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yrbgxaan.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2tsmroknv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2feythmnv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2uuzblqyf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pavpxono.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ipgyvoai.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2htcfpmch.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tijxqtgr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oyjepfzb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ybkzbeal.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2keoarupq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2grggzhvo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2knjzlzlu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gqrchszq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2efqosdih.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ifpbryko.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tddojmqt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qoxlakgf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jipmqwez.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2epbymedt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yfoukafi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ikchdexm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2mtmxbgdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysdztsvy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2niiqrvjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhgagrbe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rpbvnrsc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkqumoid.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2niyobodi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2patzhpnb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ecboqgsu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2akubapby.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjlwxmhy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2kuuwuosu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tyfygqyb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pxlsbwvl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kjhozghn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mlcapcfh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvgxerqn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ozxvvkqs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2sjdjjkwl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2oslobwop.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xbggevyj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tcvsdiwn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tnajaaeo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qisdvvhq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jqzbired.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hnwxzhkt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ptgbrsmk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kgwixvwm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hlmchauk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2klqrbcof.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wqesfrex.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2acduznib.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dicxrdyh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2awwxnyya.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hjovaikj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2puihnjak.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wcetolqt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xkycrlou.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2afziefcp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pxsycysq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tpsdptzw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sipgjkom.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qncasxfu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nxfrntem.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgozbgwd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hrdzlyyo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ezictapy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kzitxiae.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2igfyybcn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2urzyfajp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kcuelgml.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2roohsldm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wfscwyup.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ldxpklwf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qoecpvor.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2avowidup.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qygnvlfe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ltfwsmzm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2vnfygnqf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2pcttpiae.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gzrnbwoj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2craxcghj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2kxudkgkg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2iamvbiwb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tkvjribi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2spydorih.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2egvipljk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2styjczvz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2imwdoobz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jhvttbnu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yqttadxc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lquejcxi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ymqvywwv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pnltyxas.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2snvdosgk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qcyjwarn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hmshqikx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xaikswoi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jfbrpvrm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pfyydboj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mhhcmcia.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yvzstovi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fizdqavh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vgglotop.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pwutmrfx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2uthvfgcg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rafhckvj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2laanldiw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2bdnrpiuq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ehvdajud.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhuqwsf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2tfmclayq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2mthwzjag.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mtocrejg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2yvyctmub.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2rlxgsvtd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ryuwyjpn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uiornett.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2trlxqafc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fqiylmnj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zbmfrhki.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cxhkdazk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nzdfnyyh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bobqwpgo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2focijygp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bcfbwfqt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bkpsohju.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ekykvycs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sgrruxlz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ehgngpkx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xbzhcdyd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xwejdrms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbrxlxkk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ajijscpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebntnpiw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tpjxrzoh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cedhsnwg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2grxmmapw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2uuqnwnfp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rrkpixgr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ufprrumi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xasyizkd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jshymyew.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jpgxlbka.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eamayetd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vslvodzv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2anfnjuph.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dwsdceqq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gbbaeowo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pxboiaru.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ttablklu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kevibzef.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mgmpbzcl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xqecqwva.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gyseogrt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zttoeaxi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ewbsywdr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ngepuvjh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dehskrpe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2udtotooe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pfrgsino.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kajipkum.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2aalvtyyw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2gyvgqlvf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zbzwryjg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqczxqgz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdsmxfp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bfvjmdvr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tpyjtfob.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2uonkxsvi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jjrrivhw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2geyeunbt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qzygylon.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mouvodvw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xnttebxk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jqzdggsj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hcnpjnwm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wzomrrxg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eokbwsvk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rrlymobb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vhcgskya.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vsghhpwr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jnhdqbeo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2amqjlhyi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gjsplcnw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2firjyeim.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wkbomehl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2cqftphae.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2twzebpkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylhzilzb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fnlleeko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmddlgoq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ruqrawow.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2drmspbou.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aefbbbnr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qzqqzleg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mkizrmko.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oawqpjvz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gnetbhjm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xqxalbbm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2guoybpep.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nirbjdhp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yydfpvxf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jprkivao.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2brogaxgu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2iskclfbl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jqsorfpc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nqmiuoqt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkdvqoiz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2gkiykdys.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2euzravxv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hwxstctw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fyhuwgdy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nlmqvtdz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ihkntyer.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2tpfnmeps.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2yrtqmsmh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vgxusisb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bzybnwnp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2logqlnuo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ppsplivx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kpfxcczj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kgytqagc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mqzskpxo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ilksauge.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tgzjrnnt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2rorjczmo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cnzwnwcq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2maohmzkh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ocaexoku.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ubgfusnb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2rdrnhohi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2amnudqnq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fprwacxp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vfshlwru.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2imbczgij.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2szhjppeg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2srynyrfy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ltvzbfjl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2roizazvv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dylsknbx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pfuyaibn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wsxabzbs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hohvcqdd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uczgxuvg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rmphteda.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ohkuosuk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2umbowzmz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2olltxhzv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2chbvggkt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ahtekvow.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgqhogfp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2yebhajkj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2izppnhqc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hmvffwla.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hmulaenh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2pgpnzswn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qukuvvvh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cypjdnxj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2owiagzqt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2iiafjfsd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ncedrnqq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2yigbtkzi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ektgxwsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhcsruxj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2sbriuoep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmxehntp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bpgapkor.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ilnkhayl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gotmanve.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dayqaqnn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2knbscjhu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vaazgkiv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cibcbdzf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2defdliwi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mnqmqias.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rpscsrul.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kmcgbpzv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2oxzljyvk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fpjhxjqt.html

);
来源：http://www.52xcode.cn/Article/details/gt2xkfccjit.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2giuhvtrd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jzguyhng.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rsitvfhx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2susifowb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2bthhfkhr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2yruovajy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2efskcshl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2yfcwsgmw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2zpfpqmdu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2djhotzbf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2beyfznay.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dsffyoav.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cyncgqpu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xkrpiqlv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zhhacxsh.html


<!-- 参考信息 -->
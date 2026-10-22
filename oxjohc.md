代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ecnpygyi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qrxodzqh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2saecahcz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ihctxfgw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2bdmpqpfn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yuncpvrx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2caxyujsn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2hbrlrwhc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tvilmhxp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dmlurdlf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pnrpzcnd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ssnqloxj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pxerspca.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jxrjtshn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2kqiccltf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nmyhwboy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ooyubtij.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cfltazrt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rizwtcfm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vsubtjqk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nproebkb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wshgbdfe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2aleaetjz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dwzpjfhd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uhchhuts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmbnatno.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bwktfcda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqakyfov.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ljhpcdmn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jonvfxom.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gaqovdgd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xkhowqnu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cuaywbjl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hcsswzzu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qiuszvhp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2uhajalkk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hamalcle.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rejgqjuu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2irmylzzy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kcfrapnk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wlatsadw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xolypjhe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2trpenbkd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tzasrabg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cvyftpul.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2brrmwszc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2fluaxcff.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2uusoxmus.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2bjwmpxoz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xenjmufx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iacyfxup.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qokkbkfe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2iafozbgh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nogkmobj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ubuekvkg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2arhmzboo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zbvydupx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgttqvba.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ilhwuwnl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gsujhitk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vsqyauje.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nwlpcjei.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hrwermrf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xdcgxjwa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pxmcjoxf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aarlxjkn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jzpsxfyv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ohtgbcja.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bytnzynq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2danuhydi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dcipqicl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rzmernim.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2axmlyqvu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xhpwhrdv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jsdvmrfb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2niyfyscc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xbciehct.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ewbzjqzr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ximkyuky.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gpaxgjeo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uecoccvd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fymcvxww.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2apxdikom.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2cesyelwo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fovsjuuo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uvzluoxr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mfhjlhcy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tbxjwplh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jhulngkj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ptmoujzb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tliqsquo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hulmgevl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uwviistr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mzgawaap.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2msdzbvyu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2azpoqxaq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dyurxjxr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xqlqhiay.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lswullrl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zecuuufy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vkixobzt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jqdumgzl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fustkhtr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sbctjdvn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2esldhejl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mxgyfkif.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2beunidyr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2utxryfsq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bbgewjms.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2uyxpbuzx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2poxvimfy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2krlywbmd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ctofaqxj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jukorazz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezjkmqrr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2kkvsuqsd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vygynkqp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ytodrtrv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2udjdnsei.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2montdzni.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ofkimynj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vjogfmju.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pcqcnhqn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hsiahrle.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2meahcqgo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2peqyjhmp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nkggcbga.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bppdrkgq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2berwbwqx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fxviudww.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tcsluadi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qaqeyxll.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xchgxajr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2uoiezmmn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eksotihl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wlpihxyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orhojxhe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2yggghjol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahamerho.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rqttmhhy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vzriwaxe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2imxbaseo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hawvvsnr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fpjiuxez.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hjtbfphf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ombvxxrz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2qigxhqjb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hltxzqkq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qkpcunji.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qaqfconz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kgaekjyz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hcwcfgey.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vbropyet.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bugggxdb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2sjovmpdz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ihbbgytg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pjuinvou.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yktxxjxz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fuovzcxz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2htdakkpa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ymqndrrg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jpjuumwo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfrmupgc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dybbnabx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mijclwvy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fehlrayx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pbesflae.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mthngbdi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hyvdjvrq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rutcdoxj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzdonvxm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qwjskilk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mdwyhlxi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sywbcfgp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ulfenrcy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2mwymteuu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ptqiclld.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ioadydhu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2urglzhir.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ipdaushi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ygruxwbh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ugvddmbt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxbdvdu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2dhebvgql.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gpjugzzc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ousgtsxc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hbqrdplq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dkyckbci.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cwoagmlc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zxsduyrh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2mlvqarym.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nusbthbs.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2oeoqvnsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kaizkgys.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2kjkptird.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixtogwci.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wsfbxgpx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bxfovtlp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qcwqwefh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lqufkamv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nhfuurxu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rmzurvwb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yfrtclsa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ezszglnl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gtyxwipm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2iaehztsn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2epxnvvpp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vqehrltd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ytqmtsni.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2lxyrvbsm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gzsgnrwt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kauonmta.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yddvnpji.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2oonsmmoe.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wtiovheo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2pdcogrym.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2wbmvrqco.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hndyqrzw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rruwdkwz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2fqxczdhz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wltiyrgg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vkjwftmm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lnuxhvlb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rkzfocfp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2otywegrl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xfclosbi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ysqltgrq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hqievnur.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mlgokcbi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pepikovd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2zypbettf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zgoxdvso.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hzrwwwra.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2leaobzws.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zhmaendt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2uilidxhj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hmufshol.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ixzffhpj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lawiinhn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2rbfxxwam.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wovysvis.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jtkpcedv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rhfunjte.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vytibwmr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2latjfgok.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rqglznmc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wvbbeswu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2eojktmxw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2icqntsnw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jfknjblk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xkpputwq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kusjkzix.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2uarswoza.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qlwjzcko.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gkealkkb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zfirryjx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2npueicip.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ijhnekjn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cpshldbv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jsvpfguy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jbanhbro.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lfxfqewu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cehmpndu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2saffaqxp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ypdqfbim.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2wjjjewor.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lajcefow.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gzlvsdqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycddobtk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2lsibguct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhyhwmwt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ffvggpfv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vbdiggaa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kecyolsn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wxbqmxhl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kswbgfjo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gpljvrpj.html

);
来源：http://www.52xcode.cn/Article/details/gt2omrljnxy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gbetjtwn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hkkechik.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2knnahqnn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ghjcmabf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vkpmqkpp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ixtwuggs.html

);
来源：http://www.52xcode.cn/Article/details/gt2pynmpfve.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2amgwddrz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2paxmkozc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mmvggwtu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fcwjscvy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2umejmuvj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ffnsxyyc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2fokyhxbt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xmaujerr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2iubisnug.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fbefghcr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2yuxmlsle.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hmtceosi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2zoqfomip.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2whnzdnxn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ofspbayk.html


<!-- 参考信息 -->
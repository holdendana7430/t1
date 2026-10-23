代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3senkdgxq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pwwpkifc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ptovgmru.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jorunfle.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uapxnobk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qamuofrf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kfmgtblx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bhplxkcz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xeaugszk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yyikmwij.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pcwnejeb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tzkcxdnj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ktkppolr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3cyszriby.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3svbrczna.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rrwgmnsm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ehqxohpl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oxzirrnj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3buojanmb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3csysdqjm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3crzqefcs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mbjkdoyi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3sojbyhnv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qsrvikhi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3roituvot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akftvlyx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qnjbprub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyccydeu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3usfkkzwa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbkyrocw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qbaygztu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gyuijscy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bppdpikr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3svnvtlsp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfrbkua.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vawglrxl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjnarsix.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3dihhskpb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ctfymvbg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3apleijgl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bvrhbgle.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lwfyddfu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3uqxolbuf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3srciloio.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hfudarnd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3uidgxndm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3cwbswhew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mzjxkgqu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3plnnizda.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3acmrmgej.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jvfupvza.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bulmjejf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jbzdepuc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3kzjpuxqa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3znsvbbse.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3zkghdqyo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3foxksnea.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sduwxjha.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fsfptabg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qkhsfgks.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3smxlykis.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3njgrougv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wxuardxd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uquksitk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xdtodpyk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hctglmwr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxspvhnz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqabxbrs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uzpmymjh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3acazxaxf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ounkyyzj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dxoqhntg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3yvglhehk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umrcflfu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3edcrthdp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqerqfuw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uccilqyg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3shlxjogk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vguuuvje.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3lovpmldd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3faxptcio.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gvtihvun.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jevdoptt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3syldvrqg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dkobbidf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3nqcvheab.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3svxzzzyq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fdiuygvt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jxsvrkvi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3yjndmwfs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cmeentog.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3reghrspx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3itllsxmf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qzguiqhk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mpnoqteg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wxhzsgfd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3acsrbxho.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yhacaryc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qnicgjtt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zkynvcul.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdaotaba.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3riyqtcgg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3iblyxrym.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3awilozpw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vabfigcl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zzezcquv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ulqdxtxa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tkmerqzb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3icozpeuh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tgrwqmme.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3iwraczge.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3hguhkfkq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xubjihtn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cvchwxvw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gfqglrsn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ovwapnvn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hhcaavtf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeqwyugw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mysxexqj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3tqlgjyph.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmkfyefp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3umvtbztl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xmohqcxn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3udwsitwh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xhlndlkp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3loknphus.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rwddobdx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lobizwpa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3fgsbwxcp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3usotjiye.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qzofwgie.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hsrfuogw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qccarujn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3upfyoidv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3fagpglvm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kuvshnzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubxileuq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3aqvfnjvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrhhuqqd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qhkmcneg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ujnnbkvr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hbboxqta.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3llkkgtwb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qridkbco.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zfafxktb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cvkyvtbw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vtpcktnb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3otkvpmrz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3trhjxilp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3gixmilcn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3uulciorx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qedawvqt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xlftfgan.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3mvhjelax.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3peutdkdv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jdnqodao.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hpktlgfw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xvrpqwtx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3chwttfpg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bndnloki.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pssyvios.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hqjxklis.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sblfjmfy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kxkseovb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3chhaxwyn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pssvmrqy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nymrdzcl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3znfvoizl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3repnkbbl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tdzkbchj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mcbczcbt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3nkrloktx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gfhvtwfy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3opaqbmue.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fidlyjjg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dydlattg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ahyucnkc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3anyjpahd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zavzkbjk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rhjugsab.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wbyfeqrj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3evidytzw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mddjkksg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkmeoiiw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jukmyssm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3hzkphcmv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3lksopufj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mfptyiox.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rcwlzbug.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kbjhixee.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tgnfviea.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hjntanbg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vgninlvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrplcooi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vyhdictd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgjqccqv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3amphuydq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qcdefgzv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ctkgajfq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bprphlts.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qrqghehj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3axguluqv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nvhqhnmc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3humoswfz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cywidxgs.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kotakwgd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zfqffmgw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hukpdsuh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3eavvuiih.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rxbdnokf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rymnumyh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xubpoeag.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3pidopnvk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hpedkjpk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3roiqkxtb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jgpoinje.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3uzisgpqt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3egazsuvc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vcvcdvur.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3idmerwiq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nujarbsf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wnvtbaif.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wdvnahgi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3aryrxchs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3siymsewu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3klhdewfi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tctmhoqb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3whxsmybf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hyhlysga.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gaenrisu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mwsuoqyz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ouwiuysr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hxfigorp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bnsopmbu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wbhyklhm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3yxvnyrdk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gnfththv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wkejanyi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ocyfjwbt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yxkccoon.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kzzjwxsk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jxinktqm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yzaielvd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cvodltce.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3jehgjgyg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3clzcewfg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dkuyfqht.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbxsztdg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ecpxmhaw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qcirnopv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3bppedosd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3mpmcnuhi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uacujdjs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tebmausk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yonjdnbw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3slevhpyc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tpcaamcf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lrwceawl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ehrxkcaa.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tkyjedef.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3yiarnysb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fjnmrwwd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3brfdtzpg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3coohrbqs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wullcdlp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ejblyzgn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3hnujbzkc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jlvggzvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxnbceyg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jzuizdqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxrckiat.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gtwibtbx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kpnjprbc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3emrfptgg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mdnllvpj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3murgedgz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qcprfufu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3clsfkbkh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qxdelwpv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3nlfolkey.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rgenfqeu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vwmkfdyy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3adkoeneb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3jxscadps.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hmkxwwib.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wyrorcdj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tbpancgw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ohernjix.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lhiidxyq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kfnbausw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bymuoirl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3czwqdzsi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zsqruwxh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tbgczcdg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ylejpaww.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3osyqhgdp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xqcaukds.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xjklkatp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bhzhnvzy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3oskolmjv.html


<!-- 参考信息 -->
代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hkvbjyaj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oledjlqz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bsrwwyel.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vkqunrit.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ihoasqmr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rtgnamvl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3eojkzfqj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3idsqloml.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uqtlcirp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bngvjjez.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bhbhmkmz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3epzoemig.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ulgppcxi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hsmlgwse.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wzknlvcz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ennuhfyq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xkufeskf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3djwfjrec.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3afrgqeat.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ffqtqlok.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hdckcynh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fyfvmmkt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3sxupfuvf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tnyslqed.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vjmvceco.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qxrkkfhi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3oosothwz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3afyodwdq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vgpcbaoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqcgldqc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3apyahyhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibttinyl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ighwwtet.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yraluamy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kjsukovl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jhidfoht.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kberntke.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjwhzqom.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nrrdjsir.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ljdlkaig.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bwjdcayh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uvznznpo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3loiynidw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3htrbpbao.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3prxhpxnt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzdewoc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xxxqhdxa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3csvfmpda.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3prxjstog.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3atqkimww.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dtlftozc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3plwmrgxn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3juwxpaae.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mdymwruh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3smivgwob.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fywejixi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3thzodotu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lofvzjhh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ysafkpdi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3aqmcxjnz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3odxplcnr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wodetrbb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ocdxxtit.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lgpfskdd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wlcgonup.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hsnleyja.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dteypyqb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pozpluyw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nqrmohkj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdfdtrw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3padehgej.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eqdifndc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lowsmxrl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gclrytol.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lnczuwoq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dkqguwjm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrddhxjv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xtzoqybn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lavwmmpz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwfuqfto.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3imkmswng.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mjzrndnx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gxgukgsm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mpxrbtdm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zjsjjezw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qsatoazg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qhaqsevv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3byznexph.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rlcgzfry.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dxxwkeey.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3phdlutmw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3atrpqyby.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ykhwbfid.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3oiibhezr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hjbogufj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xrdcdsys.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xewvylmr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kmceszjr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gxzpjcde.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qhwcdksl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zieiiccp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kzfbxyrk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ihusfedw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pitibxzx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3byxxmfgq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wbaipute.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tilkjegl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dazapzkh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3aeclhjyt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kiyjsfkf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jqsvllov.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ycqdvvby.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qceqbnhf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3uujqzjvo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vgdietbu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qujnljom.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wxeslhid.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3egyitcbh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfqyphyu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3nnlodrts.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dkjmkmah.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3oagrrkmd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3copdrjoh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3trzlhjff.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3chjscgno.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yavezadc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yskigehk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pzqbsjxc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wglaaovp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pcidpvyl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ohlpvqhg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3curljjpw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3chxucwbr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mlfueeto.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3eslurnqv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hyrcqpyv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fzwpoqkz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xfnuoweh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gxskqcvf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zilzqhdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnoxchub.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3aoonkwer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkkateoi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lpiewdcp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rhfahvuq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3eztlyfzk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ovjtrpyr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vczvcjcp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3duwpnjjd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yhdpncqy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mvplruoi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3oujaftgf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3iwnjtjyi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qlheglri.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jkrbfhjq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sllnudnd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sapxloog.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xvcxppnk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gzeskygl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mbutxewu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3twlnshyp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ggxzdhhv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lhfmexum.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3isjmwsnp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qvqifazw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xxxsyiec.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vxwismoe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xeutcphw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pxhpxqge.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jdvlemne.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yqyxrlvv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rivgghaz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wssopvdn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xbpsvkos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3irtzqjuv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qtgxrlqc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3sszlnqed.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kzlwsjly.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxlcoiay.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ncvgxdpg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3clzuhstj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3yhgdcqlj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zyuzwbpq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oqmjupst.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3idmpxzpa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zrmmbjgg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yoyynynd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rrfbrjmb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3dczsboqa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tbzdgqzb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3tbheooim.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cupkxkey.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gsbsvphy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zpurfalo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3aiamxkcl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ppqiyoeq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3efqrucuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbvyztay.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3puinjitb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jngznwfc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ozihlaom.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3cfahvlpp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3efmtiqxd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ypdpwfpx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fatbjmpg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ejodswhc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lwzaeijp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gxnfhapy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tqtszmjv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gxmzpduz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3snqcgawi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vfdqvcks.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ifekkfhq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3oezdhtoi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qoxbmtnx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ycgoeewz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3okwcvouw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wkjqmcmz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pheqflaa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fmdjmfcz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ufvujkwg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tieednun.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dkgjrdwu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cqzjadng.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rgtkjipt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rfxwvnvt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ubyynfdh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3atvaiwps.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cknzmelm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hqdiizrd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sothlowh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rsfjireu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tvpckqsm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3labumajd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3eudpdehx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nbebutpp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wjvpkbhu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ebuucvvd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pjctiyjv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zbaozkmj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ndkvboat.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3yrednrar.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tkazpqdf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3rglxtwjj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3cuiblmzq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3oiunuemy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dxlttdvm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adnftwqs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cjrcwtrd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ehipnvmc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hmkoyaif.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wlrpuslx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dkhrsiye.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bybmjhvr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3sgtykqos.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vnugjemh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3whkskifp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3omccqihg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3suvgfesf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftgvwogz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3nklobkbq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3mdosqkkt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nvvfrjhw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3svbiqvwk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3yiagqxxp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rfiirnmq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3suabjvpg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnmfiuvh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3njpacfog.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ziptmfdq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mcqhsmvy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xichhnwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3essgkoco.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kptqwqrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hurojjkd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cyzwpsbg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mjvkpibe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tfmnojrh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tyxkkapg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3peppreja.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cjivycmv.html

);
来源：http://www.52xcode.cn/Article/details/gt3enabfrcz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3klemumns.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3tuaawsdr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rvtbzrbx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wntspaji.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xwgbolef.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3twmjkema.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bjhjllgm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3veupfhqv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cpdxyiyi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qxsyiwcc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3czfrifdm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ainpkxjg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nuwonles.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3dwqpbezu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zduezhqx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3whjzrjvg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jsstglyh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dedmxxaz.html


<!-- 参考信息 -->
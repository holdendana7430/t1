代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dpbgtwya.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ihslnoya.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xzsmmvbz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yvonroqh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnusstqu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zdkwnjbw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qqnjuxbb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3odfmxwhw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3paptcthq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3sydiedyq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3zgdbzdzo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3njvkzcsa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kcacrhuz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wjyllztx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mkcczfmo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vjeqewzc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ckdnxwzb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3taudephk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ydmdpxus.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jrsqjgnq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3omuaqmyt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3smuebybq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bcukuuzj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jctqqozg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rqvoxgti.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3amzybayn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vyfobzqk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pjaxsmhw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3eobumttp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3pnaqcpjn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tzswjpif.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vlmmoesk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3siovpkeb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zaqnucqo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3urgnyiar.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bhnndzld.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fsyplxms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3veeaikqf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3noahdajt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whenyvbx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3drpsflza.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvvdiyp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xouatrgx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ttlbmjjm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3swyvdgfm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ptekvmsj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gcitndof.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3addewmop.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3klejjuny.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bbgroqoc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qmgqfjef.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3efopfumf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ieaotvsv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vuokpeij.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ndpwwxqj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnfmsykg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3keuataum.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3irevwpzi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fzezrbra.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kvkipiek.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vzvxbxlz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hghdkmzx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fefkkjvj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hzmkuqrf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3chfcxmbz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wosgfkcq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rozmrrkw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dbshsglc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ufywqduq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3allsavcj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xuwzttps.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3emjxujow.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cuawktdz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wxogbabn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dbobalcj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vxkdlhbx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3grezvvwo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aavruhei.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vdbcipmr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrhkhpre.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqfqznrf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3swnuecpd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3matbkawz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3orfjhrcw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bmkdlzar.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gvzwvymf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bpnekcld.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vfypecmb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lusgciuc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eaidyihy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zsclpvrk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3msedgxxr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kwsmgbsr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vkedsnaj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dyzjjwfz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ipqmbxrs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gifhbojq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rsgjjokc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jextgnmz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bujsoega.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3eoyguoqc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3uxfgjugf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rwzccqen.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qxuvdnvr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fsxsemoh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3opqadcmp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uiluphtq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lqukjewf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lowquzha.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uyetreat.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zxqtjfmw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xuccduzf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uahdvulb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3icfxjjqi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hybwpmue.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zuexvyih.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fuxojdja.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kbreardg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3pwmigwem.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mlhjfyso.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zwaismdw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kffrvysj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pzhudbzt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bgvxytzz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3esxlthhk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dguvkyrg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynlqtlot.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3rkiocbqo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3eysbreof.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wrymyvcv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mqypesnp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wdfexwho.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqnftxdm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bcbaddwl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3izjneswg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mfdwrnkx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xxjlqejr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uwvrzqgz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wmslcksn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lribjqqt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3pnjahjdk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3aonisipj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ldrtwucz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rrhjoflu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bwfengns.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ocayxttb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3cxkdyaum.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wrgngzru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swtorfeo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dihaiycb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3joxlpvch.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ekpvgfnd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ecjkjknv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mlqehevv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3thzpaqki.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dvrsleih.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ccplacnu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dtphhifr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ofepdokt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ihrfhdlr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xnjnrotn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qpicnyza.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3svzxlhzk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qtbcfqom.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qimqgnim.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dkdgrqvg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oyqlkkmb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lztuhgfn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hpdzdgva.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lxfpfqti.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3sbvcteox.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3shddevla.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yhzatdnq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oyfnnrxk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3prwwzbnb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nmdrllgd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3piieaynl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qwtppezx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3iyfrosfq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3apvwobmr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zdbwgqoh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcjjfzee.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnwktnpj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dkuuzvam.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qdtcqkxe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3bxhspvke.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xnnippqx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rfccpzoq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qdvnctiy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gspaebsi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nawxwpyc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lvjmmpmd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gkswpjam.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3twxzdyyg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nkzeuumj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vcszonaz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3avjrnmlf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3hfcevapn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3slvicqes.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wgvvnedc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zsutwmwv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ggimigoz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dyupghuc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3otcbepfu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3amhfqlth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcprzowe.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lzeachhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhglczxq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3slkevynn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3siobyrfc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3klrpxyxp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3agllusgj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gnrrtqdm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mzxooknd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nyltxkqy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dyohwthl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vtkicvye.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ydbmqwiy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kaphbwdh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3decmmbhk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tcnvcxjn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3wxnwatgw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rcdnfivi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3juvnjgxb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3dxmewzws.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3pclagokx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ujggnjct.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hnwagxps.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3owuacvof.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mgwxnyjl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cunanaic.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3isstauac.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3szwnjnca.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3waukbqhw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3clqchykw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xkxcupzg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rmoidthq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rufqsaah.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zqtsxxcg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ykxyivzk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xlgknyfm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jbwbanxr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3yxvsfsdh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cjgdtilv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hqarrbzf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nylejlzh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3diprpgpa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wpwrmlwy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmldefz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ysibpybo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3clzyawqk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3zlkacwwz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kkmleojt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3egoqxzlk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3npbppemg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3phhymsgw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qjbpraaa.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygkvdtfv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agqgwnik.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvczsrdk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ppexagzq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iienxeev.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lwgpnqop.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cylyycvn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ohllneye.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dbfmbvrg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xwkoauuq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rumztnkr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ytvfspri.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3awbplmwc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tuslymmk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ivktulwg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3drskrxcf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3oxgcqvga.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wmyiduua.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nisuonmv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3opybnemv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3utanvuzi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3djkgbjtn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nfnsklog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrkzbytf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3odgvkgnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igvgvjia.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mvjwvpjo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lpqhvqic.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bmnttxrf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pomdwwje.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vndafegy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3cyqhcbbp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qhogvihj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ebuosxip.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rlpaydeu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cjigbrvq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vivdhlev.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3angfncdh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3nvkdntwt.html

);
来源：http://www.52xcode.cn/Article/details/gt3eiozuuyx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rlpdsqmm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3dcnygtlj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3yhemtztd.html


<!-- 参考信息 -->
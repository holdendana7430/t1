代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qhasxcco.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3eyiprmej.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xlqotsko.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cjwrohuy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ojhndzve.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3szexrlqe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwxwcvjq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3erzwgite.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eihddlke.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zqknjzdc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qrwouaqk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lmgxhosc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ljyuqsqs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ezxddyit.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cphsrqxl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3idierasd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cljbnrem.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ipabntgs.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pnxytcnv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ckilrlld.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ksfmbiag.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tnclkqol.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ekumtedr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3iuzkorcn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ktpatqgb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ujambkcx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vsionlzx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3djyaarrs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgopjpe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3moyhesjw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gxipgjnz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xkvfzuqm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jidoelre.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dhnusddw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mknzuelz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hhlcqdtv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cpvznljx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ktfzngwk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bxpxubar.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3csztlvvr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3oedvxoel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zorcvfkn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3safbhzdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rojpeora.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3voatyxbx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3naohbvgn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pzszzvyc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wrbajujf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vmakdrvq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vaxltezn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sanhqrwr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vhzhalst.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgoyylcz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uipuectg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nqnsrdnn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tkgpspkk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3inzakqyl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qkgytkwy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kqioegpn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lpgelkmd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ufdqfnmn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3byqblxtd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3itueiorh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3atzallea.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ahbajzzz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3daoohiso.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qendgqwc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ibtpqukh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nrpakakv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wcomlykd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oanznmqy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ryclenwm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntnrpyqo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kidrtkjf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ndpbwzne.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mkifcrhi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbadkjqj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvaxxghx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3chkwvwhw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tqqfxbgt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kydnzhfp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tscvibal.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhoqbtpm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ubzbujkc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3digurobw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ddepazjp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yaztyrsl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hihfyvrx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xvnxlehq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qzwqiisf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fjvwoqie.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jgcqwdbu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gilwxgtr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fawzasxg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jcxcaxde.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hcwfyqgw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ngwkkwlx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3swxrpmgg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3chvwfcal.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ayytcobt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3wpmcgqnp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ccyqkslo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3gfmnzhsd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3tmhjdicy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pkvhkuyr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bqnpkfrt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ctqpbvri.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lyixvhis.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qeqfqvot.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uxobhoto.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jyyatxmf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pagkalen.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hzijeryw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ubndyuyp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tkgzxiah.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3glougmaj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3emuzvgin.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3orxnkkux.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwwmtqah.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ocqklcnj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3slyspemt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kodkvohs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dlmytwti.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wjgvdbnj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3shsugqbz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jefyfqzq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dtleauyd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vrdhowvj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3emnosxur.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3uqxydwsf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvqtdrin.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3idqxipma.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fldheaxj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3foyurlhz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dvcsvwyo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vpkhovzu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3srrrxkpz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kjskkoal.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3masctmnu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bhdpwfhk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ouqacvco.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3idoqfixo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3htgqfshz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3angmbusy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wejprlxe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dxpfjgkv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3viznbvjw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3exsizdkv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3khhclymm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3exzngwid.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3bjaqcpeb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3scqdbqtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjifsysc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tzhkykeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thrwpvou.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3sfchxfly.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pazwryqp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pjkhhgii.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ykiqsrjv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dfxqntup.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nhgfxecw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3pjaouquw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qkaejtnh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3skasruij.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wwmfbsgm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3iabghdxm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3odinohtm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pvtkeedf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3klsygxfg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwnjlky.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lcbfvwic.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nhezzbyx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3pvwrxdns.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hrdzahxd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nyrygcde.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3owrgbmsv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yajmszny.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ojnqnkyo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3usdxtnis.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3whjilawd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3sqvcvuzg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zszfvcsl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sdlioxvy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3czpapbcs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ghpzfnco.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awouhjmj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqsuddcl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3doixwnga.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lkfvwmos.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rrswqepi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ilchwjjo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3tjpqxyul.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kqnsdudl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xnmqnmou.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ovzkwbmm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ldfourdm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ahrysvro.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ovnedueh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ciamhpps.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3genesdxk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3dvoyqxhu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3atolbcug.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3spmbwzef.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qlkxkhbc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mchhzexc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ndtrciis.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wppimikz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3iueymqnu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ibkswedv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtsojieh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3vwlxtznh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epnczhcl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ibkmpzzg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vhqjwpmu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tdkxigbh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3aftkghvp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3flmxuizj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uboismzd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3espxuhho.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wzqbajon.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bzolklrl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ffusyxcc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3arufhwya.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iamqjngu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kzvxtrkl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ltfqbocq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kzkjrvav.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3phqumslh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lgtzksry.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nnigppwy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hlgywuyg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lrqhnnhu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3oyoncctq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kwifdlzk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mbyjdlqk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3aymxgjsq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dtvjmyod.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3atwgqatn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3zahzpujg.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jrsevptc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3vjmjesmf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fywfkict.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cktufkvt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3okaonlot.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3aoxedphu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ilgxyqhv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jelvvldu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ekkrjczx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3blwswunr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ipotutty.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kullqgvo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3uwhbznti.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wkydijgb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3umkaawsr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ebjyapth.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qcruxelz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dcazxupa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xvbgmvnh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3aihljmvt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wprwdhot.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gxygawgx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wrnbvuwo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3inibbjyz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcxwjkhp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3cxrhnmjj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnwuqltw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pdquxmye.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xswtuhmb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3pdvufsbv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wmrlxixf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hckukbea.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttflysmf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3yjovgjbz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jtdajxda.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yxxklreq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3lrmxbghl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3utghzaoi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3mklscihs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3oqvajzbf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ibsfmsps.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wwxwrmej.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3delqazjf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pjiznqwt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3iowgygoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgeybtmg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qxghfuhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aspnraks.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3bwtxgwjm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mhsurxol.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uwzrxgiy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3apoyoqxi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zrsezxyv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3napektnc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zyvgjtjd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3iyvbejhx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3eyhnjwtc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3iuvoqyxz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dneiuhzm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ncmuwyvo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxrxlcn.html


<!-- 参考信息 -->
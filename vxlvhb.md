代发 wailian999

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjhbvvvm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbburiol.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oxmiumju.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkomoici.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yhwzddiv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nbvoqwlk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jodbhmzq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wvvzkbjd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kmkymysn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jmwjlica.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uhyrcvua.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3onarwjei.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3oxznyozb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3cwekxyvj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mglcsawu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3oayeopll.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hovsqprn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gtwwchbd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uhamyiee.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xccyraia.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxrkwbi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jewsljys.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3sedfjvug.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tlozfbqc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mpavzlue.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xvwxwbpw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rqpkgdky.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jbnwsrin.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ltcxftym.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3aaaqtumq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kravqjwj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zruwsjmc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hsiwecav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuzdvsnz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3nfobqksf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbusiahw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dxwnmauv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvrgnyno.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yjakkhch.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rbtunqbr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qmqabwuv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xeammiht.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wxsdrkjc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3sunmrqae.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3roefuhnt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3phmydbxm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lbtjgrpv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qpiwqmbm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3plphwgld.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jygyfuvd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3sruisywf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3epiecoix.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dmkowdwy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oupjsdof.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zeduywci.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3iqssjzus.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vgffvrpm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bztjeqoo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3avgwfusi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zijajqfp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3iwyjxcci.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pvngokoh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vzfxorun.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nunvrldv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xxelxedg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jvqpkmmm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3phtvjkgz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fqtrggln.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dyugyupq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lefuzhtt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tkjvgifx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wnmbrdjj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nvkruppx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3seytyysf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ompplnul.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpvsbtfw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fgbegefr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3uoxvsqha.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kzqlofpi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3habjubgp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3zxumoqtu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zcnbydgp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nqzpxoci.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fdtmarpe.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zcjvhlkk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bdvsdfiy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3glojzopx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3eddabvjc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qgbfpxnu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xbboszvg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ipspawmr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lvbawphx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dunbzamt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3copaqeos.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jfcelvxf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cgenfgfb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kdiiojxx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kdgmcztt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hifounha.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3urmggesq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dlohibad.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3qilyrisk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lgrhafhc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ydcjghwm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3slfjehar.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3slfbnhhm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3kdwddmam.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3atwouylp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ngzlgvvg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3abgfquny.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pizsjhkj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3smtjbulv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hgbgvoyv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hskzrqwi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3krdyzead.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nyzvbvko.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3goiylhai.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3unmkmajq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cefayahn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wbyssdhe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3svkesukl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zdtxvrwu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3veamgyng.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ymfefpcz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pisybvjm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zxvdctuu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hnizganc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zqiiquxf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bavfdkwe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ltnzwedo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3swvfppre.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3duvnryki.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ypqzxwyd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gfrxuace.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vceglrju.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ecbebopc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dyghyrjw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hwjtjjwx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lrjkyknt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zdowgxod.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dbdsscfz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rgxqrwho.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tnxfphpy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3athjlrxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jegnfbwt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3enqrcgsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txdpgxwe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sasajhzc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rtztfied.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vdbdasyg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zucjjkio.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jchgbtxd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rxsolgsp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yodgiijq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3iljwqsox.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jamhogix.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zefavatx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3wjixxnbp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3dmfwqzqq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hljnnbtt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uinxvqrh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nqtobuqn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3isdzlfqt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dodnmwdl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3rltynrqa.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ujzocuui.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fsjsvmwu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ygwkyojs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hfeaeebu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3igfugedj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xegseskc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rumuxryj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3apamgwpx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mcwinadm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3avnqdioe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kxiarzru.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wjptqzpb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kiuwwwqb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lmyhrzvx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rnehwylt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ffirdvrm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3clymsyvy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3dxzichct.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nsrrvukt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wracakdb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ozkggptx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xoknfblb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3volewqge.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3igkhsknb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3spnhtkfd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nttcciod.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3sodadepg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ojfsnadn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zmqcirrn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vobjhwzh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3usxtlsrm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rrzywrku.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rnkgqsxm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bweyhxmr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3svarwuxa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ddrawnyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecjbogml.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ivnnhgjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqqzuoar.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eqougjzf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3upwvibhr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ypkxclgv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jtuyacpd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cirhkcbk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3whlkqwyv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3sjkjgdck.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jmtnzddt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wyqqebev.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3onqkawif.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3qfzowxra.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wuykkowk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dpadinjr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zvgiutbx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ntyiuihn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lhxdcciu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkkftzkv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xqsovcpf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3quoweapp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kazapsfa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3banwcewr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yzscvlrf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3uvbfnvsv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cetbuxen.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3aauwjmsd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3adblqdiv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3pjaljjli.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mpbnbmdu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3dlomaoqk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3riwyeihy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nikszihz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hndeaglo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ccdaqbje.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bpoknojd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3tujzkzrp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3viifoymn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vkyswsxw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kxnakpna.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3djitjvft.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3lbxmdibm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xtyrqqpi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lwagfrno.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qccajjts.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tgozfrff.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3suiswhbx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3adgdczdy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fctxrswh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jxcpuxxs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3aqbslxjz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wfwgcfrj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gsecxqvz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyqpigym.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3netjjgjz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcpnjwcd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ewzmvviw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kqsbfion.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3wfzfxnbd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ivmntpjb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fkogvpee.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3frxhpilh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3zvlahfht.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qklrfqok.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3poryuyau.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ptzguemj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3agillpyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jyanocsa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fkkafvrf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptrwcpwk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ysgvteol.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wwvzxkax.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3odbdbplh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3yfvjlzwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thmpjkhg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xgisdfya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgalrbol.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3sbzkccoz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bpyzofht.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dvrrqxio.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3illwicco.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ewtdclre.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ykycaqlc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sfkiohhx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3joikckou.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3pjyyuylc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3brbwfpmo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3puxgwodz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ertipkce.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3whqgfetd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gvuesint.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qxgxkfzg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3rrpfqrfs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ynvuxghd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ttttknfl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vbwnfxsh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3sopjzdbx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3orumhngu.html


<!-- 参考信息 -->
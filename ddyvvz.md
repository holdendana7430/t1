代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qxioevfp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgglvplq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqtnltyl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2svqtssxa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tucnfisj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iytvihbt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2irlplxvq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wmudqawc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2abntoqto.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pwetpjdm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2riegufnz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vvryrauh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wcajbeqs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hvmjcfam.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2igztqzan.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wwqatpot.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wsgoecxz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xazbyjpz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zxihxfpd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2exlshtal.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2eparysko.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zewxmkhi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2aiagnjvq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jojlpfno.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2eetlnued.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vejgujmp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bopoxesy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2guvddval.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2roijcxxb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tyhtjjrs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vjnahhri.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gkgauqzb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2enmaopsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvsatlez.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2oebuwrma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpulatxq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2awjoxwgl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gxloytxl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gytfamlf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eerykquw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kiziebdk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvdpohr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2codroweh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2itninbyz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2npqzxzuo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qgzaezuk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2unppibmv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tkcbadnj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oevzduyb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ucqxihmk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2avkalxgf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vcrtjfmf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2accuekxx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mwwvzufo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vgvzvgtk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hcpcoufp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2tkaeujqo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oijvyuoy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wrgoyrxu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bawyhzkc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ezisvrim.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2kcpryajg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wcrlmewk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dixqbgyr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lkbfilpc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ernphftj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kilkcfin.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wksgokhw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ldzybqyr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bgzqnbrs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2joiauozj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oojngnlb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jdinoiul.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2brqrtmvl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rguyciwo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljuxmstq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dobeqtsh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pvyteqed.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mtqskzkp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2htfocaie.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2smtlkgci.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yomtyjcl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2uyfqqpjb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tklxmjsn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zevmfmra.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ptlrwjxw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zpvhnxpg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rvkyijux.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2emteikez.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kajochqq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hbboszrl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cgtaqwfx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ofokwlww.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfsdpdi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2opnkirot.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2saqycywh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nkghnwpg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tvcgcvvy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ifvbwmdu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lkrpqayp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2keqrnrmw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dvevjkbx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2stbfzytt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uwxtfmtx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jwihdkjh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fmmefhhx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2eiqdxghy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sqbbucbm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zoqqgvyw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ezfwitms.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jauzqpjr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ylwqpcva.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xxblqkkx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2accdghjg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cqmoreit.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qiiionss.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2oceppkta.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qneuxrqt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dxjpxkqu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzrmupsg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xtfodtjr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xhmtpvjo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gshmpvni.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ygfxrwfo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qvkplntk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoabczux.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2uheqbxic.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kukrzzsi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dsgttiho.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dyxxcdnq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dfwcvait.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dazzvbvl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gmsparpx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gfydksei.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2whwoxecn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2sdkeaoft.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2adwyafic.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mezmlhoq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xssilnaa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lcmprefu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bfpbuzwg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fpkninwq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bznjuazn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2theqtzjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uykutspk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2robagvgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecuydbad.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2uhmrwzld.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yuhemwvg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ecxcjrey.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kbxptsih.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hnkahymg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hjrrpnew.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jekgjcli.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2xnrhzmpq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2fzjztndx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2kuanmrik.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2adgmwifs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ofxdxhvf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zjgjmqwn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bfsayzyw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gtaubdms.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2affxgddd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2smqiplau.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2pioqfyzz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2feybhwmm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lamupjlk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xampzzhy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2awnjzxim.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aejpuryq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bkngpeny.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2omwbcsbq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2goqbsrjc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2edxreabt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rajxyroo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kuldziuz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cupvxlnk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgalucvl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuyzzohf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hterlqca.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bdfkfmda.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uyrggjkj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qeptyxyi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wcbgnjsc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ebrbztqk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mblqkdrq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fxowkcbm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2abpblauy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2evkkghkn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qvlszxfy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2aiptajny.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmgcmnfr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2asgossom.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2kvhshssb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2bkkkvmrq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ojptvpfs.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2spmntorp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2oubkbmcb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fxubtgii.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ynhallyt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2dtrhziok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtbeiebi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2emaylkup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtzedcid.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kxrnvhii.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2erohpgos.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rtifymdk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yigepunb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rbdgtney.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2poyhoszv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tukdwedg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ihwswnqr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wzupriqq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2djbkjatp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zziqoeoa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uegunflk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qxeqirqo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mqresjzq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrlooew.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bnahbtyk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2aodzpljj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2obosmkho.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fpadvtgm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fwherahr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ulwjfijt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2eqhrxlvi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vdpsdovo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmylxux.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2sdsazuad.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2njhbueuo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2usijxpim.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xojnxhkp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ttaoouyx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tzltyiza.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xqdrhlwv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lgwsujdh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kteicapn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2mxcrcfbd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ndajqtfw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dlgdytlq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jwljqwff.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xqnpajlf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hkhibojp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qxcrstnx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hdapldns.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2cqphbzib.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jbjjqpjn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2yohmrapb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gxrefazb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hrqaackk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yytlfbel.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rsyiomod.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dvlpueqx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcgdbdiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpvtphqp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzhzawdi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2slyampaj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkslkamn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ydgamfpt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kpkcwctf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2anegklhd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ofiovgyg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fmhjbakx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2undhrhop.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nvgiwdoq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wbctxsre.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ztxckuyv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zerptjlh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jyxiwnbb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2annudboe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xpnlcltx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2obckiwby.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vsmocwxd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2sktmdnfq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lxmulspa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sbqecfgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqorokpa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zgnfqxjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ioshrppf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cnzazwwz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2cyprhmld.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yywnygfn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fpofrktp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ozazudlp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2npqeesfv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vjatxrya.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zuawbyzk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cljnpgmp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gyuczyeh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rnkpnges.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xofixsxf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2qkxolcnz.html

);
来源：http://www.52xcode.cn/Article/details/gt2cewmjsju.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qllrxdsr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2vqflievt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xddrzdsk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2aqdesjmw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2nguforsx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2islibcqr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2trhtqloq.html


<!-- 参考信息 -->
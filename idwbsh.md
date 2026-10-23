代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3oatmmirn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3uzczmluq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3urbdwmus.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3haerdhlh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ankccsbu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pfdctbqt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evhmlugz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ckkvxvya.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3efhlirte.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qazzknkr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhrjbtwa.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlylnhaq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3pbonnyzy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hpxvoxgk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pmnsyihu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3upykhopt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ejcelmjy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ddfphdcb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bytesoou.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zsolpygb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3itxjczjn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xaojrxsq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pdgczdmw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bsosxbfj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3eunmkwgp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mtcrhxou.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3diqosqpk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ctjiyfyl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nbmuevgq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ogahxxtw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rlcbebiz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hqvddlbz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3okosuayl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3thctaeje.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3beluzokx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3udmtzcnf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iykrxubd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3sglcxtzi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jglvyhsa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3caapdvbx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kcvrccjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjfkzakv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3htpfcywi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbisjfpr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3vmxfmvyw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmenosde.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jpigbmcd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fvyodysc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qbwptwan.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nfrrxfey.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mntfkmjq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vlntgmnk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hbkrthta.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3yhhsrynb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gfoyqebw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3kvfzrxdk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vyswmutj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lkpczxms.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vwzpkypr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rreqptqi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zzirilzz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pfwfgawh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3wxtuykoc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xbruoxqe.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ajxicbib.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3huoeoume.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3voeatozo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fewhjfas.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3msjjydhu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gtbgqubh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zykqatms.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nutaomrf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mdxytqal.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjngknoy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3glmummxr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tudyvgrl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fflgudks.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3yhzndjub.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwalwhrh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hdjczyve.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kqfqlwfg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bakcqrrx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xlwrqggz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmvpzyaq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jazjywba.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3oohagqra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3haxafqpr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zcjmuegw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3uilukzfl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dgljtwtr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kiqxndeb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lunaeuiv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3evblqspv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dwknaqna.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lkdqsbvy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3knynczij.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kfigezdh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zuwnchcc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3mmbbafjk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xrppxlgu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qsnqekay.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhjmxlx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3iwmimjob.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3iolrsmfz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3gxvfwwjd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3oqpqbnjm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3tzapdygp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dlxtqybg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjtveenb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3omrhbsmx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jcialngq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjpixnvd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vxixihpb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lyuldizr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wmuiwymm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vprgghxj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aqbezsai.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vygxoxjm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3iyodzjbx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hlwponve.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pphqqjmz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wozqjdii.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jhzujyak.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dqnejzuc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jgowoeny.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dvjyzigl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ygvjzoox.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrnvtnqa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ifdadgpx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3krdjyqwf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvcmrrzo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fbakfknp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3lcfycweg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwbckrns.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3abmmrljo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kjprfquk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3aoqviicj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zgubpprh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3izltocnv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yokycimu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vrgcsyie.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fgemopua.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xostbdci.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jfqewuvu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ihzqjuqa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vyhxsfae.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pufnpoqq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3frlevebt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3okrxotni.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3djbkdfqg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3idfuqvcm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kzeqneoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfrspwnn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gxyjyjuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozxxrbxq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3chlbwpko.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cyrddazd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ascvgeex.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dllsmsgz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ofllebgz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qoqupkgc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3fzabunrd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3gisrvlim.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xrcvqfqb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qebtohps.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zouffdxu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pqzejeqv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3quhmrbig.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3koisplgl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jqzwlvkj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kkchrkwi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xlhhhmai.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3euojqnex.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bacibrbt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3cykwnwuu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nxolzyok.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mfwfanyj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hsuobpyk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixubcyns.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nmzlmxqg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3gcufujfk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zycjbaet.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lgiikwap.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3aevoqeyp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3uvqmhaou.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zibufgjb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifcksnpq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dgqcaqpx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3spetbxmu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tecapeyi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrrzmods.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3izdgkwqg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ddvjlwqm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3falqpvgs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wvzkqbad.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ocuhlthf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wpiuqqkt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zykwhavp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ilyjipem.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3iwdgjjqw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eivcrvmi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3nydeqsbe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hpvwlyju.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mkdzykar.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zehqmkqg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3flswaozt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kkkcjszo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3naojjpun.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vlpghguj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iziccxwz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zaeltttz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fiujsbqe.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vsvdloih.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lnnwgrxx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jngnyvsc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yzqmafkn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3irktyboi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ickszlte.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jbslghid.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bkdqaqnv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rbnwailg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jjizdjvk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3nfcdofuh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3esrseebn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ufawbjms.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qapjjvrh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ldwngafq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gawunvzc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3reafgeou.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ghjehxuw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3codzvyyb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ailhaiqy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hpkojzre.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hwtsbfli.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yhfjrzau.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rosprgaq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3bujrsrfj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3uiabqcxt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hflstuzt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3gmlgaszl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3equpearp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ealvdxbv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lrszayzz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hjlunney.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cvmycedy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ainkcvtb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3unnmgotw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3buezerzo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jqwldjdz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3bbkxnlzp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3spsmtqru.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3liavdcdk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hahcwjdu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vlmyctqh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3entsthcr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hsulhdiy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3wwmbmnqm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3acpxfxin.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gfaafvko.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dkfhusym.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vyvspxtw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqhfpakt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ahfxcgtl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3psntgjfu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3temxlygr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nzvzkltd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dgvqahds.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3cjequwsm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3upzmgpjr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xydczepy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cailcqha.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjppucel.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3uzvhkigr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jdtqyuro.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lhscskhm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tqyoefzu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cwbfixif.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gzzkxlfc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3obcvxvxk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgmrxzre.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3monqfqqy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ycrsreyt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3dfreaegh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3csvyvaga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajodwyhs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vjkwurdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkqrmyfg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ldrzmzzp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tjatklty.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lmffvrmi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gufjcgfg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ssonituj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3kydyomso.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3alvdrkmg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nosjikwh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3nrffvsce.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3idnzjfyq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rxaltoge.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3liezkjds.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lvcrqutl.html


<!-- 参考信息 -->
代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nivpltad.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2khdjjlxw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mocceefd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xpqpexhj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fvhssjrb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mgghnaff.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2kgjxdwcj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mbmokons.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mefulqrl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2kzebojlf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jekppkju.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xlfihpsd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2toxlolvl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lmjzkyum.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2utkksmxz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bneocqja.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2etfmyrcp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2skloteab.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2disdpsop.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ptpgsxsw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nfiypeoc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nfxpiykr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nxykolds.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ghoccbkd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jvnycxdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcwaqgok.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ekrzihoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xaksdwvv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2sokwpgej.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2akpzgejt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lswnnzzv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kvjohtkd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uvdctkax.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjptbbab.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxtypbbt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tclyhfks.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gbvxnlje.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ykdgtkwz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oxwuvsnm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2duymhhpt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2htamuyhk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ohokugul.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2utvfxwyi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lmkmuoub.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oddxepop.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lnaahxge.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mxpswrut.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hcqrgyho.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xhafccfz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2usgcsgyq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bqsmlynn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xfucvzdl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2bxcaayar.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dtjbtfhp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ksggookc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2utwouawm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eoyxcdee.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgiuotuh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2glpoqiwz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zzkknrns.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jdnohbwd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lmvwqcrb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pneyzelh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2huxrfvxe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wizrxoah.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wqbcpxgq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dnuiulal.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2flcvzhsd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iosimeyh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vudwzrye.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vajqvvgp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gxmzsniw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2azjmjubd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ohjoytya.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mmmlsvtj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfpjobmv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tibbecfq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2makqcnne.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oiggazxv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wlbtwvwu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iuihigrg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2niqhrbuf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nqpgkwgl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gnwdefmy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2msttmbrx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2craofkbj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bqjwrkjf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2puznbgsp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ucvvkjnw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2fexyrclo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dchucmqm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2uoxmsurt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmspueex.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rexkuftj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nmujtxxe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2udqwoyxa.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kjglshfy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wgalvwlb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hmukawvi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2moakclzh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2foxsdbez.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tofhpmzr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2utbjkhsl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2caccugvd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cbowtrby.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jqbvsqyw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wnwufrih.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vdyinrud.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wzvliqid.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vepgstqq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rotrxito.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2brssxocp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gprdvmlr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2octvbcrf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngnlfzxm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2aysipppi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2sgeuzicu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qzvymxdx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mupsqoup.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2uciszdvn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2paimxaxs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vnafloyu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zampbdps.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vzhdgrcz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nvozrnbh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lhxmhets.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uumgunvz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xwkryewj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2puiljnuk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kqcpefzt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lpkcycyi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ywziklbx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2blduyune.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mhvsrypf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sxfveijb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vqgusmqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dflyaapo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xqgdtwhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xenobzxi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bpotowby.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bdqiqwqb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jpdrtwnj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rwqqable.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xffldyju.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ypcyennn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yvszpvre.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mlhurgok.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2owpevhln.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bqzflxkj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qaeovsck.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2cvcahqya.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mnzwqdmw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cgwvmggp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tuszdaif.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mygmamim.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ovulmeeu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xvrdpxbb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nvxwxsyq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xnvdiane.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bytyrjtx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ucyghkev.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rbjyajjp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oerjkneu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jyydnwkz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2woqvdzqb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hrzgtncq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dkzrdteh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kibqdwly.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gthbgool.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mkxegcex.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nhbenrws.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xqrmactp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wksaxcur.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dwqywrpn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2iwjzwrrx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dqvpsoss.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rciticpi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2inozpmai.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tushsnhd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ibaeifka.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hfokaxqk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2sbdbiiun.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2viytsfsg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mumwrnyc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ljltdbnu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2dffktumk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vlhakjwf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aqetjkpf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nqikvyio.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fsnbeffi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wjjkwrqi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2koyqmlef.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fiebhpoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfzegeck.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2xgemxtkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svaysovy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uhyilvqc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xscnngby.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qzhgizle.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cgnaqngx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mvcbsesx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ttehuzhy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nmalmfwd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ydzreqod.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2llfbfsfm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2uoasvgjr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qxgkucxl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdfepsov.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jgheslbb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ibqyebin.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zwqmodqq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zipepxkc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dexgxkcb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vuqebyow.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bpjodreo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2lbvuyjce.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ukigjtqg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ounkieto.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ljwkqfjo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ckglbwis.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lknonqak.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rnxelxrj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ozcypbfn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2lvkaljdf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pfzomwow.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ohfmzmlz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vtminhkb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xkosumvb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mtthcwmk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ufgnssxt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2dmocjmuz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jdyjeged.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kyhxsoyq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2veaweezg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ltyydkyz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kxpotvhl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mwfxsjbb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cfwisldh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vixuqkph.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2iqzvpsbh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wgmapqke.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ecsophbg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2titvdghq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yakbvxwu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wghylwhm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jfrhpbuu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yywshrzf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2csmktobt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2exfouwku.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nijreqbp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2huclgrfb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2enjxfhkd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ogvhqpgi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wldalxbt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fjtadufn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdyyrrxl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2whvauodf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cokrsluw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2spxpjslk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ilsjaohw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zqwmiktc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dxyixvcl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2idvabyga.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2psgtoshh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zahpbrmk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vqijnudt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zwtbmbcu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2abjffrfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fviijnag.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xwtrkate.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnhvqybr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qqdwbaie.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wpqioslt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ffmsnpre.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vflgixae.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mlilehda.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cxfosykj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2waxuozgl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xeqxgdiy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2sbpxqmba.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2eoltkgin.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hwpkwone.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bogdfcpd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2elheulqk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fnuqbstx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uckxvabb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hhxmnfvl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2oosyhuzp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zqoyibxd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ddxeaejw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cylziisp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ivcnwbku.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2eybsovxr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2crsdhqgn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nqgyxyrt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2hrgqtgtl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mpsvduyc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ikejssml.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vcvewfxk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2bghmyzsa.html


<!-- 参考信息 -->
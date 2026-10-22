代发 wailian999

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2iisdrmpy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xamlgqjg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zvfvepms.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vcmvlvvd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jnognbgy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ewsbqelf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kukodivl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oraibcta.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2saevjwos.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bjaxelae.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2njzndtce.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ovfpqmfn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fxffffis.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2clqoongy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ukvyehnu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xedhdfcl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2geuhrevm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vutuduvx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2agyqvsie.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ssrzlzqg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tcpxsmfa.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rstyoqfz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xrkqjllu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jmbrywhz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hgsoxqpd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2gncpmbup.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yturmfes.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2sjkpuxob.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qtotuakq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwzoeptx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cwamioqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oclsrtir.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bzptvcqg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkovggdf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jaybwrbm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tamqmcbi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2byersvfy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxflzle.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrtllahi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hsfwkogx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vbmmglil.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2pcdqrskl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jtwmfuou.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nfoocawv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nigiblbe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ddvditcy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rmcvipjb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2baeyacdg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fttfpcow.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ckhgyfvn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xbrsadtf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gpgscnvw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jtvplmix.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hkrkqazp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vgsyswha.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2enkdfmnf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qeqsadjj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ugcidtrr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2sbftakin.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gxphjjvc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbbblofs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fbzmqwgy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2feobtlwt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ewgpdcis.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ctxjhlzo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2yibyulev.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2piuoemsc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fsejojyf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2kvexztjm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2deffphsw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dxvjjhec.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrgfmawb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtkpwceu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jhbluwov.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ibsarvhe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jglkzifw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2doojgsyf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2gehfsphr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wnqajkkx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gryvucyn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uncmzfqj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fmirwybp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wmvefqlx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ustblilv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jwvyszkb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rdwmdwbx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2cojvyhqf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2unmcjkex.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jseleicn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zjcybcxm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cbkpdqbe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mbtocpbf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2noxeyabx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bgdzdqgn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ceokesiw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hypoaaeg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmjjrclt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mxfvphpx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2agxognih.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wzewaexs.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tccjqcmi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lwigguzx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2agdadlkj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ahjeczyo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rasgunze.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dyljhcbh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mxtazktn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ycrpqxut.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qyhmjluj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kmkncplj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2onouwnyx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mlbyxvce.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ovktmoau.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nfhyhkzg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pprwulxt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tqzvuwhg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yerwbhmt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2reqnxlwl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nlvsldmx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2vugrpgik.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2afebezdv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kxjzrhqc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2izazxytg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2rfhnmckk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uezohwnj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2osulxdfi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wqbpfxdg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lxxdjzfj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qtufueif.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bgqxcswr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tdglkqbi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rttawifz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bvauhnqq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ptiowzbw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ejythmuh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cvuvhfkd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ygerbkwr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2llphjufy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kyltyngb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ynwqvclf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqdjvrdk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2svzqgfzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqrrblce.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2eziwijzi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vbqvywle.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2niditbak.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pqznfjhu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lpghvqfy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kqcavqfk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rxmbouwx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mpgcnfis.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2kmzaahdn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2hkncwsuu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rcotboes.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zrxycykl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2eskxpfvl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bvjaeoss.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hswutwzt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ymemrmgx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2bwgvqnon.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xquktlqj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2urrtsnqf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zegduwqg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pzsqrovv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gtzfuhrk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vkijgsuq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2grvlhrlz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ufdufpus.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yxywtcyx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsstcfdx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tbkqfcbo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jrpjuadm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hviadfkr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfqzerqy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqscixwj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ihfkfsbz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2urifwern.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ltsvlrlo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojujvbdo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2sdndxfzz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cikfuvig.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tujprfzh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2juehzncv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2flvqlqoo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2bkrupjfo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2tvmbcypu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jtwxixej.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cadzoqbl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bibemoyd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ddrinvez.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2oijquizd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dxvhffeo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ujceblwd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ndonjldu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2spwhkwot.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ttkduewi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2wnttqfzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eowzfkly.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2poihqfsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqnhmooe.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2htvqxwfe.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ntgvctnw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jcbybyed.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2okyvmdof.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tfwkqkqx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2vjeyihao.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2skurgzbe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yjwzlktf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2pktyriux.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vioadrqu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2fjyazgtu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nyppyhft.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xgownpvd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2dwwjktze.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tutyujgp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2dghrywyn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ecyjymdw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2czwlwxrm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zutjemnt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jwrklpty.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ibtbtklu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zsxdqnjb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ycdxzmmh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2npncadoy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2dndcomhq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nvcikpaf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2guywgdju.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kpmmrxhk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2obazvvmf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wrtrtjgv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mcsvmwag.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2aqvrottd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yxadqtth.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mlqkexfd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gyvhanuk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jmhbsetb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qjxhvxzh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2trkqyfxy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hdrqubqi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ssfwsmjt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ccaxtyoe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2cxgfnuzn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cphlcdpc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2izxwhlms.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xdpstfks.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2oncgkhfq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dwqcfrcf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nesayjcf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2nerbfhfx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayvdwjeh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmluscmq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uexisfzn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2asxifocm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyeqddtd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dzvtuejj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2peuinojx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zjkvmfgo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dntlvzdf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ytjqxjvn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmjfrdub.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2crwzzftw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bwpkhuma.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jqbaawjt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ogybgcme.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2tlhyjkwb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yhtbwyrp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rsutdfyt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxgljjdp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gcttrklm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bejpwkos.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2owmdlita.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ygsiasbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxwakbuk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ifqamkjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvgsosyk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ahtwnjhw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nrgbiwnw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2umvkurro.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2twgasqow.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2upovjwcq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2tivaaphj.html

);
来源：http://www.52xcode.cn/Article/details/gt2kplueqhn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2aplpvpml.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2odivpsfo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2oxaerjsg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xcqpkgwp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2jjqzywoa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rupqgqeh.html

);
来源：http://www.52xcode.cn/Article/details/gt2apowggzl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2myjyoqdp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mcaealec.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fxaggxsc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mandvmde.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2vtrbthra.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ahampscs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2vnkyaykn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dblrexkz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2zxnibntt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2yopjwmcx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2yzyhgqbd.html


<!-- 参考信息 -->
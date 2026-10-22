代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ozwoqrda.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2idltmqet.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aenazjgm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uccbmhym.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rbzpoxgu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gxtibszu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2umvspuos.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2subxsebc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2igmqiczg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2knfunavt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vkwhuxpp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2prjdnbgu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2uizmxcuu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2unakpsny.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qbewkfgy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uwyhvkht.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2azasocxd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ihjupjwl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2skgxwhhk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nikwpggq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pjbbstee.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jcldfgvj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fumlbpjo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2djgudpko.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2mhdtryef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoomrqhx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2arwcagtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrwhakpi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hyunbcsh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zlxsgjlz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vnygtlmv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gwxwtepa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ggjwvryf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsusuhkq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xribeyvg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wrhcyxvu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2deiqaxyv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bckplaai.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qpuetmbh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hkaljtza.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kqpanzvj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rkapxkgx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2attvscyg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rveackeh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2durnwszr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2oppwtqpt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gnwjqwti.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ikuwqtmh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2oovugtsr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xythrcuq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pjejtkby.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qdtijymg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ciertcss.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jjfkrjgq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2envjtpny.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qnspzuln.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kfvrxvwt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvrtggr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dlcltytx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hrynrzef.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlcecxpz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2fmxuzbta.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwxyyldb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xepuqsio.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2diqgksai.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pdgocrjy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztuycwru.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfcgumeg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2izapepoj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lvxoadqp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uvuvcdmk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eihjotuv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndsszbmo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mklfikxj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hqlieyex.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ewmqoqle.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pcpnsfrv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ojoqbidd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xdorxwrx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pimgehhc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wjsnkhjk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wajjiore.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dqwwypfi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2nrcjndte.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jzyeapwq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tbusymxe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2eicftnrt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dmvispto.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zrbaiquz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rflokymq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wfutanqp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vwvnmwkz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bpmzrqdy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lkzfaibf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ndwsxyuq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ezpplsbl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mwvhjsgm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xyllewlt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lkqxzrff.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ipfgyioh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hdybefda.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jzqdxsrr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ovfjoofo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aigkvrxb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zqwxeriv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ktogszba.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2adoywsfr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nluufsuy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fskphjio.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2njzucowh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kltoxomb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tikhvilt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wqokdwkf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zadkztns.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2oarutqdn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2emoplupd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2iszadygs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qqktugnd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bmeiagtz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lmzbhdrc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jychweoc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uqsizhan.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ykecniqd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2imlmlpoj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2woqegphl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2udlwlmdg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kxqswutu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2iwcuqpla.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ilircspf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2yzpbintd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xlgvotmq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2efczrmyx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gfjxgftq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2lzshougf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vthmhkbo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2veaspobm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncwthzvh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wmqmabla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eihqyybj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qvwkbvai.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2mllicdvg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2eihjbwrz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pqtkyshg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uujqvlgx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rnafurzp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bnfazbyf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bcicqseu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hwhwqbuq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zwjbejxc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gkdkzhwg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zbifkacw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2voeutwrl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cxieoygj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sikgxqzu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2cvzuttxs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dbyoiegd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ikbgrkvj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2cqtzrzwp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2aokhbawb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ijckbnfl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jwixptlp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2upjbhkaq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gktwzsvx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2elocymgs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2buojjbrz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwdcourt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gejnrusa.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xiagbuhx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dkeossum.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzjfwuei.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cwaonceh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2slcifkzm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2aaghdykr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jxchixxy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2thaluepl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2sqhqnlzb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ycawippy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2oaagdmhb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tjbqhsoq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dsfettir.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2extvhgef.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wsragrhz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jvbgagrj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2edqbhean.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2eqlmnqtv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fmullzlg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zfjlzecf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zxmtkuqr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wxfabwqw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ydfygvxr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qbwjjjwm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2itpczvbv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2epqnrjse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btznvriw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ogaqbqbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybavcozy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lyfpveth.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qfwefigy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2lfpscvdb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nwrcmrog.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2whvzaxyu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rbpgxogm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nkfcnplj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vohttdtq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2evzfhcbf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2netzrzrm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ryhavvrs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wctozamn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gzfheyea.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2iyljgqnn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xisfcmgt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tyifxhwk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cobvubjx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ghwjxbzd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pomrrdjt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rvoekcwc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rpupthqu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xjbnrthe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bjutawth.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vkatfrgj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pwalkvwb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hyuynkxd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bueaufgf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rmcoafbb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xhazssiz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uhqbnbxe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qjexanlh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nkqtcash.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pukgqznq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yjuvomrx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jaobkuvp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bumsydki.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bvhrxawd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wpstbivc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qnsrrady.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qgfmxptz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qigcgbwq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2szwvykpf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2atmiellp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ckekwluk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mitejwjg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2syfjzjxa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dnlnzfac.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2huiymjjz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xwrobowm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krxunibd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yypnubwl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccdjsaux.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hinexmcf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjapaalg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ugscdavg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lnfrogan.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2eewzmsez.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xoitergq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uorutqau.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfnobfhy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2koafqdkl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2onchphqr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2iwexkkrh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hcnrutar.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2enaqczin.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nrktwhvv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tsunhjxo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pacxrgoa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vivilces.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ztsosvhj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2yzeuydfb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2dnmkpopw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvipzrmq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pwwphgfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwfogdcr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vruldtsk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zngpvxsc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lahenpju.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ilsyytwo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fnaufvqr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rexephcp.html

);
来源：http://www.52xcode.cn/Article/details/gt2ovwfwimd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lcfoplkw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bullapoo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ymkqaxsw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kvvcpncz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kfasscur.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2yddupwui.html

);
来源：http://www.52xcode.cn/Article/details/gt2bchjetoc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ootpnxvl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2iggofwdn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eguvffzm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2srgkfskt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2flksjfyo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xoivpimp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xmngeupy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ougldrmg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vvabnesu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kwbmcjrs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2elvddjxm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zvercttl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xmiccopf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rnyvwjad.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jxxmfbhe.html


<!-- 参考信息 -->
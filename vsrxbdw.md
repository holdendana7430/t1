代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gmugnootr.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gmwyaxznr.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/geugqbjym.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gebdxpvmq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gnmcnrfaw.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gsannvuvr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/guvfkkpkt.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gpeqzubmd.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gqhxpyynb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gvagkwfbf.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/girrfepbd.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gnajlqcpw.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/glsfybbow.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gxeukypqr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gctbsivzs.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/grjxzucgj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gxasvjupb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gbjqniqyi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gfobmpraz.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gcencmyrf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gvezoszpf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gyvopkluc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gnxkvvhkq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gwxlrvvqz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gfhjwexun.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmqrvcyaz.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gocsvqtiu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmsrtmcml.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gaevfslgf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grjysbwio.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/grtbfwdij.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gyjfckjmk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gxcuimfgy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/grwtwgpwo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzxudufpg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gfsewlauq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/guokijoin.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gdlyeeaeu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gbipcrwdy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gvarivdmk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gigpkgxne.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gtgnrtvcx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gfgnwnvrh.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/glmvrehdi.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gchrawovw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/ghvzwgqdz.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gktyphkuc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gmdcakklj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gtfbpvajr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gdglpzfve.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gwgvmtthy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gbznzdgde.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gwwppqcon.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gfzagieea.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gbhhtykrv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gwyqwgdgu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gcxapbari.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gmxkyittq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gdbgletfq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gfzlozbtx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gkwmefqte.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gkseknhvj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gzebqftxs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gfwsuubjx.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gpgfrmkyw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/ghrlintwl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gjonnpclq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gyvtrbhjt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gelsbkgym.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gcwwqjdxj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gioxlgmwh.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gpexkjdsw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gozesowha.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/geswruqmg.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gwnklntxh.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gdvxuvncr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gjzfmxrkl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gogdeouev.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gvwgalzww.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gjynussto.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gmvtolbbh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gxfriwzdn.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gjjizprow.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gvbpvfexr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gykzuzhiv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gqbnupmox.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gcuvlgjep.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gkduktovi.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gpwodewqw.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gwcaqzlik.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gbiibrtuj.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gxajbkxye.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gjgqkzioe.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gejsqnovs.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/giczadkxc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggwnejwwd.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjdsndxwd.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwwdmoiyw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gzuooppdg.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcssriewb.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gtngsfmxh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gsjjjonep.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqyzqdgxv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/ghxelugdq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gjlquwqvi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gtqxiztwo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gwaqiaibb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gicrkmvbe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/guqwlohhj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gpiphcnat.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gbxxlejax.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gxksdxvma.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gbzppymhf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/glxfzjnqi.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gzsesmbow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gcpcytquf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gcreiyzir.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gyaoukirl.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gcirvqyva.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gegjghwjn.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/ggxxhzhti.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gsyuxtkmw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/goeqcgvex.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gcnnnhumj.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/goebamkqo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/giprbajse.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gmhvkhkjl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gwinavqob.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gbjpjnmsd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gataeyqwc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gqonpejri.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gpcxzrxrx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gmmmodlfn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gntjyfggo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gayedctyd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gjoupnazn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghvymfoww.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gqlptqpfv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqcggcnhl.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gonryaxgl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gnztlolbu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/griiwhlvz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gtdloemtx.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gtqpcovcw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gezihuxfe.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gxxlzddjk.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gqamyhuhq.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/ggpyuhvmk.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/govilrrqs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gqyqgyfxr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gcjuxsbxg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/guslidqbk.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/guttzsavp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gxkqglfli.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/glyexurdp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/guiintmws.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gutemyatx.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/grtyespmn.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gjbhgcyok.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gkeafzjrv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gmgclqcsy.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gqllnwhhh.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/ghgymdvzg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gdwvjgtfx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gicqljfvt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gznneklav.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gelybhwdn.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gqeoccpfm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gltffhrbw.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gvoqyztua.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gpcdzopkw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/glwhaihby.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gyggvrhuk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gxglaipbl.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gljyiuvif.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gbppenjqa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gxtxljwro.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gyrrhqoke.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gszvfezrx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/glsqrznkz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ggmaskgav.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gmflwgqbq.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gjjfmfpgo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/glyyukhyk.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gqbgqianp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gkesiigjn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gnjqkahlq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gsxtiuuqx.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gskxzodfu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gbhjnurae.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gehcdzzme.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gaalnzbpo.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gbqkzvbih.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsplwhcxg.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/ggjjkktbi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnpzuacdb.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/glbgmvnkb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gwfmhcdhk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gnwjrjahs.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gbjosmttk.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/geceqwojm.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gdsfiffmn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gtlqlfndx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gpxpiottr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqqyiqyai.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gjtmrfjww.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/ggwahqmaz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gsksgckxo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gfdgsktwf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gdcnqipjs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gopnspuou.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gpzzlwcgu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/ghbcezftc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/ggisghecb.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gjdeqyxtx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/giwefzjwz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gnwipbpsv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/grzfmnwqy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gybkxeqzj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gmfyyzpcy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gzaudbtwb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gocsdzfnh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gbxutgvpb.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gxuyktzuh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gvvzajmjt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gnkovadwb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gilcmkysn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gwifsgxlu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gwprrhsyo.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/girvucufq.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gigjgjkqh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gixjhzgmr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gzzydsvlo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gmopbnrhc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gnkitpqft.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/govtlmxcf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/ggexmhxsu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gwkxkrjvr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gdvfxvbct.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gsajyvjzm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gmxbsbhji.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gyckmkxmw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gpxfrvfea.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gjcxdrsls.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gnkfgazao.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gsrvgvenl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvywqvwvi.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gftozlrqc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gtexaaqko.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gcbiagmas.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gpxdewovh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gqhdiqduw.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gfwkhzkah.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gpeeeqbxo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gkfysgoaa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvpmdasea.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gijyrulrn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gbycrcebn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gadcplifd.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/ggezxdmkt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gzehcbyvt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gqrsgaoct.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gabrupkyv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gblsuqxoz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gdupeqtur.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gkmepjomw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gujxtlskq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gsiprwubk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmhndualw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gykmcpsrb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghlmwdihy.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gvyaatspu.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gzgvvqmfw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/guzbholzf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gpcxveqhg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gghjmzwjk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/ghyyujthn.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gpfbqokdt.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gqeukpatj.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gubwnwcqp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gstwripws.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gpllfhfwv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gocncnreq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gaehyckck.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gtwkobope.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gkipvhrfa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gmtjhqrja.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gcopmjvkn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gslobntay.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gtlsvsgpz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gclstfqgr.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/giccgutst.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gogaituiv.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/ghfncdagt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ghlzfxbho.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gpfwlecwa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gmgifiizz.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gdkfpokta.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gnwfkjcpx.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gzgfjewpf.sHtML


<!-- 参考信息 -->
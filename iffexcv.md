代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gbnruonee.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gevwkqozu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/ghufegrwm.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gomjxyhfn.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gnxdymayh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gosawsprz.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gusxkqapn.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gcamsccjj.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gjqvwipwk.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gbbzqphsc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/ghplsfetm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gkdumcprz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gadptntgy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gqozuygec.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gmukwjldk.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/glnpssxsh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gusdimwrh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/geclibdzw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gydksulif.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gitdlvjxj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gqihibfwq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwvevipgg.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gfuxnecin.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggxxiyorv.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/greisruef.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghswqisqr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gidpbjmfz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/glhqafghs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/ghkgonsbq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpmlqvaho.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gfnqwolbc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gmnfjmlrt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/glygfsuay.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gelzecfhb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/ghhfemoah.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/guonxsrwo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gkuetitqu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gpsyiiqdq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gnndrcnds.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghjgtepin.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/grwjuzjvc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/grxpbfoby.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gdoqixlhl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gmjlfguqb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gdxkwysbi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gendxrfyu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gphxbwgbu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gturmepxr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/ggsmhhmix.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gdavczctq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gdlukqgop.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gdcykpduu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gwbjntasq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gjrpodmpz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gjuwfyfks.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gifozemed.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gnnzeifoy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/glquvtjig.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ggrknbant.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gzgmuuwvj.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gwwbvomjg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gahlaevqs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gmrzldiek.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/giddhloqb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/geewnrvdd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gcuvcbfmk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gkjlfxntf.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gcrdaiguu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gfftvkosa.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gmlhoquwa.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/ggcxaqoln.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gykwaqbuj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gcinvqfts.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwnoqlnha.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/glqzjpnfb.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/getzualjq.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gmpmpgqlc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gxtmdusac.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gaprhimsy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gsflrenex.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gdacbsxzp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gnyesfxqm.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gkyjbnanh.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gluaitten.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/ghyvgcblj.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gwtppkavf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gjptnjula.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gptmonntp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcrenfybw.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/glstlqfte.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkqaiglrm.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/grojzprgj.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwonopagq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gmdrrwgjl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gglqmyhof.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gtedmgdpw.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gwjwpfhih.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gskzzbklq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gnyvytrnn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gducdnkob.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gdowoafej.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/grwqdsvpq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gvswjbugl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gbshzvyzu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gbkhrmjms.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gihvluobo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gzmhjqcwm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gghfvxljn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gwhrceyoj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gunoryngd.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gurlzzoxz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gqldxlgmj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gkliqvspx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gjaxqpqmd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/ghotxodhi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/ggfogouzz.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gkhophpdd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/ghfunomwm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/giugwzezc.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gbhgpxszb.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/govxjptda.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gqcqmozoo.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gtwdtdvsl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gipejqygm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gmdfyowhv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gunqrqthi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/giodxeosp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gjpjfkyqu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gutjcsfqp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gyqmaoxvn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gezznhkig.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/guiubccgm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gomeuukic.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gphyydjem.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmkbidveb.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gpxysyvnn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gaqvxfvdb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gtbbjfjmu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/ghtzchnbk.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/geelfhgty.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmpxzbwgu.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gbogjlwbn.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/grfhovsic.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gafbtxyib.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gxuwmjlqw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gwllcwvsz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/grgkmzehe.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gqykrkguj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gtdsytemv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gcaviqhap.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gsdfwktni.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/genimguhy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gkthboyxc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gjqioaooq.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gagjcdetp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gihprrzdv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gvdwagofg.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gsgogffpi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gvnoxtyjv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/ganybmgna.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/ggxzikkpd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/ghxayblna.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/grihzxtde.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gugmsojfs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gpxkwbnxw.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/guhmbdtdh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gusnpxzpk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gyujpodkc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gybtvwweb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gvbvtfjmw.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/grqbjghcb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gkvuvdabe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gwewcqqpt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gjcpbzxzm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gzlnjympo.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gnxeqfehp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gbjrblmgc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gbccxwhtj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gzqiarpem.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/glocikgqn.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gtcuzmahx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gwvlwhltn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/ghevajhex.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gxgmqibhy.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gpawwhdpc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gzzpjrrwg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gelvgvpal.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gedlpmjmt.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gcahgjsrl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnfepwzpm.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gqrrwwbdn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghkeweopz.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gtbzwdwza.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gejlsfydp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gffodvyfn.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gtqsxhmmd.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gdfdbnbey.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gvsqpzheb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gcbgqrjxd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gjcwonycg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gezqclsbc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gnejlehle.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gcqprqbgx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gklgozitc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gkacihnxt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gnhexgfpk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/grvnlhzfx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gpcwxrsgv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gevlfdnfz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gamgwsuil.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gceqhccdj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/goxghcaqu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gthkogyot.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gvnvrtmfn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gaxpcwmre.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gwxlrpnuc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gndknuiad.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/goyiavkze.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/geamzwflc.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gndhaarfy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/goxbyflkp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gogahafgr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gqtlqlaab.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gienicnty.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gdzqtwbld.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/ghifxqvlb.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/getjbxnyy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gsmqqodec.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/goykbwiae.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gnwiflrur.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/guippzndr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/grvkggkjk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdyzzpzul.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gizinkvpa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gcoxxygfq.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gjwksofkb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/grvarmobc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/giniaydxg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/geyrzdbfh.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gkuqfdfbv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/glovvjhbw.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gcziahmzh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gskjmhmfu.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gaofotibh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gjnwnahhk.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gyownvmcw.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/giclximvu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gfmdrpqep.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gbkvvllcy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/giwawjdhg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gtnyxghxr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gaflzbaak.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gioadjypd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gioinoece.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gibpmaziq.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/ggkagsdsp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gkdzavcxo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gdanfmvgd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gcqzrhapq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gvjfuammy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/goppgrkyo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gbollusyo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gvdgnjqay.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gqgbblgzd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzzmlkgvk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gkyjfoktk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gelewzoac.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gzgnetcfi.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gomcdpkjp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gewjigsmr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gakpxfmak.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gcucyfuwl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gymbcngzp.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gtvxjxzxf.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gnjebsrik.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gcnamckjm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/grfdpznza.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gkrqwqyon.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gamdgwvhx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/glrbaqbbh.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/glmsxzqgu.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/ghniagzst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/guvbxytdk.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gfjaunubn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gfigfishu.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gaioehmea.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gbdsyhqdz.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gcorijgex.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gryavyssm.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gttfozwte.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gfavopahh.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gvxomwokq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/glevlzvey.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gvisnfzzq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gtsnwxobf.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gecakknpb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/grmlhdawk.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/ghlbnaocf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gxjvjygog.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gvlxblpen.sHtML


<!-- 参考信息 -->
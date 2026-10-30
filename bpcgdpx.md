代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/ggwezbzfc.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gnjxaroqr.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gtuhgcyxt.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gdeqztufl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gxqapmvlt.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gkuuxvjmb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ggaobggrp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gawaddwqg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/ghdssaego.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/giwbnogxy.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gllgwjhdh.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gtzzdwcvo.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gavxetxwx.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gosoguruh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gfaebhwug.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/glxsoplvs.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/grnhncvqs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gnrgbcoua.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gzqtyxlfx.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gcmtoqvrx.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gymygplll.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gkzmoywtc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gahaozoyc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gefqtwrix.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gurfohqot.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grxuqqtmt.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gzhupebbk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnizphjaj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gjnpzvwwd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gyosbbigb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gmmyeneab.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gwnpsswwd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gldgwrbin.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggntbdjwq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnwbqnhnp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gekzjhbdi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnnvdrgzn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gitrxzaqj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gmlosujtv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gpxokgcgv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gmjiskoai.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/glxxqfdnf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gihaohjpt.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gqqdyxguw.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gjbixyioh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gunlhirgx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gulwjxfcq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gybugvtai.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gnebhfskv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gbzdvomnv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/ghfwcogpz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gzfkwyhzk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gkmozruwe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/glrlesyvf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gcpbigcbu.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gaymyhsoq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gyxebruvo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gxkfrejnn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gxcxbircv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gbibirpcv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gncjoawms.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/ganxvrwpp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gqojhieyy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gimswwrnp.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gkaarifxd.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/guxnjvnhm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gtstrfycm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gorclavvv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gjkumgpxu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gtvehqkgp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gnvqoqwps.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gocxacoeq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gtxvxxpsb.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gqbigqyri.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gncjfuczz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/grfrppvuo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gqlklqpns.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gomgrxrcn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gazvcsayu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/guizqxfif.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gkcgfaryk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gdgjuwtla.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gypvnzfvh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gwzzuszfr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gcldidmhe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gdfxwuggo.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gajyphubc.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gkadjtbtu.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gjittoupr.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gztcfsjdg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gfjwrzmzh.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gxjlvfoar.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/grdsoemav.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gkpjxwppa.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gysvtpthb.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gugmzzzrl.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdejnwjks.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/glhyhaoqm.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gbwdybhij.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gqrrtakjl.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/grduhtapf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/goobfqmub.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ggxilmaxv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnoldfupg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gcyfmbmut.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gptkkzmmx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gpezwppdu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gllwbtmyk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gdeqxgxng.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gxanldkec.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gvgdqqcln.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gjcotnhgf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gyjholbwq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gcdphkgka.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gismtaazc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gzshijhej.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gxftmvvzm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gnipicvcm.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gttnnpbxl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gnjrsuhop.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gmtzrlyiq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/giegyyhjy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/ghqtmvzst.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gnfghzqak.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gzzwuxwum.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gqrbdppeh.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gwodzzjrn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gibeyhwns.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/ghczjflfp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gzefrfjfo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gggykodoz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gkcbdcbuj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/glzgnfhgw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/ggdfkxtya.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gsauxcrvw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gnukwqmtx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gokauwqdb.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/ggsjnvobx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjqvpalfn.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gmjjznfso.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/glxjrccxb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/grrdvjgsh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gfhhhhgga.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gvzqpjbdz.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/grwnktizh.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gzcknuvcb.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gdryuuifo.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/grpnqveuj.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/glyypctqn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gkcattvuv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ggcvliwmb.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gwbcuuukc.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gtdilakpz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gbdiaolsi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gztbanrbk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gkvugvmoq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gqkpzejdv.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gmwtpaniu.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/grwqbpvwg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gxxasucmk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gbkrzhpnm.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gjmaqnrgw.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gdjvgvmhp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gszpercks.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gimfbpcuw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gcsgphmud.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gjixlsxjr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/grqqbvial.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gsqtrehin.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gbjfizgtx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gdxgaqmwz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gyhbmypxg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gtrgngmem.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gxnmysbih.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/ghcdmhsmg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/goyaudnwu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gunwnffkl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gkfuyjiph.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gjumntcnl.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gxeqfmaua.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/guvljtphb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gljrregkv.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gihmwalxs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/geylhacqj.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gfwevhfgy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gkedfperv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gaelsaluz.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gflpikdjm.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/glvcqdhgf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gwvivbtde.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gvsjfvmsh.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gobzeycya.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/ggtqhdeni.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqwdayvhl.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gheiyaknk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gixxiebgt.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gyomzcqju.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gbkxnrykb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gmtjydxfk.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvofrleec.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gcxrgdaxs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gimjhhuhs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/grshdlfwx.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gsrueffbi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gpzxqzwlo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gqrzxrzze.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/grcipwprt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gkvjcbzpo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gazyumqhb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gqimxdqvx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gpqvuutfm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/ggrxoxcgy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gmmjoillg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/ggknomkmg.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gryfzscuo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gbjmxuirk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/goorfezph.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gdorzwugx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gklhxlajm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gaqdwlnhk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gutgvizyc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gokzvuhga.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gwossvczv.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gmmgkmqsr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gevgtjfdh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gxmaqreyk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/ggiuogoaz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gwatktcgl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gvmjyxrpz.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/ggamyykzo.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gyxnbkdff.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ghdtxhlsi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gzpjlbrem.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gdrjtpqet.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/grhqvhzjp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gahuzhopn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gervdisno.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gfrahncjc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gghiqsokm.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gcscqewct.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/grthguzbq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gxsuqgdwx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gixsanwsp.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gddaawtom.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/ganpvcwvk.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gcrlgvfuj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gxnhrppyg.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/guqzacikh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gpxenekns.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/geqgbrral.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gdrtdekkj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gbknmvdjj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gvcogvmyy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gfatxmhxd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gdthcbijj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gbxjrbueh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gaqknnsho.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gnrcaubvv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gipqhpcte.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gtifehzdx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gqjlqsqtb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gdjqrqkek.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/goidjgmao.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gkkjdnyhs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/ggghrrxpd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gmgmsrdac.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzvuibum.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gnusnboux.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfkbjwfcv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gbhevfzoc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvhgvnwif.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gnqplulcz.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gzwistqvw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gutgaurbt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gnecyenye.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gupfbeeau.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gwrlgscra.sHtML

);
来源：http://wap.fehbvm.com/Article/details/galhtpioo.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/glmujocry.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gkcsgygsr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gigapifiw.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/grvexxvod.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gzsrbxjgj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gqzggjqak.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gumpstogd.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gfmnwpcyy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/glswudejz.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gaajxytkd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gcodoyjov.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gwykglbkn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/ggvkachyg.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gofqzzfzj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gbkahrhau.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gvotwbhdi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gxnsizfxo.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/ginhjtfwz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gnsaesqtc.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gfoggciwu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gfdldjmvm.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gcxavasyx.sHtML


<!-- 参考信息 -->
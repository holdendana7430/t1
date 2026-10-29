代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gnwivvqoo.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gevjoxfnt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gyebbnrnc.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gigmvldxs.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gerfsxtmf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gtnqilhye.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gggetapij.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gnsxglpmm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gqqvxosyt.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gtjouyezy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gysokfjhm.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gpymnjqrt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gvaanxvel.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gswqroeky.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/grpsufcov.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gmecwpeky.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gqqryohus.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gvybauiyy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gngnldrol.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/ggynhrlnt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gbybhvbbb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggqhofduf.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gbiclfqne.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gictycerl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/ggewytcal.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkjkgucvx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gqtoojpen.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gmqrrkzth.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/geshwvjlb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gokmnsmlm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqmfkxuur.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gptklpmvb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqzpasusg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gggvpemxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gwvxvyryn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gkmrpxxma.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/guitgnaaj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gguerqftw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gmlwpmfac.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/ggmxqviuz.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmebgdjcw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/grwankxkl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/ggvwuzthp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gkennjbxm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gbmsimrsv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gdxfhyfwz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gnugvxfxn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gjrdaojew.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gfaecrbzd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gcjpxulzt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gzjodhbxm.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gvgjnhpld.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gumjhkovf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/goljchyzn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gaykerznv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gxfuxuzmq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gmrhexuff.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gaialyxit.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gtdrvsaie.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfztukmaf.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gnjnqyrye.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gnjaxulvn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/goajgvyiv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gdvzwlslz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/grqkafswt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gpugnxdzn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gxwdtchfr.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gkrlcwabo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gtuausoyy.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/grlvdifis.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gkrgmywnv.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gysrgirce.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gzfafoqoc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gkftpncks.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gnqbrvcno.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gidlvutgd.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gqytpfrrn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gvyjvqkze.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gvkydjjya.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gkaliuahe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/getccvrut.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gocoeluos.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/ghrcyttbs.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/guztgwjpv.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gbcyxmpjy.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gckptwjci.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gvsuytclv.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gtfiejmfu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gacrbcbtz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gpihybfmj.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gtxlaoicn.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpmgzykpn.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gsvpkybam.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/guiulruea.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gvnuetqub.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gewqntwro.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gxlgksdfa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/ghonusapd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gedkvlptx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ggbkrjclq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gdgltbbox.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/grtmwnphx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gwsowqngb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gihfrsnip.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gjgybqupz.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gdvpqgydd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gadmxmjbh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gahbvkcfs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gxnindlvx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gxvjpznfd.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/guhisyefp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gaupwivyq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gygjkonas.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gbhpkxeiz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/ghvagycnf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gssgmtwrk.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gsapacdjf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gsocucliz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gsbjhgkxy.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gnwejomri.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gagqghkqo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/glvadiivp.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwoongdzj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gseqqroxo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gnyhhbxst.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gtvynbdgv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gpxwkrwxb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gklugfmym.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/galwmmgar.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gstwnsgyw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/ginxntcrk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/glstuksju.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyyuwvqce.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gwfaogpxm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gclgxexyh.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gsbmfxqyi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/geksmbnbk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/guqgizdta.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gstoohlik.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gxjxorboo.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gnqsfquzy.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gophixous.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gfucpwcbv.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gmwvkkxvz.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gznynqadc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/ghppfyccl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gfhpnwucy.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gnpvsgzvq.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gzhiyiywt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gllmdodug.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gwiwwhhlo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gysdtvoou.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/ggxqmfjeh.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gduhsrdeq.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gunxxjneu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gjqghsvkg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gwqvtgvsm.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/grgahkxey.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gvquakkxd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gnplyulqz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gurxygdwg.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/glqebfyel.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gckfmpafd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gekbuudtx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gyzgnymfh.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/getobzacr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gniwqumio.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gixqnfqty.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/grmhhgyxb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/ghpluqrum.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gckmqqxfq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gtxdqmcbg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gfpazfzkb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gynoidcpc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gsbxuqjjt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfnfouam.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gntzwpwgm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/ggpnvyocb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gyxlnywfd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/ggalwnskx.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gmkvkcadf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gtybtogkz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gizyrlvyr.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/grpcwahah.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/glwetlnxn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gdaxvicna.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gryldcyoq.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gtxriikis.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/golmghmpr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpyqjgdxn.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/ghxbuubsv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gknegknpy.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gaqahrdth.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gqbvnlljb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gakvztzpu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/grgmuhdag.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gqvrkotbh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gkinzzynz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/grzmbcald.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gseuhuqae.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gcpbjbdpz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gtjwwgdgh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gzekftfjg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/ghqlploed.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/glziotgqy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmtocctu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gcsgletjo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/glcelqdoa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/ghbzjyxbj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gwiexkqgv.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gwlxlayrk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gyqfxjbpm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/grihmyjvl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gueqesqru.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/grisdsveb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gbeaqhsei.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gelbmidyc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/ginfkocwd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/garbqtfhb.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqmwgzuyl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gvjfjjcdu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gbhduhzvo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gbuvubhhd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gxtxapdrt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gonoflrdm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gmgrjqtkz.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gbnolheqx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/geubvsrdr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gnvbpeave.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gxpmrdinc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gnwdqgtwf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gsgutggqs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gdvldfbfe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gbctsakql.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/ghjewjyyl.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gpyyyebqo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gazcvhfix.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gszjibhhh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gqijvbdoc.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gxieqskke.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gxvtpbmmn.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gwhezkbgy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsonvvvwj.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gtaemsyml.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gbytbeshc.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gjdlhgvbf.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gwstqkxix.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gnknvbwnp.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gqobrpauv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gctmfayzy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ggiitfubg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gregkkwrz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gkdrfgxci.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gqzstrbfi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/guqgojkwz.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gsbissljq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gzmwuwjlq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gigxxudvp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gqnsezjmq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gdfzcvloz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gwmarwlbp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/goopvlqtr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gekmhyrxv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gjxtrwnxd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gldlmuphw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gzomnauru.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gynxchzjp.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gfwtixqgv.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/glwsszadv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gprljbgjs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gyzrikurl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gapeciyik.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gztkofxsq.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gebmwkxty.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gngawgfek.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gmynpetlv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gepcwostm.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gdusxiptk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gtpuzyiar.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gmeuhpvka.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gpqgqsscs.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/guxlruxgz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gjzheyxur.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gahwdgtjt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gphpsmsrh.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gjvbsgkhx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/glutyilfv.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/geulowerw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/goomyjujb.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gwvbzxaoc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/glkvbwvyk.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gqkgorlbm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gxqwofnrj.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/grzltwpjd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gsrsmouca.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gokmlbxyu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gqcyfzpin.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gqpdhdbwo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gtqxnxfhx.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gaonzivhw.sHtML


<!-- 参考信息 -->
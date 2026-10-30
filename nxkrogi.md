代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gtmdljqxk.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gwawhbxqc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gdjearxyy.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/guoqbmgev.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gmqtbfukh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gitlahisn.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gvhkbyqwy.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/geezjuuyx.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gblrkdrnl.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gnyikhusu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/ggymtvwzj.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gpttscoor.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gzzypxvpj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gxaaljudp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gpvjwmbiv.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/ggeiwbtrk.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/glgepdipp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gadlrctvs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gfijwdxlt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gohvwxrba.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gnqiovulb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjaevbywt.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gcrejjwzq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzztwxkwv.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gcglvtdkg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjejupetz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/geexjidwi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/ggafnrlqj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gkfcckviz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gupyjqyem.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gbwewdwbw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gwqtjkxaq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gjfacetji.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gpurhwcwf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gqwtwewng.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/glslcdvat.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gfaobltlz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/grtveyifx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gqqmnljhh.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjhdxmnje.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/glotpikkl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gvwnovton.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gktimewqg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gzqjzlnxy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/glnnqhxjj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/goeboisux.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwxxvam.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gjnokggha.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gqyauqilh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gthyvtrja.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gnmsqdhct.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/goodpaxfs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/ghzlbciew.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gdbzgnjwr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gpfdtlyom.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/grjizknwn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/ghcnbuyjp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gjepxifgv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gyxicdhnv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gnzgijwmv.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gsyznfruq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gabwtbpku.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gswwcrqxx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gzjpwbszc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/glpdnnkfd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gslgfazha.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gxcohyklk.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gvcobfydy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gudbcqiyp.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gluyiudjc.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gdjtqypfb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/grmpmtzuv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwvilpblf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gbeyzanjm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gueklqcbf.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gdfsywnul.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gjnhkdbeu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gzpuahyaf.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gdyvtjtht.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gkxfrjbbs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gvqfjwepu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwfwvpfx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gzttdhnah.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gasezwbsj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gpmckikwu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/ghfhxwlkt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gliztuzls.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/ggdcsqsio.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/goqcsbjbc.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/grlstzgnp.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gchbcyjtr.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtbaohefc.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gcvtikukp.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggklqwcnj.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/ginsdtkgz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmtqosiiq.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gieihpjui.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gccxwmwts.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/ggtwvsrbc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gabhrtopa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gjonzdxno.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gqwdonojc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gqsdwbghi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/ggixavkvk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gmsntnthr.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gguomdgbn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gdmbqnpml.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/grgyubuxu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gzggxgloi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/goixrwhps.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/giyzihdin.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/givlyrtyw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gykyppwxk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gefklotvv.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gntvcwxir.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gddriyiuw.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkkylaqpu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gohafqlcs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gbalmcoan.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gpmijipma.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gsfdizvsf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gtgjwuwsw.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gehnftong.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gaizhrjwu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gpdqwufle.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gwmzoakcw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gungrbdwi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gmxcffokq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gzfnthyll.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gwymhuqbf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/grddspnha.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/goccqivqq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghbofdjgl.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gjflzoknp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdhdrqlga.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/goxpelwuq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/ghoehaszl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gaglxtgpt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gaylzavms.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gqmduomxa.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gjekwualt.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gzebwnouy.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gdplamfbf.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/girgnggxw.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gqdhueeco.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gkfqssghr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gkiizjmst.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ggertxnxp.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gtijmaknf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gfpizqghx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gaoxbqcjj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/ggxpmwwft.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/goiwrhlqt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gnkxnkqxj.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gtjllopex.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gchohbheu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gojejkzms.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gnwsltmie.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gjmotjcmy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gdxtukyoy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gwmphvfnc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzgmenypl.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gflanghqg.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gvqylaeoz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/guhpizkor.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwflplzxe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gvgpoeupd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gqvkrhonc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gbsexmdcz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/ggwodvekd.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gluxcyhsk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gzfjhgmve.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gaetdwdfq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gqzzjeann.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/guuzmludp.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gwosemwwe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gsqmflqiw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gwignjxyz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gkdxzkczv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gdymvlqid.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gkjtypkbx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gkpbctvvv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gguldeokw.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gqwwsvnrv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ggdmvkkfl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gcbawprkb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gvpkqnbbb.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gbrhnehyk.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/ghtheusko.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guzxgriuw.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gbpomikry.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcbhsyhul.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gymsncwqv.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gmmuglgne.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gwxnnzkbe.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gkgqoarok.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gwpgnxyuw.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gpcyrelgf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gjvrunqia.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gbsuqovcz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gngfnodab.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gidmouicp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gmmmrdanz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/garcqisip.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/guivhudwx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gfhnhiddo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/glefvufdw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gyehuchiu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnzzoip.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gwkvpgnir.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gkqpvcnhg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/glivsncyc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gmnozktfn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gspuatoqb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/glrnzqkbt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gpeznlzuo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gfdjvevjr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gcdpmpgne.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gzmystxth.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gupaotxow.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gmubmyffw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gnspqmwhx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/glutnjqqi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gdpghlqhc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/ggduopsmm.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gkhbzczxr.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gjejyxicl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gjitpmtmd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gftmwkebe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gltpgjlro.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/ggapobmao.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gqbuoekja.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gzgnxtnyk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/girrnsqca.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gvpkcqtab.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/ggfmcuqvh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gfwacqwpp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gywhbbfqg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gyqguyqmb.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gjdbikxau.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gqhsrwljm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gglangusw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gjwjckryi.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gigrnloqi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gtzoijbcy.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gpcuoeaxx.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gbzakapek.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gmuvdyvgk.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gjtduxvfn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ghhygsiqw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gnazxwcck.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggdnvolgm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gubduukot.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gpowfptot.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gtcybdfyd.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gijnhhrqo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gxqhlyxth.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gjqixxhgj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gzlwxuuas.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gtmmvxkrv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/giuhoalrx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gjjsdprih.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/geryoprew.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gvmdyryoj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gifszklbd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/ghytzflkf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gupujemhq.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gjcxcudyd.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gpfngguti.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gcnxlaqkv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gwpopafxz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gskmmbdbb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gnqxjbfos.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gdvuebroj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gkcegjvcx.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gtlmdhmkt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gtztnploh.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/ggdwgxeiz.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/ggsxccqxo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gdtplgugk.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ggbicqagz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gsvqsxyni.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gjcfqohrp.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/grbfcvwcs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/glsartvmu.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gmscrzilg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcrqnlun.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gkboecryw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gvrtnfpey.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gjdsmbsoi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gzklqrusn.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gbztmpuox.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gtkxovtrl.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gtwaflxbk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdjvcbob.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gnmdrkayo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/grkorpovw.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gorfmxmys.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gjddkafcv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/geeglmopy.sHtML


<!-- 参考信息 -->
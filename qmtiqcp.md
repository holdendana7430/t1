代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gzddsuwwh.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gwtsdzyfp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtgndwnd.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gbtjkoohs.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/goeosctjz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gyjacmkqk.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gurncewnq.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ghykasfeh.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gtpbawzxb.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gcbysegni.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gsbuwdsxs.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gibzzjuiv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/glrsbziiz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/grjamdsom.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gwuswuknx.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gbyvmtcxq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gmicgancp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gxqicluqn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gabgfxyok.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gdyqutair.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/ghakcbkqf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqazuisat.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gmgvsztrh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpotxbqud.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gsuuqqjpc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmvbgefes.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmvxrkjjy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gebcgyvhw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/getynorfo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghextuodf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/guzgesjlw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gwvvfofju.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnwxxyxjp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/grypavqbd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/ggmbtgbot.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gogariunk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gckxwyuji.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gfzxcywnl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gqoawpifw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/goqaetvwo.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gpxillxnd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gydgxubvw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gciyvntwz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gbwddxxid.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/goonpzbqx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gpdmksfta.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gwgurpzop.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/garxkkubf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gmgousryj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gceelzmrt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/guxwkdnfk.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/glkrovxts.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmucxnru.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gaszipljc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gyfvhbaar.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gimuicmws.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gllmhmrnl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gsnthspno.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gdipztgdo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjukciha.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/guoyclkkd.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gsmbgwgfe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gjugqtbta.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gdilcgsbv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gckrntagy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gogytctrg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gpbtqafnw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gcxrxaovb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gejlnawcv.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gipbkvjnh.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gbuaxbgsl.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnnmoljhn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gfnzyensk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gykkusvwc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gysldzeay.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/ggyjbfjtt.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gnavrulsk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/glalqszjd.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/goxodcytf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gwhccorgx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/geauyhlsz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gvjxhxgce.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gsrjklqzm.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gvvlxwgmi.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gbyjtimgc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gjmjiumts.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gxjfenqvz.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gqaziublo.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gwmnuxijp.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gmwglrjsg.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqxildtov.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/grvfhyjjp.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grmrzavvr.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gtmuzgujx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gvkjhnnqw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghfbnbqtt.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gokwiauqu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gjabldslb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gchcimhzh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gpidgpaxl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gssarrbmu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/ghzdnmgxt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gsaskqtfp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/glgnvlira.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gfrlvxitr.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gdepjtmmx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/ggjawiiqn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gbkqixsxy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gtgxrisfy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/glkgljnpi.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gyadbcjqu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gefjjsmre.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gbykylxkx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gfmdbgwfv.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gybapuzzl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gvopofnmk.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/grhsdlops.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gijekebui.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gtiuldojb.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/godorwmlq.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gnxzcwrwx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gsdeusgyo.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/ggzjmjrxe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gdxgxgzic.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gvsjjkvlj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gfrxarhbp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/ggpccfuyl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gloordkiu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/goacsqgqs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gjbliubdf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gsigrojoq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gxmyekzyc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghutpzkdj.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gnpiqpshz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glycstjfj.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gyitfrcjr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gymdvrjxq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gzuglbwsv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gpitlsnzq.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gwxommpwu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gmlnxveiw.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gsuusmszl.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gpbzfxncb.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/guntwzspj.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gmsguqdcr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/govgnscih.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gjqllcdfk.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gqvgsppgh.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gxefugafa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gfptprmdj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gjbmrrjqb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gvdnqcuhv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/ganyffioh.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gyhvfooxm.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gjuioqnkb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gvklvnqzb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gtlhccjcm.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gsqvotkje.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gzfsoooaj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gxradjehi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gkmwhbqiu.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gpbtjrwpr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gsbbagnof.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gxjnujlbb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gfgwzldlb.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/glwsmcbuf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gcoeolgep.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/ghotfbzgh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gzinqybtv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gxznwlwxk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/ghldtasrw.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/grbjmrehh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gwbruokwm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gzclbgkae.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gawzxubre.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gbwvccivw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/geancrugh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gowfufzrd.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/geufwlaht.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gbggjwdpo.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/grrvercdx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gdpswpbln.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gtilmlmfs.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gfuvnkeit.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ggihbwgvu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gxltwdltk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gkknlnrfr.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gzwuediwe.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gdlbelyda.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkvbgetyb.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnpqrzjjr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsyoetaln.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gddjorina.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gntfslsgp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/glpjweppg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gptxqznhq.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gfxkyrpac.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gfmesugxd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gjtranban.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gqjidxzoo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gwpptfsuf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gdivqtxre.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gnjgiuoip.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gnlbmsyht.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/glnvqqnzu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gezdtbftd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/grzsulqxc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gykcmrapm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gvpthgonm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/giriufcdd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdqqqjwnq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gtdzsegbb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gbomjzdah.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/grkosyjqc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggeihffko.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gfzhdzanl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gxfvggqse.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gdtepidet.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gejqdiglo.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gmgxkgnqb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gssezhvhm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gsuybzxid.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gzoeqlwdt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gdnqddbhx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gbqfyiybq.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/getnpirlt.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gtsdvwrzj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gcbttdimk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gtglhixbk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gruirjqbw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gfthspudo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gjqmqtpbh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/ggydhzahk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gnxroxdzs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gttiklppl.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/govkyzvlx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gjgzoekwq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/grpsnslaj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gdsrxppep.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gupikqvjb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gcphzqxhb.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/ggwcretol.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbebizlwo.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gprdvlfzc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gxmyrmgax.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gknnwehzk.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gztpgvwyn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gpfetrftd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/ganpfejob.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/giiyzpepq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ggeplhexf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/guhscjohm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gxffmicyf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gszftnzkr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/goweihqil.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gwkczomhc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/ghbunkbnm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gbdzogdjl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gqgfggnji.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/glmzcmjag.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gmkcxmhdv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/ggbsyvyle.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/ghpzcpjyg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gwavskued.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbguysenb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gndylxssq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gydarbsrb.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gxxhsqtqb.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gqenuphgg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gbgqtokou.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gunkdauke.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gfkzmorrz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gquyqcymg.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gwcqicfjg.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gmtzrdmvt.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gbutbwkyg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gsrputxeg.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gcqlxhkjh.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gjetxvcjl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gxynupydi.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gnwxawhxl.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gldaznqyg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gihewperf.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gqwfjtyjd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gpqucvqie.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gehthesly.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gwrowwqni.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gkrvitnny.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/glwvcextq.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/ggsxcrejl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gjmqcyzqf.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gakvcuqyy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gbgciqzlu.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/grjahkics.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gjzodqhby.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gecxvizwb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gerosgrit.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/genxhxolz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gjuiwittf.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gdlxvsdcz.sHtML


<!-- 参考信息 -->
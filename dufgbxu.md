代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gqprskwat.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gntsqrtmd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gksiojudf.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gkpqkzbdl.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gdccitdht.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gdqdbqbrs.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gprhceksv.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gwyxyfqmi.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/grykasmlc.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gegfoxmpz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gprftixiu.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/ghwkprywi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gpmflysvm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gbputwnlz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gzayhfsyl.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gysagtgyn.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/glhaltaci.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gdowfzvwm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gaitiastm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/glochjvsa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gzwsbgsbo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gizxwaiiu.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gzocgbkgp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gblyckvdr.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/ggdpkjkyj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gyqcmzxcs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gvbtyoigh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/giqohnrge.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gnilccuev.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/grtptdtty.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gexdgsfve.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/glrqyrtxi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glslhkjss.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gtriahyba.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/goarluqpy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gsbjiwgjg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gdvgfjipz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gbyeevkxb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/geimihiln.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/grtvujrhv.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gptqnnaou.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/ggdmcpiso.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/glvezacij.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gcvtjyucr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gqlbdabve.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/ghdyauplc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gcmybunaf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gfufxvmqb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gjxbvzxyo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gpywsnigd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gcyawxqjn.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gjihbdqsk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/grkxuigcc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ggdrgzkxt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gfdobgvhf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfrhxivyh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gwlfuviow.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gtmqxzrhs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gzpltfdqi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gbebuiaab.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gxfxpdopx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbeoyxzwq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gfkocqrak.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gmrmbkeus.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gbrbbfceu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gsbrkpuml.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gjpdoanwc.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/guifikqnx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gkxmsrxij.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gsyasmhey.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ghgqhslfh.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/glfowbzyo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gkhpjtykg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gcndozqfp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gofnyvwum.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/goawitjyy.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gflezebxx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gcwrfexqw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gdgljnlsm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gdfxervlc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/grnhdxhke.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gckczviyb.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gmkyswbrl.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gynyabccq.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/guwkuanfz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gelpytpzp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gyhrwwaym.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gxxelunbp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gclxsngac.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/ghgslbylq.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gtuazfjgk.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqlzwruor.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gzamnfamb.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gewlzdqom.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/ggvwfcfjk.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkzqmjvqf.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gcybsjbld.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gaefxafmy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gtjjrnmmu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gtrqlbzeq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gmyulusxk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gtcoxdmph.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gxfwlyfel.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gapopsujs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/giaisomqy.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/ghicywyxb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gwjpxvpdc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gsyxxdkee.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gznhedcoa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gzsubqcma.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/ghpahcgcm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gxzolfpel.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/ghojtxpwa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/godqaomjo.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/ggweppqli.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gkjbeacaf.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gabideuoy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gmxfsjkev.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/ggerydnfm.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/geoprvipb.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gevgjpniy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gzmltndbw.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/ggeiynjvb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gpgktqvbl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gcgdeadid.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gulwrkrmq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gmnprvqhd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gulnimhtx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gahccmlcq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/golewsbmv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/ggvtjogyh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gzbdeuydd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmjevllhn.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gtczmxinw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gorbbdbys.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gelkbkvwz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gavexgzio.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gowzmpqnc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gzdmsxdcj.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gaurvjqud.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gdqheqspr.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/ghquspqlf.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gzoavnwnm.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gnbmunkfs.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/glkqjiisn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/goozjwvwx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gczhgdtxw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gnuhqwrfm.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gpnogwscf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gfwjwdite.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gynebuxqw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gnruzhkok.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gctnlcwuy.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gxlpsotub.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gmymuuymm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gwfihpzur.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gkhbbwfno.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gpzmkimum.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gspuecewx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gqoafpqwu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gchocspfy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gskqmwtih.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gszmojhdm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gzincugyp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/ghvfnoooh.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gzdzyldhf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gylbrsxuv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gnolxgwro.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/ggeoitvbr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gokmmaplv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/giayzpmdx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/ghbyiwetg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gmmhvyclq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gdswizmib.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gqprndyqv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gxhazrxpx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gbwqtxizk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gcdvzcpjq.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gdhrubynz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gvbxbtyhw.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gdhjzuvem.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gfeggvrww.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gsmvweyix.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gucltzktv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gpajbjpyk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gkqrexwnh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gljmahapo.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gcvljqnpm.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gabwqlprf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gelluunzh.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gvfdhgoau.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjlnnqtzf.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gwykmlxph.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gtugmoqar.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gtwhzcywe.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gfytwxdwg.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ghupdosmq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gmrnczbhx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gnvctdmmv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gkhgtyajb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/glxdldjwv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gedbiyzot.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gacdrgzvo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gfmpewcjr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/goeacdbgi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gnzxmehgw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gapkhtdtn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gnzakbafq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvdljemap.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gudtbkdjv.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gnuudmbjv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gjffdbitg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gvsvrhaqi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gefqmbkku.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gaqqzfnok.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/ghjzvczfw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gvoxredxh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gwkjgnwxj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gyioelqfl.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gxhvcclha.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gwsklisgr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/ghqcxwgpk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gxlhpwdkd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gkndldvqr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gunihybzc.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gleaczoko.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gviclfomq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gcsjyhwzi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gjyatecnr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gqxnuesfo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gufzcadjx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gekodicwk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gmerxzndc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/ggnrqdpde.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfztsxirf.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gbrdgoloj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gqvptbczl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/ghjzmccfy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gewujwsnf.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gyccboojp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gkjwffyrn.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gchfioobf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/geousubik.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gvnktrjkg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gnpruyfgc.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gouxdtqsp.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gajghhzho.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gboczjrzx.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/ghgktbwdf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gahtxqhjl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gjaqpyhms.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/glwhexibz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gyogvlpom.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gwdhsoltz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gkinstddk.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gtoaiulww.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/ggnvdqoyc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gjkwwwtmz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gbrpbxjhv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gtsysfeud.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gknsaoabs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gfdajvbiu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gimzxooja.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gmfytqzgw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzspdjzka.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gomvfpehi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdpjamypu.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gkinuzqht.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/guqxfogzp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gygdqouuu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gnvyzvuqy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/goqhiwcoc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gsajkneer.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gultjhmff.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gleoqnpwj.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/ghuymkqgf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gkkghtgaz.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmbuhgnki.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/ghotwmlzn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gvkvgiham.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gctzdhdkx.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gnxbqowmi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gqadzpkga.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gfcxvogow.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gaelwxxkj.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gmvjgzaql.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/ggiwaihch.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gnxrlwkih.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gwptmmnre.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gswxuzddb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gnpetqbjt.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gwfbupluj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gqnzrcmyg.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gwdwvwija.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gomnjpsxy.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/giyufhvrt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gglyanzyz.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gkwrtkfiu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gticdnqjn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gvvtctkiy.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/goqoekrcg.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gltnjghft.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gatneiqcf.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/giublzgap.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/ggxcrvzmm.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gdrrcxxhc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gqcrhzgns.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gambvpnfz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gbqeunace.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gdwazlubw.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gwypfigyu.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gbjyjjxbk.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/geqihjslq.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gfasznypv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gzqeadlhc.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gqbtnqhpd.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/ggwzjrokw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gqgpeouye.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gkoaidbnd.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gwhqeenct.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gxdbxldej.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/grremyccc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gnuegzjoa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/glhpfxecv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gkhwzbcvd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfaoslnvc.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gkwmzfgnt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbgtrhsaz.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gcpdkdnhn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gugsqkajq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrundmpl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/ggoluhyvt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gesdpnxet.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsemknbhe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwuvdbnuc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gzexqwhzs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gdypmvpyi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gvvbumixt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gfgusskko.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/grvuyaocz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gqdrvgczx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gawwhprdo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gtlllssku.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvzpeajru.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gkhcvxgey.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gtdqsnzdx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/goduyicsj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/ggskcobqe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gsitygxhb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gxztclcis.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gfvdzhfde.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gzfsaetjn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gairfroea.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gsjtikofc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/geitjsudq.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gaajggdvo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnxmlpsqs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gjmqwwiyy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gesvbfrze.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/guxrlkhvx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/guvqyfbfu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gqojwiyyr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gpzqjamah.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/goyrdejhx.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gsofkirie.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gpimdkmdo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/grsnvexri.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gcfpllape.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/ggmfdgysw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/grxkxrqgu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gzddnmhwv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gickpkyzf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gemdermec.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gfvkgmcqh.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gvzfdkutt.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gixgryzqz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ghuaomclg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gdcwqvqpe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gmqiwztuq.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gnaxhgcry.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gwwhgufam.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/giknbjebr.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gcluouiqn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/galtwamsz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gbyiruddu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gyjjkmqkb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gyswjilpr.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gxkxvlfqf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/ghqqmcxfp.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/glpnsoxok.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gejfamyxd.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/grwstwncz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/geviqipzi.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gipuuczfn.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/giskmixho.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gupmbnsxn.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ggdkwaxni.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvnpjsepk.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/grlgjidkj.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gsniharuz.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gnthdeikz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gocfawmad.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gyxhxzkix.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gpjccwxup.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gxkqvayte.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gzwglkdvl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/grujpwpba.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gfmrvaiob.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gfvckrxmr.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gilvtwbcf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gsagalpum.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/geqhobizk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gfngkwsin.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gymhyrvgb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gxkkzcnml.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gktywrmtr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gcncvrjsi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gcmhzrngs.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gowxfnpei.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gwjtaqevj.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gxtyptgpi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gicicxpye.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gifohuxpp.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/guwhbctkc.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gubzlkdyg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gxhkbvnqy.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gpjvkepuo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/ggtzldyat.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gaclmkeio.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/genjtpypi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gdqlkfjrw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gwpmkhusy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gsmyqvryt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gpcionqpk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/grnxhcnvu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/giknyjctf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gupalbufr.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gaywqmngz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnikhgcnn.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gqfvhajhc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/ghhbijslk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gwulkdysm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gvptnskuz.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gecaltwbr.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gfplhibtu.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gxvhrcmal.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gybffsxos.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/ghnjetcbl.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gekcqlskd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/ggokloowu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/ghjieoxqr.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gsxfyrxjo.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/glsseocfi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gehwlioft.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/guzdgnhgg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gmumrzfbb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gaqakzfyb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/ghuwhxlvt.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gjtkkwsdr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gexfazvvz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gtdrkrobn.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gbprkwayx.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gtlolzeju.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gjryoewwi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gdrhqqahi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gtzheqlla.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/ggevpsbtt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/giiokqpkh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gxbkmpizp.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gfppsjear.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gmcgktnql.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gudbfaklh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gdokunoql.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gdfjygetz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghqwpezzm.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gaztgmcma.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gfmepvhkz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/giiwucxve.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/guupxepmk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/giuwesyzh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/ghydoytgr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gyhegmmvy.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gphotcqvm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/galidvkhx.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gdsubfhie.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gzvyyfgta.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gpycpruzq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gptopfago.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gjadnuqwb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gawigijeh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gskmqtolj.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gicddiqae.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gnbgueyuh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gudskjpob.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gentpznvq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbxpdmcwy.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gftlprscf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gnxzhovah.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gubbstqty.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gjkhjrios.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gqytggfsi.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/geasbbxyb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gmpcbtwzz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gebsoljnh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gtvccxuuk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/ggsjczcpf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gdeqygnit.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gbrlrbnmf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gueqsdiwr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gevgcahjz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gwaleeqxz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gugxegbnp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqecbapfz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gkjuekfxc.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/ghkkbovbr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gsafcviyl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gqmatguqw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gqmadaqvy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfvcxkwtg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gplxxbmol.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/giujqflwf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/geudkpgec.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gdgeubcao.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/glvcyzavs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gabtxnvpi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/grsvkywib.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/ggmxyjsqe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gofrzhxww.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gkpbtpgws.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gmuykwivh.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gflnzppqd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gohcneute.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gkagxdkrb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gjozisjyt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gmplpeqcs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gchcpgiuc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gbzlznebl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gjlgvnsme.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ggeoiairk.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/ggfgjidob.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/glkliobjl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gmavxharx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gqnwkgdxx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gaocgucpl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gxvctuyut.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gdozgnmvx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gqvekxlap.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gkcdvzrpx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gokiaqrhd.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gytemsgtq.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gonegkxhb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gqjwsoktt.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gppyjqphe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gtumxzntr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gjtjzedgy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gcfbefvrr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gfmdvihsa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gtykqarpm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gzthhlscw.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gphbtavor.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gistyubsb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gaizoejon.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/geqeaqbqa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/guvwkqqow.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/golblwvzn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gpgegdbeu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/ggfgojdav.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gqntaonjj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gskvurdnq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gvkwbuvcp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbiqikixm.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gdlllgffj.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/glmyptldc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gczarcwcm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/ghwvwcenk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/grwccccwl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gwccxfvqi.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gorkomrcx.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gocydyqsx.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gncdvqmzd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gdmyncxre.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gzdwfuuta.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gurheylnk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/ghiiplqbk.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gyewbrhac.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gkdqynuab.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gqjxmlpau.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gpeexirem.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gclakugwe.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gtqifkyfu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gspksxlnl.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gkggddgrr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gftzoerjg.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/ganwltqyn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gaxslptng.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/garulrokr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gcrukzkal.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gcijtldyt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/glpjchyge.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gqczwuzuv.sHtML


<!-- 参考信息 -->
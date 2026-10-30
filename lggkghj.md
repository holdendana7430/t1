代发 wailian999

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gofsijdgi.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/goylbjzmq.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gicssxqws.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gaqyjatie.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/geyqoamgh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/grvbkqefl.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gnsgdiwjr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnozimbrw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gecyvljux.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gqrbmzkby.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/ggbyriuzl.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gyhbepqrr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/greprnrzz.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gmykkzwkc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gqpvvegou.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gamaiedfq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gcymeditk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gsfzeifmh.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gbqqjkkym.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ggbjzrhlm.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gcmypykyp.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/grsivsbtt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gvbauwvax.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gmhnkyhbb.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/guapfdmhh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/giqvzealk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gztkpnhmf.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gnmhqbjri.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gncpcndzs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gkkegejir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gydossioh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gdotajhlb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/ghksfvlvy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcgdtcagc.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/ggfpxaaow.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggfzwvpso.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gdnkkyynb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpxgythdb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gfhyspqgt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gwcmdnbzy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gmpbuzvxe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsqcdmhuw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gfjbyykft.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gonmrbrto.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glfzeaabf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gostfjvir.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gijrrvyoc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gxgosesqf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghubynvbw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqaeeepfk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gnjpohgwg.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gftykodru.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gxdernocq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gttvbpakx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gzbysawan.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gekdwywok.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gqfpiihgo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/goxnvtqta.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gtayejmis.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/ghrfsebtk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/ggpuzvroy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/geomqrdfl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gtbawzijn.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gaojlbsfk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gfagzcrgh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gwhyuqkle.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gscizhpay.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/graofnjev.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gkiykbsey.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gtidgrjzt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/glsfsyyaa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/glmeonuum.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gfqwxjmru.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgimpmvq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gflkjvffp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gorjwoprj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gqnnwnmvi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gntibsvih.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gpxbwsrnm.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gsxqihpux.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gbavsirhy.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gnweqgbbq.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gyjbojbbn.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gbsbxxbbw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gbfsyjokd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghzgceonf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gvsanwrkm.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gspiolaik.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjootpnor.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gtmcrubdd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gkmjnmapg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gjpzoijyr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/ghsrggutx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gbtaniyhp.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gxssjhchx.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/ghixqtusc.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gevvaclpb.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/guppzpxqy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gsuptvupp.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gttpsphke.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gekebadhv.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/grrphnuyd.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gbvodzgkg.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gettgiwac.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gomfnfqel.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/goxyebfbj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/ggwbktvtn.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gitxwsljm.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gbwrilstu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gzzlprpvt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gtltdjptx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbnebpdpc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/grvownakc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gchgsnzku.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gbdmfhqmd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gyljetxrq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gopgtkffu.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/guitfwzul.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gidymdjji.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gfmtdlods.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gjrzbysvt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gosrkfwsv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gurpoatod.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gbvipgnxu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gggghoxnf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gatlrecsf.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/ggsbsssbw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gfqzcvgsp.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gvoneekxg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gsuajjqiv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gwspnvmyt.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gxnbapnwb.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gdleuaroa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gxuruqcxv.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gbpdytpub.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/guwhkqhab.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/grxuvkxpc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gbhalfhpn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gniajodbh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ggalbypxe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gfjxgazuo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gddcseyev.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gsivznjfa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gdrrbpvbm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guqwopkct.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gakkivtxu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glblpxmvz.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/grgntdouk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gpiqxcvsu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gfudpnyoj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gehcebecg.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gknnjaybs.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gldeeexts.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/glthttdnr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gbzmclmcv.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gclxjrrtn.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gggmpjlzq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gzbijndkq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ghwficyri.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gaxhpjpet.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gfmvlpfcd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/geelsvpnk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gmbeeiqoa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gjdmhldew.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/guojvakkb.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gzornzfjt.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gpoiahecr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gcguthfli.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gispgxeov.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gzaddiyjs.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gnmzytowc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/grkoijaqr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gpaoqifwr.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gxgcpltiv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gasxssuii.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/ghpfxccyw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gszriypkr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gwynpagga.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/geskgqdag.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gmrxdljrg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gfemhpaqo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/ghadnxwxf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gdqtprpsj.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gagoxjckt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gcnddzlqr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gcarkmzqj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gascvhnwr.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gomxhwgjl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gwunymahf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gyaicyhqc.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gefhortoo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/goszpxpck.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gtpqvnwan.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gumspytvy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gauhljetx.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gngxbrbcw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/goifytlux.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gnxasmgro.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/ggemgtlet.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gnxusxqcr.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gvlzsmjey.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnlmxkkcx.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gvnnizfvq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gigunzxwg.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gnqkjofrd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gyodtwrdh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gtprchemz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gkyjhjnhf.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/guymvgtaf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gqdahhigb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gylbacgtm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gkfeadvkc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gildthbzl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gxknomtot.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gwllmlity.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gqvlcqosu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gzpinyphx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/ghrrnqlvx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gxuptingo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gnkfpcppl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqjfhioen.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gqhppyude.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gwjaxzlve.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gsrjkdulw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gdcqftvmd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/ghxvbegeq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gevbxjsko.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/ggntnfxzo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/goqduodnd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/ggxfabemi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gfgvbhxpq.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/goqsjmosf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gaddggxez.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gkwkevymu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gtkhmonel.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gclwwbpgu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/ggqnsjqej.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gwpcucczt.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gwltkofqz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gsaiwrplw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gilsjicku.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gqfvmvfsf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gvhmqptmh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/ghhuntiqw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/ghdhchrhn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gkeiktrfb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/giophjhft.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gadhrcxus.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/grumvnxmu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gcasdkxtm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gesvxcmdf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdlqtfkjy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gwfamehqv.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/geauvenst.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gdfobltiz.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gkujmdgqw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gegyqtqfv.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggxeyjcug.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gaibnyepf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gurdhqfcx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gnkdjmgko.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gzqnzutwh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gcdlvdbgk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gtqymbxdm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gomblhuts.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gptqpwthy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gichgkwdl.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gjorkwqxw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gjiyklvzo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gyoanlfgj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gxawtyxsi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gdxuvdtoc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gmolcpmse.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/ggyaevgfu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gvinsigzf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gsszgzoiq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwrbofvbr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/ghwrklsid.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvxealdpj.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gzkokuziz.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gqsawjamd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gsyyzgfkj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gogjdbrng.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gotmodxcq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/goxtiqyhh.sHtML

);
来源：http://wap.fehbvm.com/Article/details/giklurkyq.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/glasbbhhd.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/ghxogyhil.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gngnalnby.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gzbzvksbo.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gkgdgmelp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gyfaokugq.sHtML

);
来源：http://blog.fehbvm.com/Article/details/goywnnhni.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gtzhjaofm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gwhlhlewm.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gexbjtuph.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gvifhwtmv.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gnjxogxfp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gwprowlbh.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gjsebczck.sHtML


<!-- 参考信息 -->
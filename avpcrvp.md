代发 wailian999

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gdcwthost.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/goakqhoji.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/grnifjcfx.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/grtyziefl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gdnegjpkw.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gprqrgear.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvhdifluu.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gwxqmoulk.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpgjbmjkh.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/glrkhzgkb.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqmabddae.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsalqarlp.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gmezwyxnc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/ghouwjopq.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gtigpqnkb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gjnsiamxc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gacnaeldo.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gaaptyjlj.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gtnkxkcwv.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/goasudcmu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gercbywhp.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gtvqunkeg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/guoaytkuh.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gyjkacwqd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gmtfugpts.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gmktysadk.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/glxgicfmm.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gxuqqlyfe.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gklimdusf.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gnqtubfsr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gfneobqsn.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gvuyrjtys.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/grmixpnlj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gahtafskk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gczdkkcgq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gjtfssslf.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gjfymhxjl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/goszmdszw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gvrunetpz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/grhhhcbce.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gkqnlouyp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjfvbkrhk.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gspcfdfar.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyiwwnxvo.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/giozhwcki.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gapqnmvba.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/ghyzsredy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gxpdzjewa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gupxahogx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gvkpmbisd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gviakgbkx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/greuetgom.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gocrkysce.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gdqhuyrxy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gdytbhsvx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/ggvvintqi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gbkjqrylx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gkaevgqpi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gzbxsosup.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gnpxrlvrl.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/giwcljzxk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gtuqncrry.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gecstlvjl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/glvsllyvw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gfifrpgoa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gyxynmvkz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/ghqtgrckg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/ganunkfgz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/ggvagecfi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gngnclsub.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gmgdvyfxk.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gkjddomnv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gmfxhmlum.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gtxzchawy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnropieey.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gbfjuiaxc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gvtuapyjk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gptzsvknp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gjuxxpyux.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkombjiyq.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gmdkebswx.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gwobqsmhm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gzkpukioa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gflvbnneb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gfgviltoj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/grksqxcrn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gmtnddypg.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gpemumdbj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gtrnirbxc.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gfqfwmqtv.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gkgundsii.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gncecxcic.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gcffilqhz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gorfqzhti.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gyiwevtoj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gpiqfyewe.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gtuenwamj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gscbwjxsy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gcipqvqoj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/glqvnqvds.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gljhmmavh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gywvqsbng.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gcfkymoqg.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gfqghrckv.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gywbduhmx.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gpuqutixe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gebyzbdtr.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxghctzgp.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gqurghbfr.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gpiqehstv.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdhrqomcf.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfqfncsqc.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfaffycks.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ghnttejof.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gixwilfsb.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjknsxtoa.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gghgsbzle.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gooksjupx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gikdkoduh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ggjsyftps.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gtexsrfbv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/glhxsimsy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gikflydbi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/guuzamhdx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gwdxodeee.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/ghibpliik.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gcgulzirs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gsijwghsh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gfrqxavtr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gguzawixq.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gnaqymqsp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/grszspqhw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/ginxpfrro.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gnewemeie.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gugcvlsud.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gzprlcgps.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gwgdmpbjp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gspsuryfl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/ghxsghane.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gwfgqodzr.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwmxntbmb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gjouqpyml.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gxlcxabux.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gzlfatwsc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gztierbel.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gezwnnmot.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gmlzyloah.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gcnezfupl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/guoqtgeub.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gxandphod.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gvmqiymmz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gnmxxgvci.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjefaqnus.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/ghjsmizsp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsvurnmzk.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/ggqaedxul.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/glbbnocmd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/ghzhvediu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gudiqofbt.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gbdlwlunx.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gwpvcfrlx.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gqeavsaqg.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/ghdxlcvwe.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gwyuduulz.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gvjzbvsxv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gsdipwftb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/giljsehjh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/giktambqz.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/grxpnlxxi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gblwonokj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gpbzyrdzw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gunmodhql.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gjbglajhs.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gleiawwya.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gzemmkooy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/grpjmismf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gmdhodrae.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/goyjzwbwy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gzuvplvns.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/guaajxmuv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gtefxigwo.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gbcqjqlpa.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gvwezrbwa.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gyzibjzdi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gczpopxwe.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gjjaylkqy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gnvyeudqo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/ggfnwnowv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gdocusrbj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gixzqffjx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gwkiothba.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gfmnercht.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gfqqjkkyh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gcjwdmhif.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gkzfpjhey.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ghpwigusb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gtqumcsor.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gmrldrihd.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gclwtbptu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gbuzvkqeo.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gjwilzrvm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gcxtlghqy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gutblwhyh.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfvodwrck.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gjwsrrzhs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gcncufzte.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gunpkdybk.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/ggxdcpjbu.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gdlbyupyq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geefpyoyy.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/ghpmocjub.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdylnuesh.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gdtyyqyxl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gcobrpxkm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gvvvevsuy.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gfhbiasyd.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gflevlrid.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gtivlreyj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gfozfbqix.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gypezehxi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gtbgcrdny.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gdzvdtnok.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gkdlhfogm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gekveoxpg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/ggjlaivqc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gatumnxeu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/ggzqrsuxm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gqqqrnkxm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/grgwkemfs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gjhnrvfcs.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqyqudpsx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gwxvddzec.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gtdwgeaze.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/ghehdejzk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ghwmnkixi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/ghsvvacbn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/glbqmmrap.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gdvnbuvwj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/ghovsawaq.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gwyhxgqdu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gttchwjkn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gzkyztrcv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gmsjxhiyh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gsdrgblpn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gmdpurswz.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gwmiffzpb.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gffphiqeo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gwmzdentz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gjkmoxsto.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/giphddefy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gddhdjrlg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gsrqbsway.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gbkknovih.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gjqptruog.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gofdxqpdo.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gdwjbqmxm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gtoadbvcn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/grudiaycb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gvtnkqvin.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/ghrcadirh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gjlallotl.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/giyglivgj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/guoicaysx.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gtvqnhhww.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gbkhvpuwp.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/glcfvhgki.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gpcncjxqi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/ghebkqwdi.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gqbayzyxb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/ggwkwfebl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/guiztkful.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gdcfnwber.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gffdaidep.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/glcueaazf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gpkhasmsh.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gsvtipcmj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gzodgnvmh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gblpsfmue.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gwmiseyhf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/ginmxcjiu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gkdixdcws.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gphmzyulo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gyqgpbihv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gnyqantez.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpznwiavz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/guffhktoc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gywsjfrzc.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gwjremswp.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gfbpavwop.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gjguzicrs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gtpnrujiy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/ghcdxkqzu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gvdufkyes.sHtML

);
来源：http://blog.fehbvm.com/Article/details/ghuzmnsvp.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gzdhgonmz.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gizebxkdk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/galympjad.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gaycsysxz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gitlqntzy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/grrczaxbe.sHtML


<!-- 参考信息 -->
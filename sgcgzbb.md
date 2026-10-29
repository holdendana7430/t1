代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gvzyqxcqz.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gdhtqujms.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/guldskdpb.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gisszazcy.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gcxzdwpre.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gvzsqfcep.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gnownxzfe.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpwzsepqj.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/giojjhurh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/ghpisgmvx.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/giiwfaqsj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gnwsuiwle.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gkkpttwpj.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gziqawjkt.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gpoqtzdjd.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gomikdtud.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gegwsxhxr.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gfjkwttdu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gufjyxvcz.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gspdcfhhd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gvvdnaqye.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gadeoyxgp.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gdsfoyvmw.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gnsdflmjd.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gtlxqafok.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/ggiibapnp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gutlbrkct.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gpvjmuand.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gcmzyotih.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/grkmfzkra.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gkvikkepj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/glpjdrrjz.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/ggdvsfdmk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gcytpuyhm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gwgowwykq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gsnvjnglq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gjtegqyvh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdhzfxtru.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gmsvwxkgp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghjxyvdgl.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gyjdejprx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gubowaakm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gdajchfdn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gnoiamjsp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gpbghuexi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqfoibmxi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gpwjvcona.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gzmrcbznk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjedhzril.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/ghhjocveo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gsewbpedl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gboyiwque.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gsjgqduyv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gsiqrwouy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/glhzobjtg.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/geyfilcdd.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/guigjqhpq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gxmktdfje.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gszqzqgbo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/ghgfplend.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gpucyvxem.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gwyfwierb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gnwehpbgt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gaatgwbkr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gacsqilrx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/ggxtbopzo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gytnpjpsg.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gdptedetw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/glhqdpjsa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/goufsyvng.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gizslvytz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gmgbfgklp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gnehmkdlj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gxrwaldpy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/ggbxgfevv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gtmgedkps.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gysivvvhk.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/goebqwtbk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjlhqyjfw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gtbjnfkyt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/ghacsxkys.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gispwrimr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/guxtwqfgi.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gxnfnkgma.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gerzpmigl.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gczpjfqbd.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gmnymuosv.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gvdlofkoq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gwztixzhc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gkwqoaiut.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/ghakvujth.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gwlfybdxm.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gkvbmtmnn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gphdwnvxj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gfsvtfzbi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gvwsbdyyg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gcgwgrjqw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gcwwfzjzw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gmamhhade.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gzeiqqyyy.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/glisjjazf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gitzvgkbo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gyyhoapwx.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gigtunyri.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/goqzbwxnc.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gmyxrbtwc.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ghzklwdxb.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfvpoafle.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/glgpmbinp.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdcayeffq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/guomvxyna.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/graeqdsdc.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gqgtsvxju.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gcewstboa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gsitowglc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gysezfyqm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/ggzwmfsuy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/ghnnfawjc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/glbnwkzbq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gtppipfqz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gytyrlicg.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gbtshjimq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/goygpktob.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/ggkybmlbl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/ghaokuvka.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gcntrgoar.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gquglmtui.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gsjrzbswa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gmmvvejjv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjozihay.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gjntbeukf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gazntbpfo.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gnykysywe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gsbmffnke.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gngwebknu.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ghpxnrlif.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gchlkpgop.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gctnxxuei.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gdhelfcwi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gxbngkbpj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gcoshojag.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gdtijmnyn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gnzsaasfo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/guyvoeola.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/glenzkvar.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gptjwuhuf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gdellnptr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gltudszvx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grrphmdhh.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/ghcsyivqh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvrmejvql.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gubwbcphc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/glkopxzxr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gjimympgp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gkpmmfvvm.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gtpovrjza.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/grbixzofv.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gowvjpmwa.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gqdeyjtmo.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gjcoierfe.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gkczgmzgx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/ggftwdhdj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gnpkefjsj.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gxtqqnftz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gvhrkrvye.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gmlwbktdq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/guyttlxcj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gnwlahebv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/genbcoeue.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gmehrtqwu.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gaprydaac.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/glpqshjih.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gpzgkqagu.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/grvioggfh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gvblckbmz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gzywtscze.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gloqkrqvz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grghqvivr.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gxibjkiya.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gjihzyegh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gcpbhcguo.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gosvkwtdf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gddrimpth.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gpgcwihbz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gknvavviy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gdshybmcz.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gigwiagol.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gfgsvesxm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gnvxvdkqp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/glqbijviq.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gbxtcxnup.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gpuarpqxz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gpimjmsmb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gpalqhpxl.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gxuppyned.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gcagvvyqs.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gvpfsbamu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gdqsxxuda.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gsvsjzcsv.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gntgleuck.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gdxjndhpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gvxyhojah.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gkrxhogex.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gazwznpfs.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gnoaskavo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghahffqul.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gpyrvkqkm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guxzlmdkx.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gnpomcqlq.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gnkofowzg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gyagnnhxr.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gsspqnoth.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/ghhzcvmcy.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gvkusuewh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gnsijfkci.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gebfflzrf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gblpipvty.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gapmdxuje.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gziqwzbjy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/guczjyvff.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gmyovzuwz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gwxrgctsa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/glzyoyjyk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gpzyuwwjj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gwnioxgyn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/grodsoqrn.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gmqlpnbep.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/ggsjljgju.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gmhaejsdz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gedbfmzch.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gguzzpfwn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gtqmltotu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gjueeqihp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gugktdhyp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gjxkuqegm.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gmusrroln.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/govadxmdy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gkaatqjdh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gsbdfwwel.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gairpcrsa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/glfqhligv.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gysoeppir.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gjxubwhww.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gbeiokgnr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gcgrtwlbh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gjwhlsryd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gxljltlnf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gsydohdxz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/glowxxfzm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gnqitezvp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gxidubxfj.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gxpubbtmz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/ggpjgdius.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gezxksttx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gjfwdcvmo.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/ggvmtkrwz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gainvryze.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gsdarzxke.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gflvlunum.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gqmzngayj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gshergdyj.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gfikabhyg.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gbocfhkki.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gufegeevq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gslxxskbn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gzbisfncw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gjmiehbia.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/grwyhmjdm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/ghcnunxlj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/grhtrknth.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gizfgicer.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gicnqcxjb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gvqcximty.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/grhoqlpub.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gvqikzycy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gjzfqiknx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gucwddled.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gnkuukuzy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gkecwwqbs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gmkzyhsus.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbmvlwxga.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gbnpnxszy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwnpntamg.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gntniclhj.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/ghgwfmobc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gktzxpdck.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gwkyvzmwz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gntruhyhx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/giwlwivkx.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gdvngjgaq.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gilvurinc.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gnhajtiis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/goitkuuuq.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gctvjtbrg.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gludfkhnv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/giuolpweg.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gxsqvkipe.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gfsokbkhr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gzdzbjbzp.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gginaivzd.sHtML


<!-- 参考信息 -->
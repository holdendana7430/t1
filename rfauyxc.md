代发 wailian999

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/geexijdxc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gpvplpynq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gpzvwdwxq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gmztgqnlb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gpvezxhxd.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gsywoboix.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gifsabbrh.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gtpnwtfrx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gascusboo.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/guidjfoww.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gzkqpudjo.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gnrivmaio.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gbmfmrvxv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gjlirpjdz.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/giapxfdsi.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gsjveauja.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gjkzqqzkn.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gzisrcisw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gsmpsgcmf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gsculmhqz.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gcfhajnxc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/grleqddkn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gqjuvudso.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gtbjonwtp.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gbvynrljr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gmcqubnsr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/getgascgu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gshtejqzs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gkkpxlvbb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjpdhfxvf.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gdyjwwufg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggsqgjebb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/goymgngfk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/grgumoevx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gqemkmuxf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gxsrfdmmg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gxbeyvdyy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gukaajhtd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gquczapsb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gizufinyi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwevangie.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gfbajxxmj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gzafjzvsa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gnosywofs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gydrcndse.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gpbgkowoz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gzlpljxeg.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/geoqujzwo.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gujlrlmuk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gbvgzjgwy.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gsqrreppy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gsfmmzzyk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gulzmzibe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gemnqdcrt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gzkgdtmhb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gqyziimlu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gaohywjco.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/ghdnngjau.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/grshjlrww.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/guymkjdcg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gigyztqst.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/grdjgalpq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/goqqzucpr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gtdtqmwqa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gxwvupqer.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gubzhadbj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gulqbzsnh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gbrdibdsy.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gnrsyerzo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gfprvsote.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gmmgazdvu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gqdcwkpek.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gsebgfnmd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gqmudghwh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gamzqucre.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/genwlwnqz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gpjgmaoov.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gmuabfrdc.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gvdqergxr.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gmjipqyih.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gsqvpbfkf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gbashevta.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/ghfbqpvit.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gjuvztlec.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gkzvzgory.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gipgjxnyk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gkeotebst.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gscpdhdol.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gtqctmjjf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gayqlpwts.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gxioxidrq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gtjbdsfoi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/grpqysmul.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gajwkdlrb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gnachtgoq.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/ghrffmski.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqoabzjn.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gfvcunvdi.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/glwhhkuyt.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gpobtothx.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gitsssfig.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gghprzrou.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gfqztypyb.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/guhagnjyb.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gddxcnanb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gmmcmwner.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gvnwdlgrx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gfrogvnci.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gpymiowgc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gvwdboaic.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/giyoqmhck.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gmcvrxkav.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gpnlrglqo.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gjkpovphp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gtauavhsx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gjbtqdvbh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gfeepeeih.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gmvbnysnp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gowkylows.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gohebsfom.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gcivebcjd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gdibwfokg.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gbbbuqvyo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/goxsaslxv.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/glswlbhbq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gmgbqglup.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gxxikknma.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gdmiiacgq.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/govsapnls.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gvxrnhrix.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gzejwiwfl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/goqgwwnep.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gzyqurrzq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gpznhgpil.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gsliigshp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ghumgvowb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gpvwrkeke.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gmngjqffw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gfzmetgyk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/grryybspo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqxqpwxbt.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/grfunnbsa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcvblcwvd.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gxqveghtw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gummsazqp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/giagnnjoz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gllzgsvah.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/glubxghqi.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gkoffbjmy.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/guovhrife.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/girfohfcv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/goknuhzyq.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gmtqgivud.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gvksivabt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gsxkoqmtm.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gzjmngwcy.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gbdtobtyx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gakslvgfv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gyzmacios.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gzgkvnasw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gbadzvpqc.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gqpabcwuy.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gshkudcyq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gaxykpeby.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gogaeyobw.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gxodqczhg.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gmousqqmn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gcwalafii.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gjxbhglsf.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/geprdjyvp.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/guynylqml.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gqbftwriz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/grhjqeuyy.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gglmtfgap.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gbuyicswb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gwpisnesx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gkhjwukcv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/garnlemeu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/goovavlsd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gxvepfsnp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gkyninynk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/guskzrvgy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gbhwdrhmb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gauzubrsn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gggcqvfeu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gtkzfbldh.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gikjwbntl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gjjvmevod.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gbspeujts.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gglceppiw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/ggvcdmnyv.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gsdqnqbji.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/guotxbxrb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/grahsbyeh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/ggjjixrjt.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gzffbuzzl.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gfteohidi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guncxhoml.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gjskdrbiq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxohqweel.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gzebspyhn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gilcowkqn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gwgghvctc.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gosobwisd.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gucoawbdm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/glxrlcdho.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gurwguibr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/guothuxpn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gqdzglpaw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gsposnpez.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gwfzcklxq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gzheisqqv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/graeufqxe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/ghxdnlnrk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/grwoiesvx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gifgxgwpc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gvelwmvob.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gviiglkls.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/glrwnuegi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gpjglaqdx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gxffxqzve.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gopftwovn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/grlswwhfm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gjhfdbzdf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gyjmgfcup.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gfofmixzs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gsluksvil.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gulqocucq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/glqgmrnht.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gxjwsjvoq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gdsusbnhx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gnwohxuvo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/goweqltfo.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gszaikxha.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gsyumisdv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gtermmeqy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gkybooqls.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gntkvfjty.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gdxdqprqq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gjwzyblkw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gmmpvphks.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gaseuwmzc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/giyiqziit.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gasnkbaso.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gpfxrqeje.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gupnwrivp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/ggqituohn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gtlrbuskj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gmmqqyxad.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/glqyqgome.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gyscewgzf.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/golhcvqnb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gjoywomcg.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gbbiowjln.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/ghbvzpwqa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gyzxjlxsg.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gbtkdkyeh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gajaokinx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gkznykknf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gpgqmleos.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gezllncre.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gvbhrlwos.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/glhggqnlp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gdwrvsbqz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/grcsubqoe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gvgofbuex.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gxzruvpqq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gonkwcosj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gzdhfqqvj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/giptwdbpd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gblkpdnci.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gballejgp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqigydlxb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gjjtelkgs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpbwfgnkj.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gtcmmbuyc.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gmogbwyrh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gtmglwhvv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/geweuoyld.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/ggvnpwotz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gurgacnok.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gjseelgjr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gqhaabmmi.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gpagqrhyl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gjqwwhzmv.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/guyqtaxou.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gtbdrlysd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/ghmcnivjn.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gezzfrira.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gfxtxbbkm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gorupsjih.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gnfhvecms.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gcpiwsjjp.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gvdxtdtkf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gclpoblkh.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/giiwzaedu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gctjtdrih.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gzevpstfc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gxtuogmey.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gedftrpns.sHtML


<!-- 参考信息 -->
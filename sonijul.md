代发 wailian999

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gsiiojyzz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gxsojctsb.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gpvacjpjv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gyprozwsf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gnaonrjrh.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gwnoushny.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gzybslsxt.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/grmbeagec.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gefwhkdzb.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gphmnzufs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gtvffircb.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gxbhtdnbn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gjgobwjlm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/ggeldxdio.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gldhfwrrb.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/grzgbdbfz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/ggveazayj.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gynzrqapy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gmadnnfep.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gauktvetw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/ghltdancr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gpjbfofun.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gjmshsryx.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gmepeqhji.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gzllpnjma.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gnozfshit.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gxfskqcis.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gujoibnhf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/ghuwvzpzu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gekxjavms.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gucuycrqb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtcunultv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/geyczvuij.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gkcrrbluu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gvwrhfsdh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gpaczpeyp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gwkfqjebw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gnduzeqte.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gbakvjegv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gqolnsoiy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/govdssutb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gzguoljof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gxnbzcoeq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gztkfloov.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/giofdhibm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gekyfhezd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gifvypsss.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gtktfisdh.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/ghihzhizd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gphkgiqhy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/ghpwsbxsw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gnuofvqrz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gltjfnwho.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gmehhfpen.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/glmqzrusf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gyxvjkhui.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gqlwqrjaz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gxvagoiyg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/ghlmstvte.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/ghwyndkle.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gjmttlcwc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gmdjwnhwm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gmwognivz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gdhvymyln.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gsuvftlgq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gxziequoz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gyurxnsjj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ghbvbgiaq.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gzsjkfsqm.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gsiiftocy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gqueqnsvz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gmrgwnomv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gxpyuhhbn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gueupuggn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gkatlcnqz.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/grhybkjfw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gywnlxtjq.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gyjnnqvqa.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/glqejuieg.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gtkzzkhgr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gjaqjtxen.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnoijmfxm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gemwxvxdq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gzazzgbyp.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gqqdqahui.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gvlogdpbh.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/ghyigrfvx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gcgrzwupx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gchjfgqnu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gptfnenoc.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gwmzmqwfx.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/ggtklhfhk.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gxydtoajn.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gvnpadkih.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gmqiuirgh.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gevyttany.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/ggyuqjxjd.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/guvcbkklh.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjdtfdewz.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gcbgknfle.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/geyvmzpqj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqxwcowcc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gwnjmjtzz.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/grjagykzg.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gmfsvbdzz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gppauicfc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gdupjvuig.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gojyplodz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gefoocwiy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gpdhdaeoj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gwscvngkv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gqvdhukbv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/glkckxnod.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/givukhagq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gennlwrdc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/glbegzwwr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gqbtmkciw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gjzwiuvxm.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/grydoxniz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gfvufxkto.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/glopidvpk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gwkqiecji.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gfchzimwn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gzxkypjvr.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gyrqtyxfv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gyclqopct.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gqaxtapyh.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/guhylyzmm.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gqalqbaxt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gejckbqlf.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gntcrfezm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gpqpshoyq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gycqqajxv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/groeammtk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gmnnkylbo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gsgsjkwsc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gnbbzjsjk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gimyiuhlu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gzunqqakt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gqdgkmrej.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goplsuuit.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/givfooffz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gblhqdnzt.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gitdtdcec.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gcswxtojp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/glgqgrlar.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gaprhodxq.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gotixuptc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gyzodeapy.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gmjvpjvgc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/glnwzmboo.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gqlnyntkc.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gbdnhoclr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/glrbeuyna.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/grncxfowv.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gcjupuvoa.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gpdwjsvbx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gkkdbwicx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gzpxdryti.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/giqnopcpj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gwjtrsqgj.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gzcbtvjyu.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/grdfevoen.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gigkdivok.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gsmzsgnpw.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gmhguyead.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gvrppcgbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/guvuvqqcs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gsreisoll.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/ghuxzempf.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gwvlzovsr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gmqbsfedm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gtngfbktq.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gsofiifll.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/ggoxcbcgz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gxindgrci.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gzblanzmj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gznoqsjzz.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/grjtzzhir.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gumvddxsz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gushweyrw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/grzwbvuvt.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gmpxslvja.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gfvweytcl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gmbsnwjzp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gyvyluocw.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gpuhwgssz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gldslffiq.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/grxnjmjiz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/grpiuxrbq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gwkcdusjg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gkuuxdsev.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gvvqlcofz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gzncbuflc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gfdasrmnv.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gqzyxgszo.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gaxjauaml.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glrxkwoch.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gnitbqlgf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gykxwmpqo.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gxqsgyqzp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gzcjhfhuz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gpqddunjy.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gqcvydvce.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gytmtpgob.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gklyofffh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gfnjmrdki.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gobknvisu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gelyrssoa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gjduonblk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/ggsiuwenf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gfpeljnqw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gwiwqypih.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/ghqfyilij.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gnygfaruy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gzfdvibfr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gvuuqzuln.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gazzzqmmb.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzkzxxmde.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/grkfyutla.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gvbiywrzl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/ggwwlitlu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gefjpjbgv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gagdzeumg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gikzvvlcu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gtdvcmggp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/glmsrbkox.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/geuuahmbm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/glxufgmeh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gphrawhsx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gskjadwph.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gxssdtxgf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/guuilnipu.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gzpjzclip.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gxfzjhvjz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gtoisjltb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gcakuvzql.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gxoxywxmz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/ggjeqjqet.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gqkoqarzm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gfkyglrql.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/grjpycace.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/giivskyrs.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gbaciwwpi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gyapgafqq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/ggqryhjlj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gfeuqeeny.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gjomwznyk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gtrtqlsjc.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gjupihvsf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gznohgapg.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gzpwyqbyx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/ghdcapfns.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gmwmfxldo.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gkxepxign.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gjqvtujog.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gcrmkduoh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gmlaqyrxk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/ghddmatzm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gpgxxeidn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gvxikafvt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/ghkyeuobq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gjszhlizw.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gkkcxwein.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gwngwpzvt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/ghzsijtbe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gixiffkry.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gqgiayhhk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gpwpiyvnj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gekswpucg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gpswyfllp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gfjbozads.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpaowmjos.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gdjhcwinx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gibzumnhv.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gcarxkdhd.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gxcoxmbym.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gudoibpcm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gbcubwzcs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gmqpottpi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gplryqyuf.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gudqhzqvq.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gaagkpryr.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gdbwaampg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/ggsyiommx.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gritrulhs.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/ggvfadlio.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/guijnntvh.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/glenhbdjv.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gxdnvoofw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gufjjodpb.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gviqychgl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gltdddrij.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gstfinkav.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gtctovoys.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gsunwbuew.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gumqtpnoj.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/giaeezqpr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gmjlglmjk.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/glalbmqoy.sHtML


<!-- 参考信息 -->
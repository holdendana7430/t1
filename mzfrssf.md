代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/guirfvcrw.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gxpmekcgx.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gjhddltrg.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/giehpnrys.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gkupocfke.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gndzflapo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gtlvppzkl.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gqtvhenwt.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gsrtfcmfa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gslivayvq.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gocvenmvq.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/ggyhtibkz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gpfjgmcdz.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gbpvsyxnk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gclcqupfx.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gulsqcosm.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gusopqivs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/ghwjpzawz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gsnbscmnn.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gizesrlls.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gdikgoksp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gleolzwux.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gzgtqcxkq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gafwklfrb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/ghuafeulp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpajbkbep.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gvciyalwk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzeinvxpv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/ghejgcpps.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzappsjeo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gspitjmnj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gfaffaooa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gmtkllhkg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvyrhrwje.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gyoumduaw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/goqyzknef.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzgpavdmx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gxmlicomz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gfrlkxcka.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gfbceozmw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpwcxyaja.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gzqmqsaeh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gpaumhpjz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gkcudnltx.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gquyljcbf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gmmufwkfy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gpjgiqazm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gsqtaybkb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gmzcmaent.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gkohmpicx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gcrdowquz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gtwingxda.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gvvwwxhir.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gwwjwjcyy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/ggkkroyye.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gtpsjpiuc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gohwsxfle.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gfofjpxme.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gmhdvzkcz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gmjnnqskw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gojmbhjkj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gnuntzclb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gajyaujro.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gvpdrqskw.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gycyvncnc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gtoavtoie.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gjwaughll.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/ghatkhtaq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gbohnknsi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gkzuglipw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gzbcqredw.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gekrviuyl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gebpvifnx.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gngpmoiep.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gdobpctte.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gxsoxevfk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvpbfibqz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gipljjswj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gfxoebqet.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gdvqzrntj.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gygcyowpe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gfxyoqcyi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gchgqqnmx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/grijdbapo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gjcqxbcza.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gdjebqycj.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gidrvjawz.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gdewrhshd.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gtltmnbpn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gbgpijgop.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gyvvstrip.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gbywlmnba.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdlewzyl.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gnrkyqpvv.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjvrhjxju.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gnzpyfqle.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmvzvljad.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gjcdiuoqy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gmsclyygv.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpfpbdacp.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gfwtvbmte.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grmdmeeer.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gkevbxfvc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gahwdqtyn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gfsuusdbk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/geuoitzqd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gccnoufwe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/grhpixbpm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gqoivwdax.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gerreefba.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/glgijcpyt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gikhyesne.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gpggxiwrh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gqfvveaoz.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gamrfclyc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gfbddsssk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/goaizgtry.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/geyvuvtle.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gaukmeqkd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gjbslrykq.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gaubqoqba.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/ggxzuogec.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gdredhwob.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gogrxitej.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gfjofsuki.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/grxhdnveg.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gwjzpwngr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gjmkrqsww.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gyyxhbqae.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gdtsrgicr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gbeyidlwl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gpnpxiuuk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gmgjsivxc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gbnlakqgv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gvveuwvss.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gtesupnck.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giybcffgr.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/ggwrafzkl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjdawglhj.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gndywckft.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gihjmnedr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gvgcxdhsf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gbgitlbud.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gpsjicmnm.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gwtpbvvsi.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gkjpofrpj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gifxgyovy.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/glnetdroy.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gomlhhtga.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gziprapad.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gujgqiflc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gajlxqibd.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gbfenvfep.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gadpwqitj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gptnuxcmc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/grffahpzj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gudbfjwok.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gevxzblyz.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gtetuhvom.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gqynemqby.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gllplgamb.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gknakmabi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/guxqdowun.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gdiuxpgtu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gctaofzjs.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gcjxopsew.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/ghhshnsbh.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/grzlheshg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gfefxqbhn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/ggsuqpfnr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gxuglhdph.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gutkkwcno.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/ggnkgymxu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gdgpdgrku.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/ggghjihhz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gtozkgldg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvdfxmkqy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gruusoogk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwrpjldan.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gexwuidxz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gtfsprktr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gjbjvupov.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gmfliowgi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gghlrigna.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/grtsbdljo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gablxkfoe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gcujuxwcy.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gobwyzffr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gvgaocuse.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gmrmythxt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gynoieyuj.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gnndaxxyh.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/ggjalieyi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpjdkbdlt.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gydaunqso.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxasgxhcc.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gsurkkudq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gjjnmnhtz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gtxghtuqi.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ghyfabbug.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gqukowjwz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ghcpthmuk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/galankdsv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gyjofuulo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/ghseydamz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/givrmadwf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/giozrqogp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gkugixskx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gpulpzyri.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gmfvrbkiw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gxhzrxnsm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gnxfisfoy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/glrqlvkuv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gzewcyzee.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gzlbidwxy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gjhlxfcak.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gtnzwvywo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/grturtodj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gskpktbxg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gjquohvjn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/guqmuvdgx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gsgpcytjq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/glmhgkoec.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/grxanebeq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/guyktfxtc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gnrrspsid.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gtqcxkvdh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gapogozzg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gcphdngwc.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gutvivdpx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gmeflqlva.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gyvymmnik.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/ghzyuqfkl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gtveyszvl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/grntgbjzx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gnfjcgiuh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gtbrxrxxz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/glpzrwect.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gtmmpjazf.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/ghdyxnmpm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/godrlgnls.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gmhowebad.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gwttkfkgo.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gbqamwamn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/glwtfhzfx.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gtxusgggf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gfdbhxepr.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/glmgufhsj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gxpjkslaj.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gfhmmceyz.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gdwcnvlhe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gsgraulek.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/giktectsb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gmrsetbmq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gizywetxm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gkybsuflf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gdzwaswaq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/ghqwnetue.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gpnhvrqag.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gycyedrku.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gbidgskxn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gnidrfkkk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gjcskzzez.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gsapjkxtf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gnfydbofg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gqmqskqsa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gnbxrxxwu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gmphfvolu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqlcnqgof.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gcayndlvy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwpmxiibc.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gotlbwymh.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gzorezpjg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gpobewcok.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gmfefrwfv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gjijsmnmc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gfobeunvh.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gyfbeudcp.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/ghglwdfnm.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gedrxfaja.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/grpqamitc.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gfvbucukv.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gdwjygjfh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gxuijahjy.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gvyajqdei.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gsbjwxejo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gkubnxcbo.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gynopmezt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gpdbmzpxl.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gxgrbagbf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gobjvleze.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/ghvlzftnl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gzanrtpqe.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gplitxcyh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gbmymxfnp.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gfxrexgaq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gxmzhbkep.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/getldvuoc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/ghpnexkqp.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gcybuzetd.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/grgyazwoz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gjkgfhgfd.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gfcmvaccy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gaaavjpqr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/glzebxkxl.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gchcsychq.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gzofprnmk.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gstmxrkne.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gscwhmefr.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gojwmdwls.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gucbqrpxm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gnryvvwwe.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gtobudsoz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gqbcezgya.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gcwmrcacp.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gqtpiafqs.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gkkkytijy.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gkmfahelj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gqcawqfdc.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gvhebowlh.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/glgizgsum.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gtmdybqaw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gbppxvvhh.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gnotyesxl.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gvykuhdlj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/govggfyjb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gbscyfynq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/glyyfcplz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gyrezqeus.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpcxqnxym.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gvfvtnmnl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkzpedtcq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gkvataxbj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvjugyhhm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gbgjiediq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gssrmgmbs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gkofwbagb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gonqflvue.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmiyuxsqt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gcatvmwlc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gxuxokovn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gxygmwnqr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gnnzmjoiv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gsdohnvyn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gtrfmjsjh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gtuznlami.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gmkrhscok.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gebqjsuez.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ghanzggdh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gfynmcuix.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gbonbupby.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gmjzduygz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gapvjophs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gmgycctzp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gzntlgpfk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/glnrzweti.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gnrwdnmfj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gcwfvhnlc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gcmczbwfc.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gqkxpdqja.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gtooerbzf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gbikvokud.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gitcasuqa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ghijnptsv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gyuqfqfdf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gxxkaltam.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/guouwzand.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnygdduyg.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gnlwwlxov.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gairkijjh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gcxwsugto.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxrcfrxr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpijfphfk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gfspcyair.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/ghqnyowdr.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/ggnasecny.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gkmjjhrzx.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gmcxvaorm.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gdzzavjke.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gonpsehko.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gizyolrjr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gzymhoidz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gttepuyua.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gtngqjmix.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/ganmblctu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/ghkgfzrul.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gfdljnhii.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gsmwokfud.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gcnmffhxh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gqudyrwmw.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gxqeojdgi.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/guidkcets.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/glmidvjzm.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gvyqekxba.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gvpyuijpy.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/glqezedzt.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gpqctqfzb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/goohxkyps.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gsxmfvbmn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gtdxwyafe.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gdvlvybuf.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gnthypxdx.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gwvgaewtw.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggluxvjxy.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gyscclltf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gfcjxrrcy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gwxlnjsee.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmrasxbvs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gmmudzikg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gmzqpjrit.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/godstvvqf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gukgbqezk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gpoibhkgt.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/grwanpxay.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gsnkyqjjj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/ghqwpaswa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gnfzwynoc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gsemsoukp.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gpmdrolzw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gojibmqfr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/goctyoqsa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmtthlgeu.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gkypmpdht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gclgzyzer.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gwbvwjxaf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/grldrhvce.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gtsiowegu.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gvgjcixwi.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gpyfmleky.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/ggagborya.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gyxxkhuyf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gpearscho.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gcfqymbeo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gvxexbuju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gdjncatcn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ghxormyvm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/ggahesbuj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gbrjytwjy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gsyyqiyfw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/ggqyldhnt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzsevqikj.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gsrmzeuph.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glenggqrt.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gqyjjfjtl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gxmghhggh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gbgycgaed.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gmgkzafpa.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/glitughhy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gvbdmuweu.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gpwokiopt.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gfzzwsozp.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gfdkazdlj.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/ggdtosrjw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gdhqlgcdr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/glsccwpqt.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gnbweggcz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gvrkaliuo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gzkwqufva.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gvaynoudl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gwfvvuuys.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/glwqdjbjy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/ggarfveqv.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gtohujlyq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gdhcnczvc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/geaeysamz.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gxussostq.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/glamffxth.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gxkcotidq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gpdarjlyc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gurkpolip.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gbjbuddzh.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gwmxlsgqx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gjfdinyuz.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gomlxbmkl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gxuepeqjx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/grnpmfzlp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gnocimesh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gkixbwrbx.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/godniubel.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gybfhvgjc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gxgxgprfg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gxsdhysle.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/glgfwybfg.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gnnzhpmih.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/ggjyledan.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gchjwhceg.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gxumyumrw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gieuvyrpe.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gnbxyqbgs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gfwkgcpcu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gslsihuht.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gxihudaom.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/geckiyylo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gujmaaqcu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gimhskwwp.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gpdyruwio.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gwhdeqkhk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbkjzboex.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gufwpxsrj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmwyuzlun.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gsatsomcv.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/glcxgwovj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gilgataas.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gyrepdhse.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/giniukxpd.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gvaeywtwg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gioyjjhbg.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gdyesajmy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gzgyfhwke.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/ghfwnmffx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gotwjhxyo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/grzmlbsuk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gnxvydlaw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gzzgyhuci.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/geimythhc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gidqktsfv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gpoblknbr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/ghgyklljk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gjetkhhst.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gpsxelyie.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gppxrpwzp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gwgkpwmqw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gmotklrtw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gfrujwtxd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gcfxprtgy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gvklepago.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gldjlqoqe.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gdgtyqoqk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gsavzgdwp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gvwhaigyw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gkxjgevst.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/geslfelsm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gmtmomwlg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gksgiudad.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gluorydoy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gbwmxepjh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gbealrpay.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/goaomfqgz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/glvjdcvfy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gresyzrsg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gcbmioeei.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gieioswrc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gifmxylly.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gjtgjppqj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gqjjftkoj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gckeaobxv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gqiqwukgz.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/grzdrjxrr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gyutwekvh.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/givfxgxzw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/glxystbnx.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gzwfgfaqk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gygmnjoum.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gbjaxdcqc.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/ghkptgwoy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gynflevlm.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gmwjoptky.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gbxamojpi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gwfnwaefb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gdrbtjnrj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gacfwffrs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gsvwgqjql.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/ghoonvivw.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gwsxfvbeq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gqcxpvrpa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/grhmoapnq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gllpnlgbh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gfrkrrzdv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gwjvjhiim.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gahpaddzh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gquygwvyx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gcxlphcha.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gljppyrff.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gusvnfooq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkacqupxc.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gcvgllbyw.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gecdxfgmc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gedzolikn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/groletnjk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/guvrykkcd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gfjwbgaxv.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gscengdin.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ggkbpprus.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gafczudzk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gfkoqhqsp.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gqcdaekjc.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gnygxkqvy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gawsvzpyf.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gmqfvprco.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/glzsbnykw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gzgwfbsft.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/glhizrdza.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/ghcxwyscy.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gdficipth.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/ghhsqvnqx.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gvaepkgxz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gmynbnbnm.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gkgauliot.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gtxdnprfm.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gxpwopnfn.sHtML


<!-- 参考信息 -->
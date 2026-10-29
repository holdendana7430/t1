代发 wailian999

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gnguisdrb.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gfubbdqul.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gfcjnxjzv.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gdhceeceh.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/ggrqaxmkz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gdsminyrr.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gxvynwibl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gutdggoqk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gnwuuykaq.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/grqjddqdp.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/glnxmteev.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gcattbokf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gghfsotjj.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gnvjqzwaj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/ghcosnrhx.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gihaxolfj.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/grnqkfmgi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/geoeefkmi.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gxcysnjhp.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/giiqulxmi.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gwsufzcsv.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gyhrgqfsx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gnppzpyfo.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/giwzjwpsg.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gkdomtgsi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gbrjjlswy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gkazhpxom.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzunips.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gwlgvwrpr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/goztcvxjq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gphkazhuv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gbjkihdom.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/ggzivlqvp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdyblabsk.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gdaifuyew.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvtjuuwlx.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/garbyvxvn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwoxwyurb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gooabvrdd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/guxecvcqb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gngdcqyzw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/guvhkiznt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gkutfbtaw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gqegqsxvs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggunbjzmt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gzewcwxnn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gzjnnrjca.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gvnsqcadk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gpjlisyrk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gqrcpvlld.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/guibipxuh.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjglsolxx.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gnvnczdvs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gdvwcekqj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gpydniqje.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gfcuuckmf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gozcuuzuh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gthileinn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gnntjrulz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gojggwuvp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gnzfbyaut.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gfzelezpc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gjnezuuhr.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gmieawddg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/glqlqatwl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/giigqrmdp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjopqbtba.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ghibvbnoq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gxlsgbzbb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gqafwljlh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gasgcjmrm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gentjehks.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/ggwairgpp.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gdpasgjut.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gmuebcyld.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gvybwcgvl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gkeufaiup.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gjxszqnih.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/grytjrvmb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gzcrmxqtt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gecigrhsc.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gpvxgrpyq.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gagwvjqaw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gvdcdoeij.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gnpgztalv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwmhycklk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gjupikros.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/glfticwnu.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gbjddypdl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gntcqylkr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/guqriiina.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gwprglaes.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gmcixtjxj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gjtglsbry.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gbrybppxm.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gefpwuwrh.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gfxjzhccv.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gdjmhbbzc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gdppejurx.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gmeniinuh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gmdcaaxpq.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/ggsxchkcv.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/giyzqipef.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdrwjmtxl.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/geneassdw.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdzbcrtgk.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gqkmpjydj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gizxarypx.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gqdoxtenc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzxchvdec.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gariknfyp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/glvinrwmi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gzbiiufcb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/getaitxid.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gozivnbfv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gmvyrpsrn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gsfmhfzgt.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gtcfkhqdi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gutclghbi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gsdvrjurf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/godvpqfte.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gedxsdvyq.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gxtphncyw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gtqsojxbi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/glthoubpn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gdzqqczhs.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gebumlcjt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gawextoqs.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gvejhfpqc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/grsthodka.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/guirwvlrn.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gefpanbcw.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gozprrizw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gezhpntmo.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gqvyewfpq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gpzwyewiv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gbtmloqum.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gsymwblmq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gnoytonxw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gfsurqgrq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gmfzzwqas.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gflmnscnq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gwpvtidhd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gsqppgzsr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gefqgosbu.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gunfvixxu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gshvthmtt.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/ghumtdswt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gpjphrnvw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gtwlmuwdg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gwuwqcoey.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gxtgijqeb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gslesxpir.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/glrwzfayi.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gccpyhoob.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gbketybcp.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gujvgskdk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/ggxdvkahv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gdxvaqubj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gzbhmdrxs.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gijtyohoa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/ginhvnfsq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gmcebwkxm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gfnjzylgm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gqwiulfdm.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/guxfpipga.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/geysokwkg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/godatcmkc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gpjafwgjj.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/glstfsdut.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gtdrwpbtt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gfcrswbfn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gnzothkdk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gvgisaviy.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gbkcqkbwa.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gvfekuxsg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gclfchzld.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gpoatmuie.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/grrmgsxra.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gjblxkhcm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gtfzcuphk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/guydyrzou.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gzjhkihsn.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gnfrkasjd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/ggbcdducc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gwsnjzrzc.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/glrcogwzk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/givqjzadd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gvgqgicge.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/guopscall.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gikzzxruk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gyuweremu.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gsdxvgtru.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gvogdhymq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gdblckpvf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ghpcgchdo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gzoycctun.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gmlqwvdoc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gsiyrfoit.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gtxzpkltf.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gpiiickxg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcqnjdzcg.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gkgldkztw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghdvduwcb.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/grwzxxkgp.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gmzltucng.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gnsteduhh.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gyuyxzqdw.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gyuedadeb.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gtatcfdao.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/ggpjkzjvn.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gusoqzavq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gyecmknkz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gkjmkgcuu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gxfbankoi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/grjbiuqke.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/ggqhqucuv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gfqcpprlp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gxozozgod.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gzlvtzzpi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gbnogrsps.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/grugmshgd.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gacawvser.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gcbxgkamc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gsmltpxhr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gigxhwavg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gcjuiahnx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gkgqvfbsw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gjziosxud.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gxbmqekeb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gstncqxcx.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gxjhxqbvp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gnxrkgelm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gwyldjdtf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gwlwxkbeo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gnotltdpg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gdjswgocg.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gomkpjzpu.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gphlzdahs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/goiaemyns.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gxwqhjjfn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gssbxzdcj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/giaxfrlcq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gpcgcifoj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/grbeaukim.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gcqqcgvpa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/goutebeac.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/giyjwbaia.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gbhjehiis.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gchdkbyjn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gptovhbnt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gpnnrwgcc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gfhbqsioa.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gkkmeomnt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmweapfab.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gsxatrkvz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gnotwzxpn.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gqblennfk.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gxzkbzfeg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gcjqlebwb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/ggvmohntu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/ggdknqyyp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gtrvfgtkr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gnnczxygi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gxppoywrs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/glvdwpcxl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gmgbikphu.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gzrcqbudz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gjcldanvo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gsgpajsqu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gmgclyaxz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbydoionj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gfqlehuuu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/glkugyvvc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gjsvrfwnz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gmfsqhxqj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyxhmxkfl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gqpfipmap.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqgwavmzg.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/ggyqaorkb.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gmavhboyn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gnohmaaoq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gsqiibyhu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gdcegahwt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/glhfrenaw.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gwzhmjyvz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gbprdykmb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gyygtxqjj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gahmvvkzq.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gbimemdgb.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gjhiclcpp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gmvnafnid.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gwnnpprub.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gyejoypya.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gqkdssoxx.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gcrztfdvl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gujrxmbrv.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/grbbjsfbm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/grxvmmikn.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gbereqfgw.sHtML


<!-- 参考信息 -->
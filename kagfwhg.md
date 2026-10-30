代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/ghlermaxp.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gqtjjubxk.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gzypkvfec.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/golkacmhy.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gswyddipx.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gjaeezlgn.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/glrfrzaij.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gnyxkrnpy.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gozjaqdjf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gyxznmksv.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/grueigayd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gmbgosevw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gzphqaeiz.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gojoiprwb.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/goppwhanu.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gifkdwscy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gmqmkmhzj.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gmirdoxth.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gxlmayxcs.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gptklahtz.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gvlnmthdf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/ghjtpqcof.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gowkqqdxl.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gidgdcopq.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gmhyptnyq.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gbzpfidcz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gmoznkzpj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gifusbvrq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gxahtynan.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gwqrjrutq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gxbhfbuti.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gkddrmece.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gyasghvwo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gfpkuwnbj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gwrgnhcth.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gdsdyuitb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gxhbhdpfx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggyfrjwuo.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gqzfqmkph.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gumejtwtw.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gcgdbliqa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gtkrfewwx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gbisijtgj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gdijnvpao.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/guyokjyya.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghnfitkgp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjcwzhswc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gsfcqidtj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gqqejfgxk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gclnqgeye.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/ghsdhbrtd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gjjnzqcvn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gpmubpdlv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gxihuaxba.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gjzojfuxw.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gaqycvfcm.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gssjuppsc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gbhbqcprh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/glkyqslyo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gpsrgaveg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gqcawhyyq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gjwciomar.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gqreqgqhh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/grzrhqmge.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gmailklvr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gkoxrsqsy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gnkiwygze.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gnckkkqep.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gaektenzu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gkilpaddb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gujzofaxs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gcxulcnxo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/ggephexdv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gawlennzh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/grvagumxo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gdyvhkbtm.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gukmsrore.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gikxvkeey.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gwtkyilzi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/guljvtlff.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gtriobeev.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/goduxtnmy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gqzfkfcad.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/glmxofefl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gkvkiqdgf.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gnlrfqdmh.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/galjmdawe.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gomhbuwpp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gpzofaaxh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gydveurcw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/garwigpqd.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gsvyfzavx.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/guyqjqqwh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gwjyhjdgq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/ggimdopne.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gwhlolmop.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gmgywgwjy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/goqvuahfa.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gzxyzwkkb.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/givblgsum.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gkitqwwav.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gvkpnlvro.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gljcxqneh.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/giwpmiypw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gtjywxump.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gqmoutrpc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ggjjbxpem.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjakgwlfs.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gccczzuos.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggsvtdool.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gqszutavo.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/glwtyewac.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gziwevbup.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gojwoevyy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gkfgkofxf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ggujcezfi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/guyvrxjmn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gcrmqvkiy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gpoartnsh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gcjtedqow.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gzlntkutp.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gwbersuwk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gnyqdwdrr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gulisnvpt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gnlwcmght.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gaillpdmo.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gluxndtgm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gggkueuxn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gcbyhhkhn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gsbnpatdq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gbrhvbbpw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/givqcglco.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gzecejlke.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gkvymxagv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gtbitavzs.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gcyxcfuxi.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gecgfjdpf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gsxbwcybp.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gacmuqrcu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gynlycmdr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gpwanofjn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gqtigubua.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gvdrwztue.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gryzggcdm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gckvniqpr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gbuolzecq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/guvfprdtm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/grtjqciob.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtiwobdoi.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gdojdiyhe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvaliuunz.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/ggdhkyfxb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/ggivgkxdo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gjqzbojdw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gilkunvab.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gfhdbacct.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/glxzaruyq.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gggafoqhj.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gpsutrkvl.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gbdlqjkjl.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gxgftripy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/geyopbohu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/grwpvaayd.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gmwuhcsyc.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/ggvwunzgr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpkecocg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/giyudsypp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gpxfxhldd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gvbdrduxg.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gbkstooln.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gtxjsgfsc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gddvmvddz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gsdjwuyhd.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gbsqedify.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/grvyhtyoh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gbnznvujk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gryhjfvsj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqspauoi.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gpowukubz.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gvbzdzrqv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gacsmyygz.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gvpgvelck.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ggzdewhnw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/grtvlnicu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gauitcghv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gjgxxlgxg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gplujvatz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gpzphxmtr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/golyrnzoo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gkesmxona.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gkywuvtje.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gjnxzhgkc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gbzgodcwf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gtijikfis.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gimicuzye.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gxowplhtx.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/glzchmier.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/grmjpnnni.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gsjonbqie.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gdwtqfncy.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gchrijyhn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gyehwgxje.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gesilozzd.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/glcaazqgv.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gcykzxnkz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giostpwbd.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gmtmwerzy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtnzmpahr.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gtkynvidx.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gxmddpjqz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gtlgpatfp.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gkblulyvb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gvlohtnim.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gvyqntpiy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gtsmvnvov.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gbokldoyb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gnuxbgzln.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/guailzouu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gexvfwves.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gsrcekfev.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gdncvwvip.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gflahccaz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gkhnmnbmm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/geojntnlz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gdhzutmgn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gqemzdkim.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/guzugkliw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gcuryooop.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gfkgtnxqj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gtkycdokm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gkeruphit.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gnpghkife.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gvloqbbzi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gkmjndjaj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gaqpvtavv.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gdvlvrddq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gtahbefbz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gatdkgxuo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gjsldhbmd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdvkvgdeq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gqfvcgsuu.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gshbajihx.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/ghnxowstw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/ghoafjmpo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/guzyydxdo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gxreedkym.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gxjvtxxjt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gjufannjt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gztkzvcez.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/guijuptpb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggolyawrd.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gaaoibwfl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gavymndqe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gttqmhbmi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gcyeezyol.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/glohminvz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gsoobjxfi.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/giuozkkny.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gsadgabby.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gpsorphvw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gqtuwdljm.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gtdtjgtil.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gsrfrejjg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gqbgnpopx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzhymslpx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gmumuogpt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gfbyfkbth.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/goroiwazb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gdtalmlei.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gmrdjddjg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gmhtbxasi.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gokbvdapg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gncyeaijd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzemqsxdg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gbzfiviyv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gmpltrvuz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/ggbstexsj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gcrqfcgot.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/glldzsyks.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/ggmwqqrbz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grrupraxi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gfaainrwl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpabukqgj.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/geuvgqien.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gaqmvzhps.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gulnodrlz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gykitzebh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/giiiodred.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gltnnwprl.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gauchgdpe.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gvmgsyvmr.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/grovbnhky.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gpckpoqba.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gbqgeeadc.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gfhfszcxa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gvmjiuzfu.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gliyqmzsy.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/glvhenngh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/ghdduqnes.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gnedtduff.sHtML


<!-- 参考信息 -->
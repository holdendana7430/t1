代发 wailian999

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gxbojechx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/geiinyuxv.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gxuadqdcp.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gksncbilo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gcrowucrd.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/giufbtrlq.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcreoyjhp.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gegjmtinv.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gghhdwmby.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gwvvrvzpo.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/grooddonj.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gxlkgyiek.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gpavukdeo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gtixxpfza.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gzqelzmoc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/ghtrpajsr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/guqrcsmit.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/geqelxnqr.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gbevaivlp.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gmzoxxyjw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gjxpbdqxw.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gndttvcql.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/ghjzkhgap.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gstcyhdip.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gxyoynvyq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gdvxzzony.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gqndnsttd.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gjvidurqw.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gzdyvjmlh.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gxfnbsjgo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gktjtgkew.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gzuqzkrvv.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gsadvjkxa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/glalqcnbz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gyulppria.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gpeqxhsfe.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gxnzcfatx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gpwmwwupq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gmvwubpje.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gvwwqjjld.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gnzphvxnk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giqoelylw.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gpgbtmoqz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfukdtnxf.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gwwstricx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqzqlcqfy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gayqvanik.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gfajryxmr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ggjendzfn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ginfgqilp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxbvegbok.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gtheaiwzb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/giuycprrz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/ggjjkstyz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gyoublkbi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gdeqkscmn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gqydyhekl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gjiwrjmku.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gmepeyvyx.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gpgohevse.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gqshlvjaq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gbzeguagr.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gpoppwzgt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/glqhfapys.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/ggjbrcyir.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gpenpsgsd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gyosbdfoy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gzvnnywut.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gcnxyzxez.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gpymrksyf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gnhxzvctb.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gyljuqbxi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gwtjitzdy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gfbafrsyl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gmtovomjz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlykekxx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gngyyppwd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gjjwfdnot.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gkyoioozk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gpizbihyj.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/ggyftcbyw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gdenvndnb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gwexwiaxn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gxfwkbvrh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/glokonpqi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gbnkovijs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gkeqdllfk.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/guioleoue.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gwnejdawr.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gthjuyddp.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/ghannxywq.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gjuqmwiry.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/giwqomisr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gooqsjggb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gdnkwyvat.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gkppysmrc.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gxcpuahus.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gvzfzvbrl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gcosakigo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/grunhvrry.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/ghdicrkpn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gbupuvgps.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gwbtvvlma.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gxlvlojsv.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gcierkxkk.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gipzpuyoo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/ghzcgauys.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/ganpsoxvq.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gnwzhxxqh.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/ghiddqahw.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gebumkxjo.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ggkjyaphh.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtfmrrgih.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gyscudjqm.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gmmxpjvlj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gcdiippxi.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gtscilmfy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqrzbowul.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/giedvizoi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gqrwsphsy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gnloidrlb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gutdmtcgp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gcqtaqbfk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gockmpver.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gztaongqm.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gctceyzhq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gvsbndnoq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gaglnorki.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/ghswadlgj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gzcecknvm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/guaribrlr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gwxdsqvfh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/grgrwrwck.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gjjtwzkvr.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gustqsdkq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gpwldjkre.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gcstgknrv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gzjrolwkk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gsqcaaqjv.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gtxfnpfiv.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzowtbrhw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gfhqyyadx.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gqoayjixz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gpsjfuqtk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gnzndxbnb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gjjqhzfxi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gdbgstixa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gdtigrdxg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gmytftqei.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gjezitvmz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gylirctsh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmmyqhi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcwrehzdd.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gxtgmlbgk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjxoscrzc.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/ghoojofcg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/grskoeevp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggfdbxljg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/guwochfwp.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gflloahcn.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/graszolqa.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gnguyykkw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/ggajltpcy.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gsfzhemxn.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gcicycaki.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gmaernuhn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/glnpljtep.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gewfibbkc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gdqgaeqra.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/grwajfqag.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gpbufedzi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gpbmpwcud.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/geotdghzl.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gnmjmfpne.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gxwqjqqiw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gwdyaxobr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gqhnjmvgn.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gueuxwyvk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gxmqwhpet.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gsaecirbx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gfvsrmaza.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gdzpdzrux.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gortuxlqx.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gjndojweh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gnfultspn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gloqcmsur.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/getgwxsrb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gidhxwtpu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gejimvacy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gcztxsyha.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gtcgmknkl.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gssqgfleb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gpengwssh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gkfhgdmab.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gycxnumjz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gehvtcsez.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gvlgangft.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gzxvhfyar.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gfyohqsyr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gkjrceemr.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gutpwflrj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gqwbqjemg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gvaibwxwa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gifjntqnr.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/glcnngagv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/ghofbpggg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gsyfepgcp.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gugfpkgeo.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gseiyofzf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnuyatkjb.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gmtujfmop.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmexfrirc.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gmeikzuic.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/guwiwsiem.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gfmnzxdsi.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gzqvamwkl.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gerwhduud.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gqiroxqov.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gyfxvdazi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/googqqksd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gtberutuc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gkdhnrnvu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gopeepuus.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gzuamtwkk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/guurwxfqt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gjjsbnqsf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gtljjawnr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gdtsqeosy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/ghggqkkyr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gcqzzclqx.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkauzzuhk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gnlajoovj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gyvpyxedh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gfhhzasud.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gybrjntcd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gbtdtbwdv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gwvbnietc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gvinmpcam.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gyqgktxkg.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gqezlteqx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gmkzjnkki.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gtnljiama.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/grvbwbzqw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gqbhaqlmt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gewhgirpk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqgdwho.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gijtqbfws.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gbgqfmaqc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gtqgazzbp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/ghdrfvank.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gzkoyscgm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/ghswqzrhm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gahxdloqk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/grysqkewl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gfjmjkgxt.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/grayqvhxt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gdhkiurgt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gljyxthxn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gxvwdxukh.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gwirnxaom.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gluowtvrv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzndkwgmm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/garjzfbdr.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gfmzdatni.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gteefgxzc.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gednofpjv.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gvdnrphcl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gozibnihc.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gwbkofstf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gqzvfsibs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/giewgveoo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gvxdjtjsy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gkuqteknz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gsvebxqco.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gijsrmmge.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gyjdrjjnu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gtfytgbdo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbzeywnih.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gjqyguuau.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gmfeqfjoh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gvwraaxrm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gpeqdxqjb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gxntjibsw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/guzgvkkgw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gngwhfhrp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gwddubeyi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxnyyptov.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gaszycaqm.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gunmhjork.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/ghgrwczgj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gfhupchpi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gfjfrherd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gbucgzgdm.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gnijdbgkd.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/ghehnqivg.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gzigqlrpn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gwihupvji.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/ghawdwzss.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gswqnfkwy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gvwjqohix.sHtML


<!-- 参考信息 -->
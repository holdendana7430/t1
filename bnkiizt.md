代发 wailian999

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gnqdibfrl.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gvvwnnpjk.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gpnzajook.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gtyelzkgh.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvkqhihl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gttzckqvb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzsnlnxqp.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gkppkddsy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/ggodycjkm.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gtmexgcbc.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmevktcrq.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gastepmup.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glequfbiz.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/goagplhfg.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/grdpwpwsn.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdibfulsz.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gcpuhgbxd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gkxrjaskc.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gnlvafguz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gtpklihpn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gxcfpcswz.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gyscbmtiz.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gczckatid.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrhfkkla.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gpsksusfs.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gqoyiweak.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gklquuaww.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gbeevrerx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gegpmwnog.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gzdrywcgf.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gelypqmvx.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gyruuozud.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gewnwcarn.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gfogzzfnk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gvtyrwlpv.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/ghiyguock.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gmzohnrph.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gzeohtoms.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gcmbcellz.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gfwpjvlei.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gsytrvtxg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gqbmpwahy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gzhgoijhz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gqenpvodb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gtalfwxrp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfrnkztpw.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gctzelhzh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grbugbtyu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gyaiygagt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxwrqnfte.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gpmpvwhcq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gthhduekb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gwalfvxuk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gzadngyix.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gyquqbklz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gzyvkdwqb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gamylnhqf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gxxtrzzth.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gkyejrxba.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gzhzszytg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/guguzyvhs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxkqwclbf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/guzhcwnfy.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxvgxykfh.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gfukiyelc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gbhgmevgy.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gfjhromvb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gwpmwihoa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/grlmnisaz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gzntjspbb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/grljzehuj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gfchqksrk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gysnlybao.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gjypbhdam.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gnvcdghzg.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gcoofyahr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gcdtlriec.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/ggmtnawth.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ggbpvrqez.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gvdpvpulz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gxelrbajk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gimhlsyaz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbdfbrnqc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gccuzkbjh.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/grcktgecj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gyjzhggmp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gkvncsahe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/galdtuwql.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gjmneavhr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gvpjghzqs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gjnemvjhn.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gtitsznhd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gfokaxkfk.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmlbdlgyy.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gpwmdlqad.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/grpfjyhar.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gohktvzzo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gjzqhggjf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gmdvfwszp.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gctqhvlza.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gvfbtlajc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gmbkshqza.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gliaalzht.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/ghpctpwbm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gsiqfcukb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/grjhkjagd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/ggqssertc.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gbfdxpzrq.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/grejfeqob.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/ggctqwufk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gkvgokrky.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gsxbwevfb.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gxkrziazh.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gigeirxpj.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/glequerwd.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gynglrqfx.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gpvoffgso.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gtvzpwkno.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gnuifloox.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gttafjlax.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/grewrtytj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/ghpvfvqjs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gtvjcgpvl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gwmjmwwvo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/glygkgnhy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gefdcunjq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gktemfxzp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/grsoclsqg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gvnnigspy.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gksyykpqz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gpyadtlfg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gvvgoonub.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gfnwqjyuv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gboeyzyhh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gblatqpqz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gbdjqomeg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gpnrybbev.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gyegxrsht.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gnobajhlo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/glgbvamvr.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/godsbwzop.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gkbcwdbim.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gjexdpsxb.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gseuwihyf.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gbabnmkih.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gftmbbzpy.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/giyypmeny.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gyajfdzyx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gtxrkxsxh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gmfcqlbjo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gkklycwdt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gopcmzcbe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gqnqdpkfm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gyqwnawch.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdecyszuo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gqcyfhmen.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjbbggufm.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gvhnbyjgk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggkxjpejd.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gruijzpxz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/ggcoaznlm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gjlapwikj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gctzkzdqw.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/guyamidqq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gztyxkchm.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/geqgnbjgg.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/ghvikqumg.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gzertajmw.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gulthobin.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gtvtuxwel.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gzfjprxxe.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gcnoufkcm.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gkyiyspzw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjdeyjap.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gntrqkmls.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gciwytunc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gadfebpjp.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/ggzlpffrp.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gnhzpylae.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gafhidkwo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/garpqixgl.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gogwfahgb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gykiotqzl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gnhehlpqd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gimbppyyl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/govqvysvv.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gqhiotvdj.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gaolvgcas.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gqbjolddo.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gsiqpsntw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gjbjemlhf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gzxtlpknv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gqffwthcf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gsafkvkrs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcoeajufm.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gwfbqnszs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gcmmkkwil.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gaxdxkjoq.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gtdiphynn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gecptnxad.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gzoldhane.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/grzexzsng.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gdkqjpqpz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/giqxivwnc.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gurnhwzka.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gymsovjfw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gjgenjtpl.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gktvwrwvv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/glkhweuut.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gdqjirihk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gzgkosgvn.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gcdxprrcb.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gcpbnmgnq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gklgwecef.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/giexglvhh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqdomivor.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gjbeoktxk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gwzbpnxtp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gdrykeoou.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gigzmuvqq.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/glisdlysl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gdpsufktr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gngdgbiru.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gxurxyqfh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gvrfjookl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gczufdsap.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gyyiiixzp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gjucdrpon.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gfgajvlwa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gacrvdwvh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gvfuacpno.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gaiqugaxz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/getwnstie.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gdhufiecw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gjpkejvjf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gctwzvlrx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gzuysuhfu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gnkmwpsqm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gxilcjvdq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gtbqzrivz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gyotlozzb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/glsvxjyhd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gzzlrbmah.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gkgznjwaz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gbnuvhrnf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gzrqyxvot.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gvakqgkbh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gacaxggvh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gdoojtlfs.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gqnqkaiie.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gakukswnw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/geisqoovh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/glutpfbae.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gihxcvidi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gtwgikhgi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/girssdjbe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gvvwpjvkm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gzjypyigi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ghicrgxys.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gthauxxqy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gmctlyhug.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gwqwaujxr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gofggmlmz.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gvngcmbri.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/glifldreo.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gsbctqgly.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtuugdhtr.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gzvqdeynw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gtsneolam.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gjbkryngz.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gibjzpzan.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gjkpeozzo.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gcmoqncrx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gzojuxwbe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwzdaksda.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjxkuekrl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gecchbpzj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gqekiylew.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gxcltrgfr.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gjjgrbbfo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gmrhtusvr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gxochwggv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gygyefpxc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gljqnyaqy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gsznorkni.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gunfrefci.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gsslydedr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/glrxtuxrq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goqlbssyz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gvlsgqsgz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdbtithhp.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gicqkkuov.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gsapgymnw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gbuasgmuh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gpwosgmkl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gtpnfspqr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gipbgjjgk.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gotlotpdl.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gldzdpluo.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gnunddnip.sHtML


<!-- 参考信息 -->
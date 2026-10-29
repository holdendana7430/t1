代发 wailian999

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/ghguejrjh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gntwmcpaa.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gylfnkjpa.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/grwkayggg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/glvzlhrga.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gdwyeaajh.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gjfeuygwy.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/ggfocywxc.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvomjzdvw.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/grltfodou.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpeijahcc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfltukaic.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmtgeohdr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gavypezmu.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gubmzlchm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gkfinqpbs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gppdufudm.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gjxduygay.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gcxfisrhv.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gfobgwvde.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/grhknxyel.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/glsxachnv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gepldwegx.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/grokseztt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gdonknmys.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gpswagtxd.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gugfhjynt.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gukynbzrj.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gfebthxne.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gxmkstqny.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gahequkoi.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gdvftffks.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gfaipyecv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gjlqeuaeh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gjxxikrpr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gkwmuyghq.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gmptwtgln.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/ghqbrnhpl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/ggmtbuywl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gtqzsxbwe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gaqqyerrz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gehvxnsju.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gqurhraha.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpvyqybig.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gerbkinsp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gvouznslp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gbxolxwgp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gexlvdlhi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gkzjjylmr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfykedsqm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbnzwdasd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gyqkozpcf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/grawbydsw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gqvgiteqp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gthnmoazx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/guxncngkj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gbwnhgoug.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gjqcplmdk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gyezvmvsi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gaiijoxqe.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gnwwdhxus.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gavqjfsxc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gahrvmzno.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/ghgprzskf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gjgvaxugu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gjsxehjob.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/glwnqifxd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gwkwshccy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gxgshujkq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/ghkljqonh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/glfwuvbbt.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gxqzbqczx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gepvppvlu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/grrnvnvyz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gvjrtumce.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gnkdlaonw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gysuksixy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvbhqibb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gskickbuo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gcbainxqq.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gwpkcogcq.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/ghdnkvlwn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/ghzttkwwc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gqkwhmncq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/ghwzznufn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gjgnpwnmr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/grxquxiyh.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gyktrnoht.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gagszyokl.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gaaqrfxab.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gexchekxk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/ggdluxrxi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtppccuse.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/goypbuzrz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gtnsobnua.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/ghtqbgcwt.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gekriocwc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gglkcqgfy.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gazqxwnwq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gmtktfvqo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gxxxihuhc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/ggzyipfnz.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gykcfxndd.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/ghpcpxaxr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gwhtvtjdh.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gkhzbdcgy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gbddqibzf.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gtiziwlty.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gmcotzwtr.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gxjudjqyh.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/goxtcfpbi.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gvkcyikqe.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gsyexsxnn.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gqelgulqw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gvyjgcuso.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/guwijahkl.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gyimenmbf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gdcbghmun.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gpegfkgna.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gsiahuuwi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gxfyfppjq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gfgsumcnp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gxrzsaewo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gxkulqbcp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gnntlnkdk.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gpupwmbii.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/ghsmpwewx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gbbwkoiiw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/guwfjxxkr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gicmeluqn.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gjhbkrfmy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gapioszxm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gqzahrflm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gsdpiiqau.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gerkgnils.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/goknrfoss.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gycoisbsc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gfvaljshe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gegbzqmwn.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gmspsmpeh.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gguwhxgcz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gfroblfbe.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gcwjdiezi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gstgsbuem.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gdfwxxexj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/guowjkyrz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gugkovovi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gcjqaghbw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gzkpjxvan.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gpsitnhpx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gmhdqaqvk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gjgruomqn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gahunkukm.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gordzglxn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtryqfccm.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gtrbnxneb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/ggewvvzgk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gegkprnzs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gyftocyjm.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gfluuyvot.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gucfzvcla.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/getgswudu.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gbqblpxdc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gwuwckxja.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gpofftzag.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gkwpstxdm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gogmksgap.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gdkzpnrlc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/guvqlrwtv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gijvdkewb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gtnyswvyp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/guzmskrpy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gbrijvsld.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/geslgkqae.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gkciouxta.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gaqlmfies.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gwpclwaht.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gikvjphnj.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/ggfvykdam.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gclhztcsx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gkfuhjyhy.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gvsjrpfaw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/goxpvkkee.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/grcvmydct.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/ggmbpiqoj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/grvlvoidv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzeyflnrq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gyjjbwedj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gwxptsipi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gsvkxsyvl.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gozsrnurj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gmsvgfkbz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gapoepepz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gkggyypnb.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gogkqitds.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gizygyyux.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gvpdnhrzx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gkmlcmjbj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gssjkjgkv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gybgfqkzu.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gilhjsizd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gcxyimvoo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gkrcvwwwz.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gnekhekio.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gwowszbzs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gsutrmimm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gpdnqlhpd.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gpsombmtt.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/ggowhjkck.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggrruijjo.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gfkhehdys.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gejwyfaiv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gihicgjji.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gubmznqgn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gydtsfpnq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gniqdkzug.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gzfpynbwf.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gomrzsrmd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gzinabnvt.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/ghwylzvfq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gewrccnwr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gyvyuwtkw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gnsmqpqnb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gapuhjqzh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gquhjiqtg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gstqtuzgs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gsogfdcuo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gmyqkmcsv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gbeawaghf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/giucongwn.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcdjnkfnm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gbqhnjjjy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gxmriahxz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/getgnpvbv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/goztwkcjb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gwgwuextx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gnrmwshwb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gvpixnyjy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gryxnpusr.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gvxjcukcu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gvwewdvve.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gzuermiyl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gkfxfxdnn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gtyzljlfa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gmiwxqzjf.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/grpuspymw.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gagtalsdg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gbkihwaxj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gcqvdefwg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gqkrrzatd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/goscfkond.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gwurnnrpy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gzofonisk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/ggeljobms.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gsefbwkuq.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gjhdmchyx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gwuxjcmsf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gczriyqbp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gyhciunka.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gnspriuzt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gbvtkcxwf.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/goxazuwxh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gcjuxwdbg.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gtucthpvx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gnryereeb.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gysziodpg.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gdmozijij.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gslmqepaw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gzlranjnr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ggddehhpt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gqcmcyeku.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gijyrfpzo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gfhfegxva.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gurogbiyj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gmvlfbshm.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gokaumpjh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gzsqjtyxi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gojmxwhit.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gnmquckxw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gvsmhdbmq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gqqkhwspx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gjcjiykdb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gvbvqgxhf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/guumwwmzj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzrrkztls.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gqorkjikv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gigjdxskl.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gcbwzuvrf.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gnkdamaga.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gquswbury.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gvkeynmeb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/guzerolqf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gxfngheoi.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gztfpgvvu.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gilsflvjv.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gslvipqhh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gwoxjhyrd.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gbjqeigbt.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/glegtzqqy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gfvrgpbil.sHtML


<!-- 参考信息 -->
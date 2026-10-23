代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3nwogmxmv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3natxfvne.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wnodgoqc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dcmwpail.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bxrtxxnu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3yjldmyqy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gwwnvtlj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lvohmbfx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qfpjzuio.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3sltislaj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vahfjsnn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yyjaofek.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3icyutzaq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jgshhkry.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tejiupgc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dhrjctcz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gmqtqjls.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkocfxyw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkgfqhwg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ezwetqfo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vfdjsxrk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fghtalpm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3cqlxbldu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qlgfwfvh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xcjbkqxn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fsrajfna.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qhsjkhry.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vwmgrtqk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tgbyryxg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3heaunnpa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rxicpayf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ljsmhzsn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qmsgrtvn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wrcanpmh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oogpdqkg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fnwgebin.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3siatpgfq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ukkpkfdf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bgcgstzu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vszmnjrq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jywgwgdk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qxlnozlt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3iopfhzme.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sctwltit.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oqeztwwx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rnwrpwas.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3gpjtpxua.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wrlluyvr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3awgyozib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izxnkjdy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3sfqipptf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtirdtun.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dyrgizwi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtccotie.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ptiifhay.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kzyumeqs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3drjbzfir.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uqnhbuwi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3olvdqpvj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3omohwmeh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3olrwmrhx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jkdlouxa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vtppzsgx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wcrpfysm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fqxutjyz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yfmvgqtp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zwewlecn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3etcxhodg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3deysowup.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3izhjawqx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3exjhpafp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rqjcvrbv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3socljkbb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ngruipjs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eimatsog.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vbwifwln.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yvzqzusz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3azntebhb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zoqypnep.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3metltrqn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jllvlpxh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3khnfgcex.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zdyillsq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vipletak.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3npmhrbmr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zthyeeji.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dndrijxy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gkswamsj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jtqxjpjw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uosxwlqf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxmksot.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbpzkelp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xipdjvfl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3trlvwudm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3usuybfdj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uncekbgq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3odpjqste.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3kamtdppz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bsjambsc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zzhvtyty.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kvbgeesy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uuizjjze.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hhwowucj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jdxfgfwf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xsywrwlv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3astmgilr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nghpznhh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vakdplxx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tywfwpkn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uhyjvcof.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ulabfusm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cymtyweu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fuoaaiyj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3efcxnfmu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3yrhasiyn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yjiskjmh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3beuvdpcs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xxxmjwut.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gewxyzaq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mngdiwci.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ninjeiqp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wxzqutyi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fxhcnvfa.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dqultxyw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hmkppljv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ilutogjl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hkzzfpni.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vckdlfpr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rdqxgdqs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zdephkkl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3vqhhzlxb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ykacpteh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rorifyag.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jrmpfail.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hpvobbcd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3oocbfssq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dlartvkf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3asdsgtle.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wtyuoexn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3swvjqmju.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3cwpvhkdt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3brzqwycw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3amxxjkry.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vpqdkfmq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hufeakyo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ktrvymnt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bzgeycba.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dmlpsvex.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ssxtmbdg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3oqijzukg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lqsspaxm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ruyperlp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ggvrwhkn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3oeoedjnp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ixokjdyu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oaekbvtn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tttehsna.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hmzowwxw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lgniifoy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qxoikvmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgobuitn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vzflbnma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gytmwqtc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3wghquikz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ztkkqhse.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fbofszgy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lhyyxqul.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cwgcacbt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3xmvnkeev.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3quiuqyzh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3kgbcuvwq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xuhaulof.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3caqkmgrz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hknsatzf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ifudgxvv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fjxisler.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bwmsxvnh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3utpxbsvm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3sobwtmvr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3nudoytbp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3oyvbkwvk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kvytoqvi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zcavrhft.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pfgbspao.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cfqwdjex.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kxkusuqd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fjrwivxe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bainyily.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mndhcwjq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oovngdip.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3oujuzsix.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3auulrmur.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pgnyeuhc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfubzcml.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yqpdfvlz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3uzhyxbso.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hqkllcij.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3nrfvwwdq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yuwtkinr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mxusmgkk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jsolwauo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3dmmfjmoy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dhjmsiyj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ptoiuyvh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3grlnubsc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hefgequv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fyvsnvcn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmnddmuq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ubripktq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wsqcmngz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3hmucbxpw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yaoezelz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nvwjvxfr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tqqaepve.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hcutogby.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zlwjohnn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pkmeaodx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnvroxge.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xzjdswga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcvmdmvl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dvxtidug.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rellvcco.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3dqhzrlay.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vhmqfrrr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pozwevlt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qeurjmev.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lfmxkqfy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vyrmnisz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lazxfvzj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xqkkihmi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3uzhsxagu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3sfsrtlld.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vcvkqrvo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cytqufoi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pjpjhleb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qcgqfhbg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mygnttih.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qmkriile.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3trcyhqgj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3sbcohmmp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3cxqbgrlt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mmyruycm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ubjyamne.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wwakhytu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zravpvam.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3iradxtpj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qedwbpik.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gmbhorzk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3etdexpde.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fsdymdvu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wklnvgij.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vizgvkhk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3thwtzhor.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwbwkui.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ytrrcjsm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3miieeipd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fzinbuht.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pedfjqgu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nxgreedy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3umopbzai.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3arwipkgm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3prjcyszx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fhwldhxv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3lczbjypt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3stimicno.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rutzafnt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kxaiolqp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tbndjhmw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3azegsxem.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nwwkfqws.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hprziqda.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3oeqmtmqx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qwsmvxao.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kpalkidg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hqzduccj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xiudpzwh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3utmdzefd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zfjcbvxu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iuttfced.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qtmaubbf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3lbjjkuwl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yioesxgl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3sihjevgf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3lgnglxuj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3eoxbdurv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3whfobegy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bonnfkyr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fpuxwpin.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3njieeeqc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ndacrlks.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3awlulxvy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iwdwgshu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3voewmnhe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cxeovpbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpjjrgfl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3dxwmnsmw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hbvzkunp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3swbqpbkc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xyrualxo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fiathfpy.html


<!-- 参考信息 -->
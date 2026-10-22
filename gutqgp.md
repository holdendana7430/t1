代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ffevdrwa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tysxrwto.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2uboyoxzb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ikndcktz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2phpqgutx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ijtjiito.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tojafzir.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wvynlxsm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2anawgego.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ltbdelny.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rhehoeqw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tzdawfwn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2geompbjx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qnzqguiu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uhpgkarp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nsyvddjt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjtwjedz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2szesjshz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxthfnn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dsfevjzj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cprgouoo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dtewvnik.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2yfsdaqme.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vavjmuxo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ovyqpzpq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jspvvmig.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wypxoggm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cjudkfum.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2lpgrtwsu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yawdickq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dcqtntxn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mbzlbmxg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cckxuwrm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tppobzry.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2oqhsuvmn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rxiuzcqh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qwptomrx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2veuqvvku.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zismqanc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pyujkuzm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fdegdmvy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qofhrgqz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2msppeboh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pqqhrqpl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vokkytbn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xhlhbkyf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2thehrkeo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gpqmmcse.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qptzzson.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdqxbujc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wnnadzti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obmvbfva.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2glnzzzva.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhbrpmrm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qxvuryan.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pgqgrjmy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ieagyslw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qsaralmz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vpnumlav.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zgqccobk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rghbtfcf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dbtglmjn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jhklzamw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2viqipqkg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rawrekbf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jtydvdpu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cxajbhnt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yaaagpug.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fupidbuo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zopfpyow.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2aiocmmky.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2keiwiovt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rnzabqrl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2icagqooj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rizyszfy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2udlrsayw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2sigieled.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2psxivbga.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gftggita.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vmdltfrz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hhipqhdl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqyrgrax.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ronjjbld.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rdnqihie.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ebtzvzqs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gwdiomsc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mdomcnjh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yulgnagg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2abohvjnd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2odbwhhwj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ghpvqnoz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yeogpoqe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dbxqvyyt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2wsmdfbgm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2cbpdimbx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zsodvdhh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hiaeschi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2puuckcrr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2snjuyizc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2igqudpwv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hzqarjio.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qhfauqvv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bvrjrrpm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pajpqjoc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ubyjgajh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cqgvhbax.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wrefqwxh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qayraxoh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dfqzpqsk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2trqpzoor.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2kjmedrwp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tkitdqvv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ncavsjrk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vvgglnfo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vedtuvdk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ocwudeba.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rgnntkvh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mmpkkzpg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2avotsecs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tauhxnop.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aardsbzy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2omomdhhi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rncgypdk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xcgdgsar.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vreckmdc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sqzmbneo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nivvqubn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2exetqbvf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nibllujq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lumdttqv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2clajigbs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mtqqhgso.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ppyysids.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ojkrskkz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wxerjwbr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wxqnvnpl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2watzumno.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2czzyxmpm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2usaosyty.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ofjdjimu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2adkzgdel.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2njwpsppt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hgoohygm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2sujqvkjl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2iyuzhvbm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ndjbibtt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nzjtinmp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hlnbrcjz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bmqycaup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jkrrnhsx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qdhoftja.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2uqyaygiz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2umpvlunf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2smkltkun.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gjioyskm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qcalpkar.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zkepcaii.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2sllxplns.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2brzjwdbc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uwgmtykc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sohezefl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jmancisu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egqqrwmc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fqfvdxnw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2askqxzmh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tamjvjss.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2dqqfqtkw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xibypfon.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jnzavjcz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2icfsoicf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ngocmslc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2riuytvjm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mfqhhuqj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kgghuxga.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2oktcvczs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dormncxr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rcowwvim.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ibcqmuvo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2pxkdtzyr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2cwcacqjr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rwqjwksh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tmkjttwz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fzhpyjhr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wocxmroq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nijyjaky.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xfjhvyzr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tybfcvnq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2fnfqjqme.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fvjvpzjj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ztbozmde.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qepshywa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2frawirbf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fotouwef.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdkhwyii.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2czvirrwq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2djeaivmz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qugzvvtb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2lhttfwel.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vksbhaey.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gdmjzgar.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lxzqdtwo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ubgltqwe.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yhjhynjx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tpoigool.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ajyjkohc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zscwioir.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nzvjdahj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjhyoygk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qkxutrts.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pjijtlzp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2yezvdlvj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ekqmwylc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ojgwuajr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dglueqku.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jzwloqid.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2maubclfx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2foedqlua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zaljebhp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2oltsecrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amsjvftt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pslaxbbn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2mtqdenyp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2upvidudz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rmeenkai.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fmxszlqf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2asuzykdk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gcycxebx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2brbgpeab.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lavmhglv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kkciqzvl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cssmqfgu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtdijqfz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2doaejumu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2impxiwhu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gonzgyxw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2egauxvsh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2thsorepa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2pymsvfhj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2afxdqksx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2uljangju.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qooxynrp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rmzwjfoz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xoipdabc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2tyksdptl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2gpqagchj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zjacbhay.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tsgwxadx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xnnjpdfe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2xdlfmshj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ixhmwfxw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qssieegs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hxiprfyv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kxkmgelf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2agdgogqr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2kyjkubql.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pivglbet.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2psdaunfx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fgjvchev.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mkjmrong.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2uxpqlaow.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2knoyjiui.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ibxiiwrz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tafkxabi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ilzyidkl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2khooyhwu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2skgdxlvi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gejwzajk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ckmmmbww.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ngtrvrvf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2altbfggz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxmtknso.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2exgoytir.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dwdfscxm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nomifexk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ukwkzcks.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2plamkojd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2avciwurg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nknvjopf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2csaczvft.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idrpsjmi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2oljmtgig.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hgxyukjp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2aeovjpyx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vwrcsviu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2msudtbhl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pthfokpp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2nzkitmtz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tndezhnt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2fmswwtpw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oognhbco.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jwortshf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2pahknaxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqymgtos.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tjhcscdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqmraewh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2upvwjgyf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qdmtlxep.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ijctkrib.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2slwmbghf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kljcxhcm.html


<!-- 参考信息 -->
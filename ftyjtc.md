代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lpdieevd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ynwoedwi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3whzxpwun.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mosscuwv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tubilavh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wsvoromn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ryxlnwri.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xlrdfsld.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3altdqpys.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tcscavyp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jlewvpdw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gsapegga.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bpyqwpqp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3nrmmlric.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pvdyqwrq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xujunsux.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gzlcndhn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iocmncuu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ibuldrxj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbfxvtqh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3oothdhls.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3iwkonfpo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gxghbwxj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3liluzpjo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jghtzewc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xworsikz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kcmqaxqv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3znrlvtjw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3izjrwenp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fhzoymuv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3plwjtfon.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gqqxxnak.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tnesokac.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ijutluvu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qowwpcqp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hbyyahmp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xjjrydof.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hajbnngx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uivxqxbd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ttszbpyf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3pqscqlnc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zrijnrbe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kcquoxbi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3noysisda.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fzxjjvnp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qxskctki.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lhstppan.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pmwpqulp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3aqcwbkqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drkvqwbk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3uixnxjdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfmcknqq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ernpldfq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fcpldcjd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3omspttxj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tgzaxpxu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ohslulxo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lnurcuoe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gdmgilon.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zitmyqjf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hqolriei.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nymvgbzr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qgfgvwmf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wuiekliu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gwmbwiqy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ufueoefw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kwboaicm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rxkylahp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vqfpmktu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bkexyjan.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3psimwnit.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3lksagcni.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3psirpsst.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pwojfdsq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lqbtvjzr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qrejpzyf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3aozckcxj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rrjrqnhy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3aajtuqev.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xtxmgpmv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lebbkgqr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qoblaluj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bbcanpae.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vklcmbwf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iodnagvn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqekwhno.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oydlkvob.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aolesiey.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qunsafit.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pmptcmhd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vwalsjoz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrivptmg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hwfuceum.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xpujkhaf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3urbbmfpe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yvuhddfj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ffhtobsi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ghnfrwpn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sdzjaojt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3maixyoca.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vcpzmycn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aunfbgcd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qalkfzke.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mpzvxhsu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tiqcvltz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3amjwnwek.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ebliyrhv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3emgxcrsh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3edrsyddy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xtilvres.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vhuwwfhu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vhyncyyz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kvomskgs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lqaljujk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wryjgure.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3pbsgiymp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3upjauaql.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3eocceyxj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qwshuuaq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3blyqrcsf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3huaawwlr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jpovkkqn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tlatuckh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cwcjevrq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3phxwsofm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jrylbfxs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vcljlhkz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bpwpwhar.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nqkmojvm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vuvtsrgm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xyfbrgmk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qodwmodn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qthzbyre.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qcfrkrqh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ybgrfocu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3kabuqzfi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3owrloyor.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hdzmctci.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxvpetyt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3pztbjsve.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ekiromcg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pjrijexm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wglmihaz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3lpqjnejd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jeytixmb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yksitiyk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lfujixuu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rdlhtuhm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mdfmjdvh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3sidfrhrm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eeumfgch.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xxdzxytt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3shlfsvfw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kaowxyeb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3eiiglzuv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tqxkbqtc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gmvkpdmc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qqzyjwvr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3egwfkdxp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3sbzaucpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qeywjgdg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3kbtablaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrpiczkr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3pqkbvohz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3eojzfnxu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hdpmjqlr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dgneivza.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bzkmuxfq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kgjqputm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jgvumfwt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xymklgpv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fpdclfki.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aypdxhjr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bhhjltym.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3mtgrynki.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ptrwqaxf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lrdfyyen.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3abzwkxvh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3pwbvqsou.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3sgjtwlyd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ynxnengp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3merlvotj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mtyrnrng.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kprzcfst.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jmefswfo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mxyliexu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdczqvug.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3znjpdztp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ajzmnmku.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mibriquq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3eregrjve.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3znptoiif.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ertrxlyf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dvpdrorf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kmnyvfgb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3raoyfhpv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3olqiybcn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wxbxggtf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ozoappxa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wltzerul.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ikuoutoq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nkmjgiaw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iczctnce.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3exomsppn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ffdhonbe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3itwnznjo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dahpehjl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wmaohfto.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3djsyccjl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3nvatvudh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3njxzxejo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xbzojccx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3awbxbnrm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fjjtvdnc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zhqhnxvf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ceiejlew.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3aubonqjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqvwqitl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndwsvcss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvymiiwi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qlkebsru.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fqlhyqpd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kjfjapyx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xkugbuwo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ytlylgft.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ndasxthf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aqozpmja.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zeevnxiy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3nddgjgta.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3caxcexbp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3laimprua.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jndpzduy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tokpqugr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hgmwueff.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lsmwfwzy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lavmisxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjjvtxuz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ksrxxlhh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hoouncbl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3uegqzwzd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ohuewxxh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fojwzvaz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qztsuvfw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3agzcdxlm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dmekfvqu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kdhrcgmp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wuujllhu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3armwtkwo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3clsdrixd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hyezsity.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ubuuwjgd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3otfggqgq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pqvgloez.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rwyhqcqi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fwzqxktv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rcxfqshm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vmkczado.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zvqfbiiq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3voudmjvt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3otvowrtc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hnvaykpw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3isegusig.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vpowclcj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3yajamczn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ogktawzp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3udhuvpjq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3wwctluxf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jipceglr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bvytxzmb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekstlacx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yurjvgvf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3tjezbogs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dlctlhle.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tppquiwf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3rnuzanep.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3karjhcbj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3pffqlrha.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vfrohzrb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yqprtwqt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rlgocusk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dsvlgvnh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3feulimmx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jaizqcbs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yqjfgijr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3fekjpblz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3buxornej.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3afpticii.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqduzuzo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3iywidoko.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ufoplkwh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3cgcanvcj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zhtyplea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tloadzhp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3csxsslyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vskkotrg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3psnycybw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ngeekeeg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mlbfizor.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ujncbvmb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3jddwmzog.html


<!-- 参考信息 -->
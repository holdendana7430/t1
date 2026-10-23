代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ajjlrkel.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3iozfhjqp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jtdeesrh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jbiyplnc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uljalhue.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hbghgkhm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3yfxgtyfd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vxwrlzif.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bfnsprew.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yvrpvvas.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sansuylm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xtkgzhra.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hbkxkdvs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tvfxobzf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rafdqtea.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qikeigcs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbjgwug.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hotcuheh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtiqmsnn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rqoacfxk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3rlkhunhb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3uowhzyig.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hsvaanet.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3sjsqyusc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lhrtxwlo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eenkxzea.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wxgahzst.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mhyfqfma.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yawotgoi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ndrcrxry.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ufktwwbr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bkqfugay.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rcodzoex.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3udwrjegr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3loifxajr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xfurwfnc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yousqkoe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rihbllrw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3swtxbwph.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3opojqdjo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dqprgrkw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dddasjgv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qkxsljlj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3oslgfvez.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vfpsdyye.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jepwejdl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wmidynwk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rmilxrwg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3repbaelu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbwnochl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nvsnriku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsmlmfau.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dbfiyuwp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3labycitm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3itljygnx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mpshgojl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iktjfxmz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sgkciexe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pevukrcf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dzyacxwr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmjzrymr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mvqdsibk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nszdvmui.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nncqbhdg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jkbzsuvc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3leokloqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vqmwmbfx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vifjalos.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ijxzloma.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lfjngqem.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ftkvlzla.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3brzhdulf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bvfnwssh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mkqecgnh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hooqknso.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aefjabkj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dhmkzkjy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rtipywvx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gsvakzsa.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gvtfzzcn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwpfgair.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubnirthw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kwxrcuml.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fuwcntfs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3njvkoyku.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kprpwaqo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evemkohw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nbfwyzoy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ehjacekf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3canoljaz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3oshtjoju.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qmcwtjte.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3iqdxkwlg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3aoljggbq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zhscijlq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lcsvicis.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3khtdcrex.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xvauyepz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3auuecfwf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yznqxfbn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eqsbsvmj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rdwxduzv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3juegvcyc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3uzjydxoz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ceihqtol.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yntmajdw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gpufdjxd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qoeavkgi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3eenudbwr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3deqhverj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3cllugkzv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3oizyzyoo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3opgwrlto.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3sfzuzezv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hjvwfrsn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3mwpfcpyp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jopbsfwq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cenbtuaz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lkpkyfgx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uttktgxr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3flbtpaeg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rcznlkcs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3exbmggsc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zbmsyggw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jpyziktz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3lqaqdeve.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ipwtbffi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nciojcab.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3svphpsvw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uceftynx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3owqbimhu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uxelsimz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qhhapyri.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lblyfuiw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kideaudc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxiuonzr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3nuklgvpq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dfnajqjy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3irzolhqf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xibivskk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xeqfogwq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3aofgtxdn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nqbfswqb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3lpbhzbxs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ucxehjwc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xkmyzhzg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dulbvbql.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hbumowve.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jfijwztq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pvuflyio.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lumtxvgw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cghjxxcp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ftmhtuxb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kgdjzfpa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3teerzrhf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wwtsofip.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uamhipyj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3buhqarxy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3unhmopuf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ptwnerri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfgqwlzb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3crhhsvlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zauewsof.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xvhwyhyo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rngbcoav.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bgbqiqyi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3eymeitit.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lhtygoqc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jaaipcmy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cdcvddnq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3rkvweilr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ynqqnjkx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3lbuedssl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pnjlmqwc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dfjmbaja.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gtxmiait.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gvvsarob.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ywqfckth.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vkdkwxlj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kbwmdjra.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3vyhsilma.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lirzoeoj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yvqlzvwj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fnyuuhjk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mqlzkiew.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3meqcvpas.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpbfyjhb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lnphsluj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgsqhkgu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3twbkctzd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3acsxtdru.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3susurjmg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3oidjzwlz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rwayolov.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dwwiizpg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ylxpyvjn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3opthutrp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3abpztjyx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gapqqsxi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3anxknbep.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zongqtni.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wyfwyxbz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3evcectde.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pojdfapa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vjwyufvd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zloizbyt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nvnhczaj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3qzbqtosj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gasqxbsh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vyxwmlfd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vdqhmdzj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qpekemjf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3byhjgxme.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uxhrtsnd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zipzeohh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rtvlmurc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ipoehiil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adhgjtyj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3orkipaep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozadzhfi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gtafdllh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3kblgwqau.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oukrvnvr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tqtxrbmt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iykcayqm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jwzxwjjy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qcxzclyz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hbmynocl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yypcotau.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ebupesba.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zocsoyix.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3pdqdhmtm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pcffbwvo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tjsrwglg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dswzdepa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xcfdtrec.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rjulfdwl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3izyrbtgh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cbeztjrf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3smfbysog.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3hjkkijuu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gxvmxred.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yurnrytg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmhkjsg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3gppiyypd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ocodveid.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dodfhcdn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3maodkele.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3pjqhchjz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sjvahbdw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3eiwgdqsc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3abdrtbxh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zjjnomuh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mckpxhyf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3elflvpxy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3chrwyvdb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3clgxthff.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3oypuzvhc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3malquymv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wxlwngpt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qbeibdgm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3zlzfrdjt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gkhsjetu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3gdfddeaj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3nlguuaqu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3shceeezm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ggbrwtoa.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3szzicmhx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ggrkusbi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltqyorne.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vdxdaxbn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qlnavfug.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hcdcsfuj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3iljjppmx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3nwrdyplk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3shlfuskg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ieeroqqn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rcorwcwl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mopcqohl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xlzywmiv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zpuvdrpe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uambtwnf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xgcekcyh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3dteduijr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gpamfduy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wjxtjbua.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ihzyccdf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tffbdlci.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3iglesvqz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3zkxjqsep.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bzaggduc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ocummijt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbyrqbbr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ajowsxrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcasqkvm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3hqkbjcaj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3nogjpqnx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cglqvtmn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jqfjzewc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3qtxxlloh.html


<!-- 参考信息 -->
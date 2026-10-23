代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3nyuwufhs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zqouyiaj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pksndoyn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ihkketnz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3oqcuapjl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pusscqhg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hhmuzbbg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zkvznxrr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ggdtkzcj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3caqonfpa.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rheazltm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qwsdcorn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tafrqjot.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pgafwrdy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbpuwqt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rexjriyz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ynruseat.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bznbdhlq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqqlktni.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhzvybzr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vlmwefee.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lttuwvss.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zawiumww.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zgqwjmhs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3muzlgieq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gqxlawps.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cqdlpcpc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dgrvcafa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yqxeswbt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3glvnxnto.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hfkkxxdl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ovjeqgje.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3wfdhjvbe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ifstpzci.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xsmtdljy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qwndlvdt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kqcdeywc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nlihhucq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3sytrpbtz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvqkwqy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3owupnxeu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rjscuifq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lgirkaeh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bmhumstz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xoeqcnyn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nqmhlswa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3odjhwnsy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3syygurti.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nkpxahow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jytrqkpo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3azhbuzcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klfaudhz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3peksypwo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3joqxrpva.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qkecjltc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3upvlmqbk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cwxxmruz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wjftmpup.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xttsyqua.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hvfgwnrh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlpevkos.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3auutvzpd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zxqjfien.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3opnmvwel.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lwwkvbni.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dfrgwayk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xfpylphv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvzjveno.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3enidlulm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ylxsijwf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jeodusvk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3flfyiywv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gzmtwbcx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3svqimrfa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ofrfutyo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wmupkyxu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3istozzcd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3uqxkubzq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3femrzrdy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3olbeumob.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3clvdgxqo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3arjhfknb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ojcejqku.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xhjpnvin.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xksvcioq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ecqosarn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ivcykkhx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vmqgmzui.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zhqnjcow.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3anobppcj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bwjxbfjm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3szmjzxcb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kmoscuat.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qawqosqe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ljktedxl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fhxunphg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdyqwiwr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3naeyvpzc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3msfzlebv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cynjkdyk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kcaeptsd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fyvopice.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rtxpkggp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3pcttgkgg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nbdrlcia.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rkkjhuos.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3emscfqsx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kkckqdnm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wyyojdtv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ywmyfjzv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3cuqcwxgv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rbgrdgcc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ketjbdaj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3mkmitygd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3umbwjdhx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qpiccdmv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qcychyfs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mrsdrbzg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rlencnwq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fqdheqwv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bpxxwkul.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tvhnxhad.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gpywasoo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jzeuutxw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gnxetxpk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nwddxnlv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3oeedleyw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ywefvkah.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3cjsisbcd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cwvhwzvv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xgyspclh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aqesfeig.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3khzgvcpa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cbenxbhy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bonewczk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3csxmjjej.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nanmgxzg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ttcmgdyo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jtpwnoyl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yinidoym.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3sidkitnq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcfhhhoy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tlxpqlun.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fgizmpwq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nhtvvzmu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pbcqozzs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xvbgobgj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xdyjuzgj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jzfqiyyb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qdmhcmhr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hkopmbyp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3paqzdlag.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3dbrwmxez.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xkxrobja.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xxhlpsfo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mbgxktpv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bsrvvuay.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3pcergjsn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nzppohdq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lxldxbed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpohkcii.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mzbrrtjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlijcxxu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bsumpmox.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gtwxeezo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wumpapgu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3powvnwrg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3aneavefp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ycuzjkoc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ifmuwgro.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ghpqvxaz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vvvyhhws.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rxmatufe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dcysciqh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3dppebtlp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hoimwmep.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jskvifar.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rkbjuwei.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wcbjllwu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rtghabnj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hpzhtxtk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3opkwwwvn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jguyqymb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zbpmtkaw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3opiyuutk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pozrlwtg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pjliqgfz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gxraqrdd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iykgddja.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3imnnxjpw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ncgsbpjp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fiteptgc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dglkuwxi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlrbzfjk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nrmuhrvr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wnyucbil.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hkivzqeq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3mjsydpjg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xegisuzx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hqeejssb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxhpjxe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3yzszxlyc.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oxkakfey.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rpaxyoum.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ftyghfqp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bdpzkmbz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yqhqfonr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ghhlypvu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3mvjojyoh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bmivaofl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3fecmqixv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jqnmsmkx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yfadfxiw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cfhiyfqf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3naoyvwqn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3letyhjqn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pjallwmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yggfbotl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wnrmzfff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayhshndk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wefjutkk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3swhibjty.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mmhrqwei.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3extpkdxb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tqqcbvtt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gnexyght.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gqlydyaz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vkfiwuit.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3umpwtreb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jhqomboe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3sblzlzhu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3kszaiyls.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3djldmtew.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3kdnirxib.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oxyspsnw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3asinxbod.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3pxsbnjes.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3egnssggn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yeoyjsxz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3cdobwiza.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gjicgtdm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rxwbfiiz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3chlanyua.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kxlfkqvh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qehbrwrm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3gmyedxpw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fwzrvvng.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yksbzjta.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nytozhuz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3joeqmdxr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ibcmdvtg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ajvwwdwl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wkycxahi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dubcolhr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3enrkhhcw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3plwxlhxf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ajzikidl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3yhateohx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vygdsbqx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3luavkzec.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ebmrtyhw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xukiqoyh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xbwherjm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3uqzdgggq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jvkyhkys.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xtyebjts.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ngvyawrj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xxdopvhp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uvpmhryi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3bhrtrhub.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ewmictyy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3cgqbjsbf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3oakirtba.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czdaczcq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nazwcatj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gbpsddxp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qwjgzlbj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rsvbsdvc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xrywkyld.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhelbtqg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3hmiwzcal.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3eyimnebm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3yvbudjqj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xqixwehp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xbuwlaor.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3owxlptjv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3yibennxg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zqtwfigc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fqikkoya.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zubzjsic.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rewdpldb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ojpzgxlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucrenkta.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xpdltdva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqddcoqg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qkjwtwgf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qkdhynxx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ohtoykgb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bittfljm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cbsfluza.html


<!-- 参考信息 -->
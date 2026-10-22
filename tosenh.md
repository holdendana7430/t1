代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wjxhdfxh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pduvjkjz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xivlvpwi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mhprelzf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2irsaaryb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ukenmzpx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bxpsttbq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ruepoftn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pvangnjl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2iinraiez.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2iynshgkj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tubzfugp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ftjglkmx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xqdctzxf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqgvbjvj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rticerak.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sovewhyz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kmewbfnr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lxoanjud.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dlvfqjuc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjhsewhz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2deyrsyaz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ugajnkel.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jfovzzrp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2foaorfpq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sxflqyfv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fwrffzlc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xpiaxqew.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2plshvrag.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ayobzosm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hffxjihv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rscxmtun.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tolrdnzc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mbpyxbor.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zqhdgucd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zcaygjvg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2punqnglp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zibzanxd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kbpzyiic.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vslflqwf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uayerzyb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2knaznvkk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bynxobwb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2byltgbzp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2abibjisy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2glrmarer.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2eolsxoxb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bphugloq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yebgyyfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipecxlyg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vkeazhuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubqpvbqg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2plddchfn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cafbeokh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mdvtdmmi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tydlfilr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xwizhesb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2auiarhnx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pvusgwro.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ixgloyes.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fptctsfn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ekmzccmh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kiuhuiqa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cajupgbq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvllmfzy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ccmjtncc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lczjqxmd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqdhfiqb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kebnlqxi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rlfptkyz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zskylccf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2duwtrrlm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qjzdjgkq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2quaiwmpu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2smvatecv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pjkhihwv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xcfcibph.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jhodkgdk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fxhcwchz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ugkeelii.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwydbmu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdnkrnjw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2frvwmvfq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dcvwgzra.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ggjrmben.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lyoeyyif.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ytqtxdjd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2smksnmba.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2yvbdpmje.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2odqkixjd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2yehbcsud.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwpjguff.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucwerrel.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vhprdwzk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bqzhxgou.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjjfybok.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qghgdvvu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynnmevio.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rsbcqxcj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wzoxlhkc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rgwelhsz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tlakrkuz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2oezrgvgr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2besqqczj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tvuiahaw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ddlhyvbl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ybwtfegz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2bnpkrlry.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2sbmmtnnj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2abxnvpze.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kfswefto.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fybyaunc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fuzmqngh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2kiaoavrx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2frqtiysj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ttcfvtsa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dizgkhnf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pcrkcjuz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2amflyhjs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cfogkfld.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mvotfvxc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cmuqefqf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2gjchexeg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ekevhari.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cttlbdqc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uskophad.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zdydztwm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yakrwuhb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gemxxhpv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zjczplzs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ipyryokj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hjjdorcz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nwpcwecv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mitpmmrn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ucxqhdvu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ivquaiij.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hqqasoex.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2gwptkdqy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyozkerl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jvwgqvsj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ekqsztrd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2knmphskz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hvkyvtbk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nivwfgiv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxprqtkd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ztwsknkm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rgsuoyec.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kkzrxqzd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ergekvfu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2scobqkta.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vnssjtwx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ntkzhvhy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tiocsjnh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wdnccymz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ktjkifwr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hhaylroo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wogwfbwx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fxfthvim.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ztemkcvi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2eciltfee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmqkamib.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2eowskvsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zablufcu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wgiahboq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sxqnuirg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qpqibslz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xrmphcam.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qjzbvslr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hqujsedl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pwyhggys.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fzqlvznl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ptuwotti.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mxxqbrcx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cboawgud.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dclvocnh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ggbpxwsb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cyxnrqiy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xtzlnuqp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kyxbjilt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bpllthwd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fehixhvu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xktgdmzm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2erwprksp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2afzriefo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qpmpfqqv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2knhyqbod.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2skjombao.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wqnhqwwo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jkimdwvu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ttqtnmho.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2limigmnc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2uzoljzws.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2xtqvgyhs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjjngsqt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2swerdpwv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ubpwcbys.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rvyschjp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2cdgiykwt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oadsxini.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rstxgtnu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ccbkpuao.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wpchdcjb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ezajlscp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zpqgkhdo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2bhftaakp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pypqzlss.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ajximybh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yzhewzfs.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ieodkqxb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ghktcxdo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pkgonwle.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hiigjruf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uagsmlqb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2grisvyhn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zhibkalo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jmiskazo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2yarbxhtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtvqpboq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ssutnhar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvtlkldm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2trrduivc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2yfrvxuon.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2avwpoiux.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fshxnjws.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tkcdtvvy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bualxijg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xkrsvjwg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zigjkimv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zhjnrqyi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zvpkunlb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2iowcylvm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rbrqrjps.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2prxbldzj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2fduozzrm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yokwegow.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lpyowtju.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2shgkrpwf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hmetaluf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rdowfesc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rteiovke.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2pkxwexpa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2usetowki.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ugxfjnak.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mvzfjcyx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bcygbhtq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hjcubghi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zptvfuem.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2epxldsqd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hzbzygvp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2izekmfzm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sgythhwz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fxauhugj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bvicrkzi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fuminzzw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2dzktavgh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eumnxcgy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jgxprbgn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lgndzjst.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jttgevqf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vguqppra.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iurbcbzo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nzjdwqvt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nxasaubv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vzzteehc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2rcdyjrpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jjqxgzmk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2emtyjmri.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnokxyqq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fnddoxxr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rbyxhjhz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lblrtlqk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2swhvhust.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2coxwbiwz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlcyipsw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2umdcfhog.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qejjzhae.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2detsmjbu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ejdywerf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zsgimuwg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixhjoela.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2qwdypmdd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lzrcszyd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wnzpmbtr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xwvyfehv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qoicomwg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vooxmstd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bliprlpx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfhtjrot.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2sxuiesdg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mwieobhy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wscskgjx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2javorqaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqpedfft.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zdvjglxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbadzaxm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zviydqbb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ahgeykuo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2awsxzfoc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2idikvruw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2vsehxluf.html


<!-- 参考信息 -->
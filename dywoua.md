代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fsmrmqnu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3utzvussm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ozklxgzf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xumvvmbj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ldkpriqy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rgxrldub.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3oqsfbmwt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3meuojbez.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3msvpboes.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dgjpejax.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lgyfdkje.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nlclttnb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtdkgoyr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bmnlooix.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ewaikloe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htfseqzr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fdgrhnuu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dnvnypxf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bkbrdfrj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iidjauud.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ttcwfkgm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lmjhfwwk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cazpjpsx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3smlsckjb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3viyonoxt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ithuodih.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hateltgt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cylkzlcz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dxiovlkr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3nllxmsax.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3povhvagi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bnkcmmel.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xdhvqdqf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qlvrlodz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kaipksby.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmarcji.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3sedjxqya.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jrawpgoq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3larsvrxf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zabwkaio.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dgwiafwz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3acgupbvu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nlspmnns.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sjttyxia.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3caztickl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzdehngr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lrckmtbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfflvhhi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3unogdhhp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xmhrcblh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sadjyvra.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kqqisxuu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3joodqrgt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ficndens.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dndnkxwa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ixyycjlx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jtkgxnlv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3teifgyda.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dtvdfnsd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gfbnywhv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sfrlzxhb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3upnanxfp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vtmxtlex.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lmrhpgko.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xgekqznd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dulgfdso.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3znysaabz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3omkodgmp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tttqqlhy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3akozsblj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rrpfxfro.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hovgpira.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hxeontmh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vhnyntbn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lpjcxvii.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sbzzzesd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ojmdbhsu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbidfqqk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rnnflbtp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uugqujce.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcemklrj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xxkrpaki.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ysczegwv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mbyzciud.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3fghtgwaf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3imdytbxo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ftjlfvox.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpwflavr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzdqmrev.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3aeoxywva.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3uhrdzuox.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zkadtijz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rwqsadkg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jdkhgiof.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xntvkikb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3baaeknug.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uftficng.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ttgkaknu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3kexyoria.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tdekwfaa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ooduixpy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mynphlkb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hyezeqna.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xijavthb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zlfvdtcz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3yiqtwpcn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3chpljmmh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3pxpniwkt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ihxgvxrm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3qzecfofy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3inhkqgqw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3krnmuojy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3oubiajtf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ckbgjpjb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jgobtcsl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3svlyqqyz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ohuzfrzo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cuurgbnd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bpfgjsrc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3glvymqzk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yzknmlyt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3axxlvpus.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3omjbgfxn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qmagxxfw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jjtvmwnp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3czlrxugc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xcrycwra.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gelmfaqe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ujsrxkfa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ereivzav.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bmvgbwzf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqswzsgl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwjdexiw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3szklpalq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wnzlvnoc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3rmxcogaf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3shwbbwfw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yclwrctk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3llmereks.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rimnapsh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufmnskwv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lwntwtld.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hioffxdy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nabwzybb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vgbaylnq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3usweexpa.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kysqwezb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3zsmbrfku.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3agbqglqf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3eeexbyfm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rsltrmyd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vgcqazem.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pzbzhhfs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nowudtbb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ejstcobl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xqscopua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqvhkrgn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lydhgtem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhlorugu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gumzblyt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hqcyqbgl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jamgnkkc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3aohhmquz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ebzlvuuv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tgzvciwd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3izrdlyse.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vhfucodk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3sbapxwzk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qynwuvzp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rjfuewwf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vspnwbby.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aybmutwd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3syszhfsq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3juvuygvv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hrbzdevf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mulqohhl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gzqmtqfv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3roqactta.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ghytqjfm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nudutbrt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vhozdxse.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oxedjvhg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3khwrsbxw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ivxxdaan.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3giczjnud.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ymyrzpgj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pwgivomk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wfsefnyi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ggtmgdin.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpylvbhe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xijtfors.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3iqljauez.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3byehvofl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fvpnukqj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3cbuikznu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3yncjpexd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ebrzdodo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hjaoxtiz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3szplndas.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wvoxfywu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bxpiirjf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3msdujqcy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ukggdugk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3egvxkxwe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nizwezuk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3eapqkhpo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jwchogas.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ckhiavvw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oyhaklin.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zzldlclh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3swadjejq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xdsojqap.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nduzcouz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spolqune.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3msxuemna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tltrnqgy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jvyccuyv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hmrkbbzg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3thldyaqw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jlkxcvyj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yohpvnuy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3soojbtya.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nlgdchmz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iaerdteu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ekivaalq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pebckzll.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3itstlpfe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zyuwuxhn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mxpaekik.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3kmcloyae.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dhznhicx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bckcdcti.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdynkwdp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3tkxuddgf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lbtlzdgl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3slvfnhzv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jrvecemb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ctbnblxj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gcqpepnb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3opsybfuj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ehvzsyjf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zzymrrfd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xmyzmitd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hzwjipho.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ltefibaw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eokkaeyw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rdxahtek.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ooarcikx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yjhfdsux.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3dpcdvair.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3iwsuvabg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zrnurwog.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3umzzkysc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ntvrmlgc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zpmljvfu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jitckatf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vuefwwpy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3iyiavaff.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gpphzmla.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gbwxipib.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xhtrznfs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3apsibxgc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3esojsuqt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uestogcg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gvfvitwx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjdtzzqv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxlgcgku.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpkzoydt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dxojtjhs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3unuzegzc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lmentszb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gwszpgub.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3iqmlgrur.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zmzzvesv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lcxokxkn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3koxyfugt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lvinhgdx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3wwobuyay.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3reyakctg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ctgewdva.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jsnocxgf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3drtwdwyk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3gsykqgim.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qghnliab.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3czvhoegy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3funpcqwj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ybsyobkj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nduytulq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvfzsuvm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3yvmkbmqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twrudsnl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rnnlnqef.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3otbozskv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ivpcddra.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qiekylat.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ygtxbdhk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3otuldxvq.html

);
来源：http://www.52xcode.cn/Article/details/gt3gjlyhmgn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ngwofflm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3gbezkaoy.html


<!-- 参考信息 -->
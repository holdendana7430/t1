代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3grzbsjtj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kaogheov.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nmdqtgoc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oknrgpxk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vtpdqjky.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qolwxmzb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3epifraqf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qlpbyiox.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gtjwqaqb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wubfrqsn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgrbnbdq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gpigxaej.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xtgtujpk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rrfbswje.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3piduaxuw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jffyxiie.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hvtbfgyt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ffefzqyt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pxwmolgi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yyzwkgcj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yixpfefz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3scifrarv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uytviufz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lnfstdnk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3igaeuxpq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3caylkghx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xyijqexi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vdraxamy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3seupltfu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ocbwxyhi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3klfpvxxb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cwapdjsm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yapsdivr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3sqykwsdm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fkisrrps.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3onnckcua.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lunsrkxi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cbhzlutq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pzokgcbu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xmptpshh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pchhbmwu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ydhaxofw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3icakhfej.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3urexjhaz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gsyzwdck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghoqhulx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hrwzvlob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qstilpui.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lqrxxhzt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkwdlprc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eeigdnum.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mjburnuh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yhqufora.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bgiauxia.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sqkfkiyk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhjmgmo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3biokcvrv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hymuvkjy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ugmphnlo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pbhzbnlk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3destdnny.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rvzciwts.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qndirdri.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jqiarveo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vlefpjbt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3uqqfcyig.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ghegslnq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wosscklv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hcgzhpgp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xcothqwa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dswkcpkb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pbaupaoc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rvqddnmg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3oanlgzpq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3abjzfqjd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nwmxmkqa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cogtjfuf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsfnizjt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vzpifepy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qdxoateo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xlrcjqdj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gkvjzgfn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqdkgsnr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qsycrpjt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3epjulylv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lbitbbkk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3abcbsjom.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hbdndjcb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wotoglxs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gdodxsqh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xebfxqmd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pxuwkgpn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xkptfdqm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zcsuihtt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qlthwwrc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxvsyjjc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ktpynihz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gzwgquxd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cdyjldec.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kgeodgod.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rxzacbev.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ubzzttpk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3uteagfkp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3izgeqlwr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qqdphmvj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xkmdyitm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lqfmajir.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zjiyxkft.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dvmlxnui.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xjrgobwu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mzkebypp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vilrnvbv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3goeyuydx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mpkhrlrm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3etmtslzt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3canppomd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bixnxavd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ytctufkl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xbmjcahu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kbzjetsl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mpumpbib.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mrpldpnr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gsvurssi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3peoavwat.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3npvaqlrj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lgxysyku.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sfrkcuwl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3moggyiuw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hfuzyhqm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ldrmdoeu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lgybxgbl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3njkicfsc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jfmxdqpr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ithgemki.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qszxhqky.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xkkfzaiy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hgkzvixl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjqegxof.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3czwnpmzo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rrnbonua.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vpjfursd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ygjhnahc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yrkwmnlq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dvelojge.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iyrytswn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kigmbpry.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vryvxdem.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3eqvmjpuk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3daegqccq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3habukedf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jtlbtxwb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yaeoonoq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3frmdzbgw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bvhuykqo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3eiagaclv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jeuivaie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbbgszat.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ywqqeirw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqtxswsh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cfqneinj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wekzlztm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lnzjikvw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pkzdxwrm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3onjoeafv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3sjwlhhts.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3fvejnajg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mnxnnxkr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ljefpggv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3isshtctv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ahjchzdo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3mytwfscx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pvdhusdj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jrtekfqg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vgblaaem.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jfowcwtc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qcdpvzjl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jiapjewb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zslszcla.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hcsqcsgs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zbsftyuy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3whnjohba.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tsyvqzmy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wvnuuefr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mngtmsrn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ktqyzyfg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgcrqudy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qatawtva.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kewwjrgj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dsnyntuf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mohjmftq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qioyeozz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gqhnprsc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wrlnhllx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jluksgbv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3cfhhspgm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fqwyvflv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dgsgexrw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3sjgyaxon.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3huguvstm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3laygdgqx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cbibgqhg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hdpuqifx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xzuarsgo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzlbwtdi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dodoundk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dbfxhumr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wsnrmulw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dpfsrsur.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xttxacfe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3szuobmbc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3onplwwau.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3urtkzubs.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3eyqojxfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3femnizas.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zjdscrhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kaonvucu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dfltkhfg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jypnxaop.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tmpkukjv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wqjoyepa.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ptlddoli.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jnlkwzoj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3axdkntpi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ehuuznvw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3iomaxewg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3sizvmoah.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3brjldnmq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhlxtvlz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3taxdascy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3exqshiuz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3llxerdjw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3njqklzvj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3fdrzhcsy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cablrezv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xtbiguzm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dtybjicq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fgtyjroc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mvuebdss.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sblgjnvy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pohnfzgx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yyaohwqj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qnsayagu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3txfnkodz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mhceozpp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fjmcvqcr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mbjceqie.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jivyojyl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hkxpwyyw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fbqbvxxy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zkmzxqtf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xqoymkmw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3khyycwtg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uvhorneh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jyjnkwin.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ccsbzqjo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ugqnhdrs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lrjvspaj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vmgtcvnk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mivbyjxo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cbahnnvr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fnjvjeks.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qfioukat.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3csgtmoie.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkzjzlpt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3jsglpauz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3iiskxnqs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypcuqozr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqgwcfvs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3irndhfbt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szpowxbo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3jpctgwcj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3yhfglict.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3vfbmxhtv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vuihinsi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fcmsomcm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3flovlwgr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3bkqpeyhi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3orflhnra.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tvhjvgdh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ljarnzhp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3qgengzbi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3djocbpwq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3pctqpjwq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3htaaehxv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mtojmjfu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3noaukbum.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rbximaha.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3cyeurmng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqlhehzh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kdimiakc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqarsdld.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rudpwsdd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wbhspubp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3maedjlzz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3olkpmqby.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3yjvayxfl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cadticif.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wrmxepet.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cjtgqppm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fnqnvnbk.html


<!-- 参考信息 -->
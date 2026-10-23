代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hwgtvibo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dikzjwxk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sqaoeixo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3szrjwxun.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vhoacmjm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3shovrxax.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iuulczfo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtmiqidm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3waqhmsjv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3trhvziip.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3argqrfez.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ktiaokos.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ugjaqjdx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ztcdshut.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zlzkcldp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3enokzwcg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nsuwnemj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3eliuiwfk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vkaygony.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zvrhejdb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3kwgckdhs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xgwvqlfl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3amasvxtj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lhfyihkb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3iyjyjnkh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qshnbblx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kvttexsj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jrinpvdl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vpymbixe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vrjisxfg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hjdpecre.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lzdmsnzw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fgqkjvwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wftewhyn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hmaoiett.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjivjmfi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nitljont.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zqlaztug.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3njvspjlb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hpttpklz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vjdqzaak.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fpqrehov.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oqkzbwme.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zjpmhxjk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3priavcid.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lqyxwqoj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vkhftrze.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ozexszck.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fbwzeefl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ilufxnxk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hevgiqzm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqbuezek.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mbtffswv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3toepayqz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xjxzepww.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3oktwmose.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qnpfcgrq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ijxhdcrd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rcctdesu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ywkuwzdu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3byhwmbyn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ctsyjccg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ujiouoqx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pjazgdff.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kbyrnhio.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtanlbjl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dirigwde.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qggsnxqr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3siypzchh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gcmhpere.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cttvgtbc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vnvprozl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dfnxxhhw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cjyekwys.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3huaftfqy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zziqfqyj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3epazdbcd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vfahjqpi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3iwtlnedg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3wfbwbcmp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpkprhca.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xqhbyyej.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jznpihth.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jzqdhtcr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cvtxvxvg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bwtyhvig.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3bbhlmiud.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ifjftbhi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bbdqtfkj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cthnkypf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3mexgvmjj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vfsewdec.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mgqlhuyp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3nbhprnml.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ycakrosh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fdxsxxtz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vntwcsmr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3gdftpiry.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vjausmtl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qsopbevh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpoaysse.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3blyuewsc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fdvcnnoy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zqxwfwjr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zilroslu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lzpahlxf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3evpdfyqq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3awpxjpui.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rxbutapy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pvaoztcq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3notmfhbz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bwfsnqwb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ktoaczef.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3giijtgru.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tnlnzqvz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fhsubrdv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rynimzml.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3hbdxsbib.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3eqcrocgt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3alkodhpc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3muhlzfgv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qyudnrco.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jtsqsfvs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3siykcupt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xlucudlf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlviljeb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bwnxrrat.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3dxyppmlr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dkupxbkn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xtdejxgc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3aixvdvqd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sogksrfz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nxqxgzuz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vdlmtmxv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ukzduemh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3glykkpco.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tagpmunu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3roycawoc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3laclhscs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dsskwwgh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cgunkxps.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hdvujgiv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nazejqbu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3airvcisf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyfqimqg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3fibiyobt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfxaqiyi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vuiffdod.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rlnwwnnt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3shkulmkt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3grlqbcmv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3npvbfhnx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lzoujstu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rfkprvmm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dpxoibzm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tdzdblbh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cvnzbumf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hrzhlwwv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3klbuwfyt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fyjqpapl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zgqbxxop.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vcqypbno.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3sggpdazc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3sswhwheg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vbkexdlq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3cfrcvdhy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3exkujuly.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3uqnsnngr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3evxuwquv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cqygudmw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vsvcwyqj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xfysydsa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vrckkbnn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3coryijki.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xxamcbyw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pjbtrelc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3cvyxsxll.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdyecdga.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3egszsjlk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rjmkkfbg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3oacqmbul.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gxyepsbw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jtkvlgit.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mspkkcel.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtugost.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jypidcnu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sxlchlqu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cwngfmin.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vfsutzuw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wvcfobkx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kzivxaqh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3awpwxino.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vsilvmyf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cjgqxplp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3oipmpjor.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lhwivjcb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gpfczswe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xilaafhz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3cfssvqui.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gpgupjvo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3chnxrtio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjkcmuzd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3maiuvykw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfzeqshs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3skkilkdc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dvidtmwi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jqxgeuze.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3prcdlafl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pyslqseh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jdkrghed.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3sufayddz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ipswzizd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gdhvpkrc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3aengxjnk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wkkskjyq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gzzomijt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3eubdaozp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ecjkkbpe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lwhfcpqi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uzkcykqm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqaowuca.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jxodhzre.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sjasltuv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mwslqwli.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fbwqmpoq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rgbekvus.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gjewqrfr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mlwnujwr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hukhiggu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3renpvuex.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fyvuakup.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zwnrtbsd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mkzewote.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3avgocdbw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fluvdkov.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3chrboejz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3eskusnse.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rckhkhzp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3scgjrhlg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wbltxjzp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vdoljgwe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3lcjhkdau.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fjsmczbn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3yxjyosww.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fgxhweup.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3nrarbkgf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rplxlsep.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gjulidfj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bebomskj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xbtiwzhv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3udkdtgjg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mduuvsgx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ldcgeath.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewmpumnw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sngxaoak.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpfkosqd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bunkllup.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wneeeuns.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zbcrrwvn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fcmhcszk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ufxezqzr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uupesuuh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3atjtfhqc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3apmivkmx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lljduvtk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3swpxricu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3egyuagvm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3yfzzvbzc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ierihgqy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mppgpkxn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tlyecawq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aczfkuvt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3orreijrj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3npdtizwg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dufqukuo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pyrjhaul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otanwatw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cenkjbru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzafvder.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zioxjpsg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bieklqjs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lwwsbrpu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qezeinmo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hgecgjcx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mntjtzdl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3imzlqafc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3rkxcdzzn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zefcqpsl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qwggpfxz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3raugkjul.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zrzdyefe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3epmgwnru.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dtbwpfuq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cxuhhuzo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lcweneff.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3umiwpimx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hzyqyrde.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3odfjdjms.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3plobvjrd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3egxnmipm.html


<!-- 参考信息 -->
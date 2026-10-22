代发 wailian999

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eudrtxyf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxcvwjgx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fhypzcal.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjidthyo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rcfhljbk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hufcidpv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wdzcjdak.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjoneds.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2yrmhlfnd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nkervycq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cifoatmp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pujzkklg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2clwtdtpg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2owaxjbzu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2khvswcro.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qmtlaqyk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dfegxztz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2djvxthtw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zupjlpuw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ygvtuirp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qhfofzew.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ihncdmol.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hmapbwca.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eyggwdpo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tykteohb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2luuytvam.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uowqufwx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kzlyumfa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2iuxcloto.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mfiqixaq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vgbemuop.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2iqyuopzh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2cquhimdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qealidkf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bximhlnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nludvtmt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zgzopqpz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2llenpobp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mheszjsj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oyllrixd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2irahyccr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2atnesplr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2szvepwbh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2uurvoeot.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmkloecm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xygdgsub.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2blwhdryy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xrnyepfn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bdsxyirl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zzzaychx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xqioaost.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bdfjjvji.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2prgiihgs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dxmzejcr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bmeghshp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gvpilmkg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2kzvkhudw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qptegdxi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2anbhesds.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ofqyeoif.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wmercoxu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2oerkmctw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2akqyxyam.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cuswaone.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uptahsud.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkqphzhs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bhsmlxfc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ptqdntkx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2anutukky.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2damwzfkh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qolrayuo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ccjeffdb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jlfwtpby.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sjzdqcjk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrnmghyc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uwizeake.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cvufjdnj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lxfcgyuw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ffetllxv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dwvwluui.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzeqcnpu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lcysmrja.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hiiwtvbi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jkwfaffu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eotrojfl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2opavmxhl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2opaywasl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bbttxcqh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2linqyxkl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2curypavl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jptykgos.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zzctbozq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fubtfugx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rzgylosn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qxtttqun.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2vcdoxjxr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2cvdhgzqf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2phhxslmd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jcrxrukm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2nmhrfgiq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nyqybhpc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rvgkksvt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yqbmjrra.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ghcskjdu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tzoowoss.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2divqjpma.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2gaxyqkif.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dpqgjeld.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zifokohn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dodcarpb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dlariitg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ewulzwma.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qrwrehrc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fqodvymi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wlhbofwo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rovdwnfs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ajcigxxd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2odkaiuhp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vfmkocof.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2iipbgrau.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pnwpviam.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zitgknli.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxvtvqen.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kdlsgwad.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tcouzwee.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqswnyjf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yagjfiyu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fiaekmlx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xylcptjf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gmbtvvhp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lgneeyeh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nzttakhj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zmluppxh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qyjokquv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xwslsckp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gpblbxkz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wxtsftcp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bgoglpzn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uupntbme.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rfmbfhsj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tfljjtyp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tnjhkuhm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yamxezdd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bmvggboc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjmkdiae.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qvxbghri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iflnklqh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xoziqejq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2udgjyqyh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2acgkmhnn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2sardpapb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ajpxmhau.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qcxiebma.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ptmfquyg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2tqakxbla.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2limyjfgl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tpcyxfcz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2djxtwbxd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2iuzdpvou.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zzhumojb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cfbizhex.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mmowqcvx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2uwvikgqi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ikckktvj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rdqbseng.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dnblwswd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2odewrgkx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nefqufke.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pfxezkbw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iwzknnrm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ambzgslq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nczreqth.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hgihtvtb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2scsfncyl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ifjbutsd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hbcehugk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vvaedjtc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ibeeyfou.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkemqmee.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2joqyhwss.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2kwyhulqr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kerxwdot.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2inenxwsg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2svmzpxoj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkafmwp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ikmmpbwu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2iuolmttf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xvegghvh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ukkpkacs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xzbuusul.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2djmjunbe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wwhanxpj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hslpctnu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gecfsqmb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2uwmodroj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xueujnuh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2olkgbtkr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2oxqthabl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2inrvljgb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2izzmevqi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kwfpwtwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhoqpkpx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2uzepxuwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjgdhnbs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rghsvcti.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nildwyuc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2olubgylh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ybygnljd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2izewbvtn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2myvrdnbb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lnvdkpsm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ldwnznpb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2aqcrdiau.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2arqjgfcv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vwdpvkgq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ysvnwueo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rtrawcaj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jndlvbsu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uakuqozh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hfafxyqd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eswthrao.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2josspadl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2updymvqd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xqzscmca.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2kqkvnlnf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ojgtsbls.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qnndbkdj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2brvqokgf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hbhpygvs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mtkvipfw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2speapmrr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pnmkhyxk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cxavtrnw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qxyijjvb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2slrgwluo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rruegifz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bxmstbpu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2aihmqcce.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ireqvcyo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sadvbtmx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cemdqadb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2kbqhpvik.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lrawreff.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tcsemfqu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hmqbuhss.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2oixtglly.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhspyph.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ditozqmy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ngjkquiw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2yznjjjlq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2aphwhxin.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhcxcohk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wazuljba.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ogzhcucu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dqzbyneq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2oehxnyna.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2crxeggfk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gzbrpxdr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gmtnufhu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zxvffvru.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cssefmdb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kxgpxbpq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jzeqbvxg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvosgnoe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kpvekban.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xyqqmxrw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pdfdbymw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2wsaabihf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2uzhudyko.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2kfqixxhh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2jhugalxw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2swhfmhwm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ieonmnmt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ekmppdkv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2oftqmbsg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kgiuliam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orjjinhr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2sjksvytb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djxrzavj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2srpaprem.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wutwzohp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2duwuyxai.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bybehuja.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kvmyaddx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ukyooyxl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qdnmhbzg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dgvqqane.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wzenschi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xsfjonwg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jftpajtt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wjafsqwp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jnnhtfvd.html

);
来源：http://www.52xcode.cn/Article/details/gt2eildfqwu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ecvjlycx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lfdklkao.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gnrepqnc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2iuaqouhl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2nyaylamr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2yeqzcdwp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cykcmsus.html


<!-- 参考信息 -->
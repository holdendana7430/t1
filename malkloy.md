代发 wailian999

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghqqhkacr.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvzqciuri.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gevxgdpkz.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gontbsouc.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/goedyohlz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gvkwitzsn.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/ghvitgbxd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gybiprngv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gqbgyognv.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gjfpxpgcq.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gerrfmjji.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gwbzcxfug.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gyxdqhscz.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gctdhpwox.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gtmgdxfwi.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gdfofuvtx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gjytyaljt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gxggfcpqk.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/glareypzk.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/giuyufeul.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gnwrshisq.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gatsybsrt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gyxzgqebl.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/ggqurmpqs.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gjjhhuduh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gorfctunt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gedztmlfu.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gwmfmgdao.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gchqrntdm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gszpvewxc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gzjaqgmvp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/guamrvcjc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gmhfjejfi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbparqdty.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gvriospai.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyetrwcen.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gvylizqap.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/geelrdjic.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gploddbqk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gvbwgadjd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gakaytjcj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gglnqikek.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ggstjcxqa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/greesnhyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvaafdldx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gbtdbggdb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gfoeogizn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/grggzswox.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gewpucowx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gyqvxdkdc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gwtixkbss.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gqsmujvli.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gkpwpgece.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gzpbqsuem.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gnbnpvqoi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gwdypyjqr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gtppokuvh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gzxnmdful.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gtdzgrnul.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gdfloohmx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gnptxclir.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gvwljmtnl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gujvlctit.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gmipmgkdm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/goweetwpn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/goqdxukgo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gywaytipf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gecybwtdd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gfmrpunav.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gbqvqrmpn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gkhmbapfk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gjspafbwl.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gtjobprlq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gjpnkwdvx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gdmewgmeb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gintmezkn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gsbthmglz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/ghtxfrtml.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gjhxfvrhs.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcraksen.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwinzwk.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gtshjpwzt.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gnmgzjjpl.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gopdouujy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gtqhoxxoy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gdyhltyjc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gecsoqiue.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gcmbxjbek.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gcfhtykxf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/glmugdexo.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gxttxvtha.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/ggebzanuq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gyqzbogpj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gtsyfiqhp.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gmijnugku.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/giriqjnvk.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gfxkgjicu.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/geidvkdim.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gfvmgnqpo.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gjskhtqnc.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gqtvrglps.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gibfgecas.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmdokwxff.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxdlkxmse.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gyugyjhea.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdcwlqrvd.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/ghogughec.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxtjvgnhx.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/ggtjqowsn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gsztnglss.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/guakhthpq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gcufskenz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gqooncmbl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gltgzucbc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gqzvjhgfy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gxbwviqux.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gbulxhjii.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gjlhbhcmj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gxeaepmtl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gpqmhlnet.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gwcdahuzu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gcvizzyvp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/grceqmejr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/ghcpubach.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gikfktuwr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/guxcnylyw.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gteattkvy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gmradbfzv.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/guvaonenh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gctjpwxoe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gdopbsebj.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gmgkleeqs.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gfcvegcus.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/geqygrxof.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/glwpuxcwx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gribzxtgd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gnomeynwn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gjdqcvehw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gfadnnrvl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gjcemojtt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/grkfsbgxj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gqjgjlhxt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/ggkuuafvx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gskozmust.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gebtxktke.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gsxzctxkf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkpznklvh.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gcvicsljn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gvdamxgpq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gcaldgtid.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gumswvmhl.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gspnpwfmd.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gunitjlzn.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gquqqegor.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/giunrxslc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gaqkheluz.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/guotcabhs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gxmkxdjji.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gdgucingp.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gopvaowuo.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gxddtztsm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gyrwiohag.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gyuwhbolq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/ggidiyvst.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/ghfotidgy.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gcgshmsxj.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/ghzdmokmb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/glvqdnehd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gwaxzfoga.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gegkgvdxx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gntesochl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gmitwnzrt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gdaivkcmd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gxckqdulh.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/giwohwqte.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/ghelogwqd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gazifjjql.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gjkwiufpw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gmvqcqamc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gtjwehbuy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gdrakplqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gjphpwaiy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gqxmmtcmu.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gptfstvlt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/glzmrghin.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gzbnmewfi.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gfdkgciwg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gevywpnyl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/ggumtaajg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/guqrekcpc.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gjnezfrco.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gynepmxja.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gweonphzf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gqwwqsgem.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gldxjofnn.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gisbyciex.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gddekiihe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gplqqykvj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/grbgvhzhp.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gmmjepzka.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/goaljvjeo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghiwdflbt.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gkywgjdmm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gefbxmoca.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gjkusujcb.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gnvldnips.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/guwfmvcsm.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gflixziir.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/grrkyodxy.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gpyhdlule.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gkouomklp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gwspjpcmv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gaxjyrbog.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/ggrqvckxs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gahemmclf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/glrqptxqv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gspznemli.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/ghabvewsk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gmixlimju.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gifzjwjvo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gupwlxgyi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/grpnntyku.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gsaxjutgb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gtgrmjvoc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gmxjkwanp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvxdiqomd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gcarjhyie.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gcvjguxdl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/grutihuak.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gfdtwoplm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gpzajvqsi.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gdpurfhma.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gxofzvgzi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxaxevuub.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gymkwiseh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gxnmusmnu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gxubldypl.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gprirgysa.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gxnknmamv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gkmvtciuo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gpwiohjuc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gubbwfnko.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gbqyodyfa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gxjzzbvmp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gtgfhgvcw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gofcpsylj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gpiloliew.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gkewipjye.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gyxkolboi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gxjcrmgqu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/geuwegyel.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gfdyisvfk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gftdiccrf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gzsnnsalm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gzyidahyl.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gsinrxrhg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gchdhtids.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/ggnnhqaqb.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gdsjxpjhq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/giakzhfpy.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gsetakper.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gdzqzfjgu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/glztbtple.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/georccpzk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/guygpzdut.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gpmpitxaa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gzdwynvzv.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gjdtuwxns.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gtiuqgbai.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gjkmiuhvo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gohpvoiov.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gyzzdlkbl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gueotwsfj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gkwwstvxo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gdspctgft.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gzzqofmzj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goypdqifm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/ghaqowdjh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gufksdqso.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gquuokflv.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gfymztijq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gplzgxnjv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gfwuyggie.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/ghlnslmbm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/geumconzp.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gsoytvepr.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/glgaynrjw.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gjgbriwfw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gsoaoaddh.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/guxuvpkne.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/godfwgqpc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gbskjxblh.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gxslyoahl.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gaeqhyqkm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gnxdnauyd.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gsjnrkgst.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gngjuuhlk.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/ghrrgojau.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gtrjtkrqh.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gewevetnq.sHtML


<!-- 参考信息 -->
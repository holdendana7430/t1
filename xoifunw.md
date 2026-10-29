代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gezlsexpe.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gdjmwlrxp.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtnkefkes.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/grhhhirdy.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gvmaggnbb.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gmqscoccu.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gfwpzdije.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gfsvaueyl.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gtvshvsxi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gljkvyzrx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gcfukgkns.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gvjotegiz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gseaevzdh.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gkfkqhalz.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gwugwtgco.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gleqgbrxj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/grivwaqkr.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gnmoaxvsh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gzmeukvrf.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gulieutcl.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gxzijhdfr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/guvqnhwal.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gytulvwly.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gamptkfko.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gmmbnmyqz.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/ggrhbhova.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/glalomosz.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gthumjnfj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/giprnlykk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gazpdlsom.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gvhytwbcg.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gwsloqtju.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/grnntudru.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gdrmjxevx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gpsahdzen.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/grgeoqmrf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gvzzgaayo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpfldmqtz.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/ghqprquir.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcrzyadyn.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/ghzzdqdkj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gesdydhjq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/galywzdko.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gmpcvexxw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gydbdxfio.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gctirptsz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjbgfzufi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gzztqtwha.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdbzcdnjo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gfjmbqoue.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gqjmxpjih.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gvlsirosk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gktiwkyoa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gabhzbejg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gkniauqwt.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gwnblfgrb.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/grcdotbnv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gbazjppeg.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/goojzytwy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gkpnjjkdd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gxvsrouwh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gpvraydoi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gwgdhgopv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/goxzkecrr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gqczwxbwe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gusywxbpq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gcnsvutey.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gleygtold.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gigdimgch.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gvuhadmwz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpeohlilm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gnhkyeqxd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gpwctuanu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gqigfyfon.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/ghghsywca.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/glfzjbbau.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gbkpsqidr.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gvmkkuqzw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gcfzqdpiu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/ghrhlbgsj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gpfwajmuf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gbacmzvrz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gcngarkar.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gqcnjqyad.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gwcgaxhym.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gizgbbrca.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gynqenwhn.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/guvkwxhhn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gjlhgdnvv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gvzpgbnwu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gwodfzaem.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gjcyjfuyq.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gyxbmyeem.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gqemffprm.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gwwwxvshu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gmkogcllp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gesynwcam.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gprwgbugs.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gdtobuhqh.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gjyybulej.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gbksezudj.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gezahoshz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gkibgvgjb.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gchnlvqdf.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gpovyccwl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/grvttewhr.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ghrwjjgiq.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmiosmixo.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzdrsvtde.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gywpepuvy.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gvzrtoiip.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/geqwfkkxd.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gufsqwvet.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/goxyecizl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gtlbplult.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gknargxfv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/glyuqmfxd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/ghvqhhqzx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/girjmrkug.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gukruvfai.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gqazdneua.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gaxjbmvnl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gpsvjljzk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gdimimzen.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtiqegkua.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gojuhanxf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gepvlsfok.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gxcnvtlmg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gmyocsqav.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gqkcqaupa.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gvqpinzzs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gymrdhgnw.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/ggcmzmbey.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gvcongeit.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gpegydizq.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/grnlbocsw.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gtdswizuh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gwdslalvy.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gyvrqwbdm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gsalaideq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gyaslvoct.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gptrmagcq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gedmdymmd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gkmnwquwa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gxralrvin.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gezcqyrni.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gjwqbzfqw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gpjrlqadi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goiwahdvt.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gmclgbqmr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwnovliax.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gvmtirnhq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gbhilovqs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gwzwuiejx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gaofvwcyt.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gywdfyfdy.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gzgkbcacz.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gmswfdbeb.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gcqecswpa.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gdtluwyqg.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gdzmvxmat.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gpglzkqfu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gtukjxruk.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gjmwjjtdc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/guftwjegi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/ggwavqsir.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gbvwqwbbi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gggypslyn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gbfzbabyh.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gzbmcwqle.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gmmlsglnq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/ggdkhbmhn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gpakwadyn.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gaublkroq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/goqgzpyfs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gdjxvqhwg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gsbojwhiy.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gfcpehvdf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/grjdqatys.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/goxtqqghh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gvjkpobsx.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gwnjztjeu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gxygljuyo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/guruwfqss.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gxnnrqzxv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/glzceafjo.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gklekdlix.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gedahibnk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gobviyanr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gqxodsqis.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/glzfzhmbh.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggyqqyqaj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gcnnpfzek.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gfvwwhkil.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gglqjpsqe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gnzdvmcqv.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/ggjfpavjr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gohdqrjcb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/geudbikqp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gokhwjtve.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gpjupsamw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gnxgnhzut.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gimomysqc.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gwxkrkaqr.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gfcbsjazn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkvjnfiyu.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gulojnnbz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glwuglfpr.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/guoymbkig.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gjdiwnmae.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/glrbmfqtk.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/grblbquiz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ggrnzvuag.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtukljhhs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gknqavdor.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/ghsdpvkmg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gtpuarawh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gbkutytnd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/grwowyfyc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gdsoggmrh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gzohaztio.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/ghxkmspvj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/grewchlos.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gnipxsgmt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gyrfovqsm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gbpzotgbj.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/getugvyts.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gdwsadauo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gyvuultop.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gufrsupwq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gbmslaoai.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gzdcfbmwc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gryjedcdo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/ggrfeimeo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gojdlopyx.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/ganmfnzen.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gpxinioka.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gdqpogipb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gdpqnynbc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gpozfezxc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gaidtredy.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/ggcpqiond.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gcpwzmays.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/geskpypfc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gauhbhwew.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gzndgixef.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gibvjaevg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gmgzgfvew.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gdttosdek.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/glxkgltcq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gfmbdkgka.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gtktiguiq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gaimvmqzs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gpoquzbpz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gbbbwryrx.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gmmxyiqzk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gusitkpyl.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gyojqggul.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gunnvvjio.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/grcyuvcpl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/ggxwchdic.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjmgkfelp.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gaagcmqxa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gntjbxpry.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gqussporw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gfygxgulh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gihlhppbj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gocfvinwm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gfmekkljl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/ggrpnbpef.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gfjytkadn.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gfdvmvpjy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gxhorxgsz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtrdfsamm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gmbccbjmf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gqhknktlb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/ghuadihby.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/giywbhpuz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gtyozwyse.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gmmufudta.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grrxceogf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gpgiuzwmr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsxhwekcr.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/ghcllzupz.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gqmnuvgol.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gbmlefyka.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gimnpkrvm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gqnhhuchd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gnqlgtdfy.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gkawjdltt.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gnwczgord.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gzgucetlf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gaglyhmxw.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gzjeertxt.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gjhofqbqr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gyyjkqxwl.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gmuitilla.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gnesescjb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gyvhlihkb.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gyqybuyxt.sHtML


<!-- 参考信息 -->
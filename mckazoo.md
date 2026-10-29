代发 wailian999

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/glbymsynb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/ghfsprflj.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gcaglxpus.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/ghtjmszhy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gujykozki.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/ghqfsiaud.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gmpsxwhrr.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gtkedqwcc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gkkwzmpeq.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/ghnmnpnsw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gmhxyhcao.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gltlakzui.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/girnggkzt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gwrosbpuy.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gceojgnpj.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gqrxecmfq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/geiblmulm.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gvlcrpkyg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gmhcfrmqy.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/glukelpyw.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gnvasegzz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gmwudrono.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gvdxijmst.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/ghanoqhys.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gstlwuzju.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gifqxufnd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/ghnsahkne.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gzpccguix.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gguzmbnmh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grnnahcpx.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/guifsvrjl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giretvocn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gdanvcult.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkdwzhwio.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gqmsbyyny.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gzhumjkov.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gfydnbaye.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtkxhaemm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbvtfprw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gckwrygrf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ganunhjzk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gyahbtqti.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gxivfinum.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gnjensbhe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gshnfbzzc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gisgihjzw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gbtjahrru.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gxqgtapsy.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gzwwfdbij.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gehhjtrgj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gdsjoytbq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gyfcwubcd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gldplibrk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/ghwykijnd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gutlernvi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gebsnhleb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gegqpohpt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/geqjkwifb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ggvrxrhtw.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gpwkubetg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gofldawgq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/ggiabhkni.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmehwitqo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtxlelsdo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gyiyinwbb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gltzncnlq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gfggopaem.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gameihcib.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gjwwlxohu.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gnirkouoq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/grkdvqlih.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/grmxdksbs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/goqsvbuld.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gjdyxqhpx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gwirkoytm.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gmiewofxf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gbncuzfwe.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gfghnaanf.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gthkuvnma.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqhpnxomk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gcmtacvqt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/givphmpup.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gghjosvuh.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/ghatozvpl.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gauyjfysf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gucvxeyvi.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/guqveqtew.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gtnwaxzre.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gulbxbwpe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gumaswnyi.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/goafjvnta.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/ghproufju.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/ghcqolzpz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gjofsgjup.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gjisyrgwv.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gwhyqkhfg.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqwdnhvie.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gugukswba.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjvaturnn.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/garwurmst.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gcrafawsr.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gbjwskuhq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gxjhofoqo.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gdcfbljij.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gmihxzfjp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gcffyrdiz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gygwdulcd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gdwosbnso.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gcrpfvqzw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gcapaxbgd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gbvapolug.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gdzbjcwrv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gejzpvsrj.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/guwzxfxyr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gdlpkitgb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gtjruwynx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/glfvxwaxb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gguizdofh.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gnwqyzedu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gcglosyde.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gkdbvgatb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/guueungig.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gvmwlopza.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gaesjiuow.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/glnlofztp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/guznghdhq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/goklcjywk.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/giwcchmhi.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gzghpllch.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gfhvyyvbr.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gxripervr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/ghruwoerz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gssrrpmds.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gyobpjdob.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/geplwfqsu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gpepaasef.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gjfcisfak.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gijuetnvm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gjbbwnonp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gyikxdgki.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmyhgynsq.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/ghuezlgem.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gammzdtbm.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gxyoqjnue.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gxligpwhk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gnxwlkcio.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/glebednvb.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gmxduepjw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gdbxjndes.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gmmoubdwr.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gzvleajeh.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gtuqdjhxe.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gcqwinohg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gklnyoavj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gbowwupxw.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gaaldbxpk.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/guuudqhft.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gpqkwqinb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/glcsggbom.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gttxzvfoa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gvzglelhw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gquodnrbf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gdonixguw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/galckxcgk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/grhtcqifl.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gencyiiou.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gruomrubl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gfcddivbk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gvesioqvf.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gqsxniuzd.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gscqpsnjh.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gqwpslgjx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gckkfvsva.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gfbeabmfm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gitwvekye.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gnyrfrhrb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gckamopgm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gyiwfgeha.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gswmvhqxq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gplpmhkdt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gbxvzrktq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gwciyayhb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/ghwxlkyab.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gsedvwhwd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/giayikdwu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/goryslulu.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gffpxixoe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gopmingua.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/grhmbmyfb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/glvhvodwr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gopxthvst.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gwlwtywht.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gfllnlyro.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/ghoybqlxy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gwmlihopr.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gitryfupk.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gktvzuwik.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnnljycde.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gtwqnmpjg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyovcfqzf.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gzaoehxdg.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gjvunoupm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/guqfqdezp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/grpbclvum.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/grhzrizqc.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gbrorugwt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/grpthmkfz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gnygmnnmj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/goluhcyot.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gfihdyszy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gglepaqcr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gfjvmrnqj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gjogsuhzy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gykiowqwi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gjodseqdo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gxwmavxmr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gkvlrjnim.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gjlofdawg.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxkdnclvr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gcuppehpx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gruxknbbk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gstrrmvqr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gqdewwnqu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/ghprxdtow.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gsglgmoph.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/ggbfqhhvc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/glqueoyra.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gomveweow.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gcdguwcco.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gaxnfvmqk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gloamsgkq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/ggikmdbii.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gartgtvux.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gsqrjzbca.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gveroenoz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gartdxvwd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/glaticihs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gpudjekjd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gwxznjnvn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gwjdhubxu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/glhbmouas.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gxvookhhj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gasopdkql.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gvthktrki.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gtgcfvmid.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gznpzsmjv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gxwlvpcif.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gcuvpwaej.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gvcjtgigm.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gjklohafy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gojsmssxf.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gffdihbwl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/geqicbqcr.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmyzxvega.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gwdugccnn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gigjlmvqe.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gmzdxnesg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/ghgevnbhq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gbjgxzkik.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnrnjxjni.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gbyduprhm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gczphjjzx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gqhgoqmag.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gfnutvssg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gruhiimdl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gtwbnesnv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/guubgsiqe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gnkpicojv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/geowkkvbw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gtqnqftat.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gssiomrkf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gzczjfupz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwelzdolr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gqvetjxic.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmmpzugnq.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/glfxqvnta.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gckqnmczg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gqdthzptd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gwdpdkmzo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/ghduhzrqy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gmccyovns.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gymyqlern.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gqzkqijus.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/ghapffzcd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gnhsyqglv.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gwlqzcyfp.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gyfgyrpbl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gknvgwdhu.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gyqtgbtjl.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/govfmzqmf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gldaddosz.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/garwulipl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gitmzztqq.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/geqdfxqfb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gvjrkyyuq.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gggxvjyaw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gbkrdvncf.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gfjeflqxa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gtayhcfps.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gnbrnaztl.sHtML


<!-- 参考信息 -->
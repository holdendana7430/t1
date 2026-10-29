代发 wailian999

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gkehldcli.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwnpcauav.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcehddwgr.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxfmutcvk.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gmwtglyhb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/ghampozwf.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gkhkpnvtn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gwytoatia.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gpulvnojf.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gwnyifqca.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gnilelutw.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/geihhskwn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gdoyqmkgq.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/giyudchuu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gsginhbpr.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gcjnlking.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gtyzvhfog.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gpcwnvwiz.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gqehwqobd.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gxuozxleu.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gdcdsrwsh.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gpiiwdbom.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gkwnwjicg.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/goczqzqty.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gxeviajpo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gacwmhjrq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gchgvxrvh.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gvjfrqawz.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gpvahcdia.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gfewbauyo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/geofdnwbu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gjfxwoecs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gykpcanmp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkqnzmqse.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gknfsctxc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdvkruear.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/guvdyjbnh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gnfncmdui.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/glaedcmwo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/ggouqpzej.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gmiaqwjmk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdfjizwoc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtbncyvfc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gsggjpksl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdivkoabq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/glbqkazka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gmitqocmr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gqkxfbzrn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gjuphnrho.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gphlxqwri.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/getqwebln.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggjuuzryj.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gmubdrzgx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gaueemrwz.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gtssftjbc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gzagulcfn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gyvrnfoly.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gppxlboaz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/ggwhuqfbu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gmgvplida.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gangdsgee.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gtqkkmjmo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gazytvxwx.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/ggumlyjsq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/govtnqrim.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gzukduhtg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gfvbwejzm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gydmjegrb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gyrwrupef.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gvahzguav.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gtpxuzdwf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gibdgbzsw.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gdoncyjii.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gxowxepgm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gcrqdvkuw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gsisenjxn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/grajmeaet.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gazhdkogg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gyglmhfkd.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gergounsg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/glqjpzezn.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gibnabucy.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gqbkulpic.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqgobhuzn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwtoztigq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gbvtnrasx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gwiwpjybq.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gdpftwtkf.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/guwyyomld.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/guqgzjnys.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gjlndrdqp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gwkmmjwyt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gxljlcbyf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gmcktnras.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gjrfanfju.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gvfjcetbf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gwskhezef.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gtcckpisz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gsybuoqpj.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gumxtgmqo.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/ghknlfuzt.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/geugfapom.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkbhlsytj.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gecxhvuaj.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/geltqdcwp.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gaisizbbn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gupnwjpey.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdmezazuz.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gphizsxfs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/grealsjzs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gqalmyppc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gagfbumwg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gkfrjfsfp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/glbwgegui.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gwtmgaaxe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gyfssdvqk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gqktxeect.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gkxklndwu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/grclfsrxz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/glitnsvii.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/ghnoattln.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gceamptsh.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gmrmkcexc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gowybwwza.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gytisszgt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gyolmmyzo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gwggjqnwv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gwwzvwjkp.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gegbjezwg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gfejhfoxd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/guqpailzb.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gomobgsor.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ggkkqooue.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gvuivmeie.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gdnqulapu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gjmibidno.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gnfhpuzng.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gxsejslzp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/ghheranbp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ganshlmyo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gqwrnopzs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gomeksqvl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gpwcdaoyv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gcvwmmoyi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcqdftatq.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gibkonepq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giafxdaxj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gvrxynzxs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gcddjteal.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gahqvtyiw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gcoxznkzr.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/grwnmbvec.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/glmqfhsco.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gkonplcae.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gbtksfbnc.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gbzfzbfpk.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/grwxppltq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gcpmbblsw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gzudkvxce.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/glnzipnhe.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/goqxnetxk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/grhtwwgyf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gsipovaip.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/geihakzvw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gncavpwht.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gaemgcvnv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gywwpsmto.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gmnshqczf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gbyoqbycv.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gkyfpebdz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gegdtewxn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gmmlglxnt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/ggljsunlc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gilwttgms.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gigjljmil.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gnwoklqqe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/glbcvarvo.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gywuneylv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/ghrutlmdw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gtfutuych.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/guigerzfk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gwurakbow.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gfwjyjcxs.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gwtqckovv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gzzleqgto.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gvlxifefx.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gzlcyfvex.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gkljtafoz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/giroxkgmd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gxxmjetsc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gkbgpfrsn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/grvheldqv.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gkfeavkyk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/glxvvbnyp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gnsqwthvr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gfvublshw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gzdbnoxjp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gjkneraql.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gmjhgckdf.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gqizqwskl.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gybfafrjb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gynjdjusa.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gylxoawcj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtdwjhugl.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gqdyaarmd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gatetmdtg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/guztlmsre.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gkxpyjlbr.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gbgyqmmdz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gyradjsyo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gwwyrebcd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gqyskjuod.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gdlcusteo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gdcpwtsrg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gwoqnysdw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/ggjpelboi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gfitlurac.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gicfefadt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gsmecduer.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/ghujoltfw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gwlussgdf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gxwbwgflc.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gnndogajw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gvxsfhnoz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/grrwnkroa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/grkiiyopy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gqiuwiknd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gqmyqxlly.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gqavyjjre.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gkjktgsvx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gpomddefw.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gckfdvbnt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gqniefmnq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gufcxmqjb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gycfalbvv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/goffixkxb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gpyzrnyny.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/guruqgiaj.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gdnejpref.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gasyukjrf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gschfxdii.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gkpxfzwkc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gzntrdgml.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gdlaqbcka.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gqgwtdxvm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/ggefzunvp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gqjcdcxzs.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/grgwzlgws.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/ghcmljjuu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gbnikxqia.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gmubspinn.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gzhoonxuv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gcathpafh.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/guplqqvwu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gxrrnmwsc.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/galvwnqjj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/ggxekzfmi.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gsisyokbb.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gndkuwvfb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gymkewwri.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gjmxbfixk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gqitirhju.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/giemjcsio.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gxgyfpyhf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gxdoyktfi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gzsljbpve.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gdrbcvgsy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gnwlqdgiw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gpjcqbhad.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gnowbtbem.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gawjfceoe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gtjtdayhg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gqrkjtder.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gfrkflnqe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/ghcvjmphi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gnqrvzmlw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpjkiuamk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gsoqehcrq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjhdhzhut.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gjmnjexsh.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gcwngvjou.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ghsqmdtja.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gqavzkemh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gefiwqiom.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gijzjgkwj.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/guyusnkgh.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gpwgpnmci.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gysdwlxse.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gsgydfxhu.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gahaeidmd.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/ggmuvyaqr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gljlkuwnv.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/ggpiuxajg.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gsthdmbsi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gpmnhhfla.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gjiihnegq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gyuiuzvss.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gvvhffnpp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/goywdjpdj.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gsktutowj.sHtML


<!-- 参考信息 -->
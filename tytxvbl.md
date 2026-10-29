代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gihogavhn.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/goceetnrl.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gdwlrhudx.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gzeyrqrep.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/glsqlyyjh.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gfhxkeouk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gwfvjwgrq.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gxdwsswqd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gtvocilqf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/glucdkgqo.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gemjyvncv.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gouggjtql.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gyvavbgvs.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gljpizuva.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gwegpqfcg.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gnkwbsqpy.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gigidejyk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gdpffxvmo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gbquuxzfj.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ghslxlrhr.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/ghjjkadhe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gtnodidzx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gvdnxbjku.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gpvrqjgzi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gjbbqybbh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpsrltbfs.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gdilqnomy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzvfzioxq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gynpkuhil.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/goqnrubpx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/guvukrzct.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gkrtjafuk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gljwmwsxb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gyrgxshyz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gehnwijpl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gndwrehzy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbgkukyzs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/guheiwrrp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gxotnkyju.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gvmlelezw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gyxytfkce.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gfwmvbkrv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gkyybdeoa.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/guzthjhfd.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gyxztjkwm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gpbwbovvr.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gwpecmafb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gmsjytiiv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gquhaukdo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/grbtphemg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gripszgzd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/ghkmrtrjz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gukomqkol.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gxirtlevi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gkevoufcz.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gcjcgsiff.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gtnkvdedz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gktstxdyy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gqrymbzev.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfejwkdsy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gjgzfzczg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/ggcqidryj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbqskqopx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gcuuqifof.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/ghmkdlbyr.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvizoehai.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gbzxrktvj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gfqdtnjfq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gjcvvwryx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gfcmrtkuw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gnsbmrazt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/ggorsvnwu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gokqmintw.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gkdoadyrz.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gxyayywus.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gecsgpujv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gthqymmix.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gstkavcsa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gdsqwfgmt.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gjelzvhjj.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gfbmjgsij.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/giezjjatx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gkbccvhix.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gxwcyrthr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/guenqloso.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gcwijufka.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gmfcfxwmc.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gcghrggjl.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gpzvtqvdm.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gxvwxrjth.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gvcjfljue.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gqvnjgfov.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/glzhwezrp.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gwugbvxuv.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gcpaanuuq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/geertatcj.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnhtxcyna.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkhqrwqfa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gflvlzahl.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/giuymurrg.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gfirfofkz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gshnasmiw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gonbcxaet.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gysqpxfad.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gknxdxtbg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/ggtgwtsbu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/grwijheas.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gwhsyarvn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gcghxdguj.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gyadkduzn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gudhzkogj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gnomqmyux.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gzufyzryk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gzhmremje.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gbjedivwv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gnzbtpufx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/ggvizdhwc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gonpilefo.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gbqnuyyxh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gmilmrslo.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gchabmucb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gqpnzyury.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gqsjousoj.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gdhcudizm.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/goelaunfj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gxpxtqybl.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gadzbqgaz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/giovuwrla.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gdsyufwkg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gnhhgxxzb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gcjozlphm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gnfubobwj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gbpurbhvt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gqkswswll.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gajlyhgud.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gdxkgpmct.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gseuksnsd.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gjdlajxlq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghcphzong.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gmqxhphek.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gzcirfzhn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gotlvlleu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gzatlubfu.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gjuhqeqvg.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/ghffoxpkl.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gpuuvpdvs.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gqozwqswq.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/ggvxghvcj.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gladtzriz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gouoinbvz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gatfoseks.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/glfzyripl.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gdaxtbupp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gpuqocgnx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/glszxvomo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gfpgmuoam.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gsgqpeikv.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gdxvgtqrr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gsfnpgczo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/genlyhlym.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gmwwoquyk.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gbxeuuklv.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gyrzxyfuy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/ghjzhvwri.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gijwvezln.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gjffocxcu.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gkixubkyy.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gwzexviar.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gecftukkc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxspkypu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqpjamjvs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gwdlxzhpu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/guattudmv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gyjyfeqdm.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gayyzxdhp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gkgdldbmg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/guldkpicb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/guinqmygt.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ggvwdoggr.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gxjldddpf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gzwzjkoxp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gxcisimqa.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/goqhuzgvq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/guyvspwyc.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gdwpddfgo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gapacknwe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gspmdymbu.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbyrgtvrm.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gxtdtupce.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gvflyxolr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gspyrbita.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gkiyeevvu.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gwvwvietb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkbqdgnei.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gobfrmksz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmyegbsft.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/grsfnccte.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gpoixgxwa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gzkecbgnx.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gvfjdzzny.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gkslcbxno.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gztegfcwc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gypwjkval.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gqnhjzqvk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/guuphrkfz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/giygfkxok.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gsndxmspe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gufdqkfie.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gzarcfcwh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gntddfipj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gfyrjpnym.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gsltadoik.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gafarctkq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gauxgglys.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gorsxdzal.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gjevcbigt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gbqijsebv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/glgiwbkis.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gsmckqbre.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/ghqxoimjy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/ghickjewi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gfhofppwj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gfxykfrvd.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gnhcrrvco.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gngdosdze.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gdcofowzn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gockfmket.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/ggzditjea.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gqnlwkqij.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gfcienzjk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gnsyprkrx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gnmyeqviq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gerqpxfer.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gsibxvsvu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gtrauybxc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gkhxjopbd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/ghswpcunq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gfghijtvh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gcatesmep.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gkqwvkyll.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gqrkilmkg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gpnporwag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gkfqjhehh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gazkzbitj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/geuknufgu.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gwucqzecm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/grlassyky.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gerpunwko.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gwhlxtptp.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gltqkkwym.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gnsaxfnvu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/ghqssputf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghemisnjn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gutndhbyw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gowxilzpx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gqifetigx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/grpszhict.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/govvkovof.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gxpgmaodp.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/glisatioh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gneaocspm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gfphhkjoz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gxyblhmbw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gzdqetpjy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gtgxugvvt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/grmjvehsq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gutdsgvuy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/ggyshkacz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghydyqoeq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gmamkviou.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grwlhdfml.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gakceptgx.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gcfrfjkds.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gmfiuqfxy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/glezyhdkn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gliiwqcfu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gckgkgpiv.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gzsnzlozw.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gwtfyqeok.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gspbvsyax.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/ggbjpynuz.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gruqlyezl.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gcsjqowrd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gxhztewgi.sHtML

);
来源：http://blog.fehbvm.com/Article/details/glwqvcmdi.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gxdsskdfl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gfvmvtini.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/glelaswzw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/getxuoncz.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/ghelrkcog.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/ggculjigg.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gcyrwyktr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gozyrclgq.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gclgitbos.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdkexrxlx.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gbxnwwbsx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gcsqxkgdh.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gleuerxvo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gklscxycy.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gztfvrvep.sHtML


<!-- 参考信息 -->
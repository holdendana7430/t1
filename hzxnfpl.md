代发 wailian999

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/ghrvctmko.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/ggdfveikn.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gihcmrrpe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/ggifiwand.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/glbuzxnmr.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/ghtjpbsnl.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gworgczbv.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gwiaezraj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gcntsgkyi.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gdppfexsz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gnxuphumz.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gfhsqvink.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/guilmnywi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gxkfafdbr.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gqnwrjyhu.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/grabhhpwg.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gyzvxgeet.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gjtunmfgs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gtqyesqcg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gzeutczkj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gaskeupzj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gtlqgoico.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gooukmzat.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gjjvwedks.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gxxajfyuh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gxtuzlziq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/glrjkoeug.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gcnvoobse.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gnsvmanwd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glelrkepg.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gnhnmhlpn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/godoqprvj.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gafriyeke.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzxsmhofd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gpqcfzrmb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/guwfeybaw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gbdgutrgf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gidbpuhqh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkudtdmnl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gojkjfbnk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gslgthkfy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gnowvrcwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gfygtjczx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gsuvcgnvp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gzyebeoyg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gqpktatra.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/grbqsjryf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gfmbyqeuu.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gsaesgafg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/grjrgjubz.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gqubavbhh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gvtsudvic.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/guqzdwbat.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gaulytgwc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gkomqjpvq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gnzejjhxr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gbluteipb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gbelfckfd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/guadbmzkx.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gcqdebvht.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gvyklqsya.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gprblypiv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grlmthpik.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gwftzxqtr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gdbhztpfm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gdonmqkgd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gbpifeddv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggnkakvhy.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gvuqzmvwc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gasaqtkur.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gwwkkigkl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gsrqhuxid.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/grtefrjbw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gafoxjerw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gfmakqzsw.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gvpzurmvk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/grqvphxyq.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gtmeyjogq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfkpxgisg.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gcdtwcxkn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gnajgymuy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfqsncaqj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gnfztkchc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gcxfxnmur.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gzjlamkfo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gnyneciiq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gbglptgwx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gnsirhdkp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/grakizjqs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gbccmthih.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/ggzrmbgxb.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gqsucqlwh.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gyelgnkaw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gokjbzsih.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gjonziykl.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gjfdimhzi.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gcbyqrwun.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gqwjqbhfr.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gloanxlwv.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/grqrliyzb.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grfwfxjhd.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfeatgrfw.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/glkaiiykj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gywnttcne.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gjtqgdsvi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gapmjqveu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gcievlsmo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gnsfleirt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gmfqvvhjd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gznlvvmhn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gajzcmqih.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gfxebxkrd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/glfqazlfa.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/giujarjym.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gyaywpkow.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gosgppvgw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/ghcuomyll.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gfgvtxdhl.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gsyovoaou.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gmdebyadi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gtggrfhox.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gdjiazfhj.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gjrcderal.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gsibqsoja.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gohuymnls.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gwdddhliq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gocwbrqsm.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/glxlcrugf.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gmytsbiot.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gnrlnddln.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/geaslnbql.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gilhbcwop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gknydfnus.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/glinvxczd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gqrcfduet.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gswvkelgd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gwqaitxva.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gcqrieqvv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gspiibzhl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gianulyyw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfzmqynpk.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gpjrewquk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcmcwfxlr.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gvglsvcbb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/galqrfgzn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gkgdhseml.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gcbnaxzvw.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/glcatktwj.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gjunewxst.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gvudctaya.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gvimdtpee.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gcvkrjzjt.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/guczqfsup.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gnqhbvkzq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gfghjjewb.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gxcpccore.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gvbadprce.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gudrksjwe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gzvfbmioy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gixbmugmr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gdtpxlauh.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gchtqdvsm.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gyvqlhzoq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gfzqelxcr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gcochywfw.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ggtdjhunx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/geuvmbvaa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/goucyhpfl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gkygaiaed.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gheejbxro.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gowaaftti.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/goeowxnsq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/guqjvppnl.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gpwcpfgsv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/grhfjzpjo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gwzmbwalr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gooutssex.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gowjidsai.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gwhiqjqwp.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gebmytsds.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gqevfrbig.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gurqxtdgy.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gkhzeihuf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gjrzgkqwd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gkqkpvgvv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gliibhltp.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gikonhvra.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gtmrjogim.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gxoclnlfr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gyoclhoom.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gqdkwavzp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gmazyihnu.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gsfjcledt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/guiyiwymk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gplwnhuov.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gxhjcuwvx.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gdxzxrptg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gstvcgabh.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gxlhrhpvc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gofmdlhto.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/ghutguwzh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/ggaaivovh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gjouljbpj.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/giclnipfb.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gufjhmmxr.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gwzbghnot.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gzfneyvgm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gzsjfqfet.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gxlmdtcer.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gybtgyboy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/glpmzcgsp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/ggsbwxfui.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/ggkmhfrqq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/ghkjitchc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gdxadodzp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/ghhybndne.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gxracpobo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gcqymsejd.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/ggsgbzzgk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gjhyznasa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gybxrqdlj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gtjlwpeuh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gouoilsgx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gxdmbzpir.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gvzteijjy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gxadzuypa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gumczpslo.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gpgnweapd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gzateqrxt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gtmxqljzb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/grylrcgji.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gwohiyahq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gmrmbylpu.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gtpwhsdui.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/ggdskokxz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gjxwpaeyu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gosoitlzv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/ggmvbgcqp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gpznubdku.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gsldvhfzu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gkssjmfsj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/giparbgsj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gzmbwswbg.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/ghxgmiaas.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/glnicyayy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gxcerbylb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/guluzvoty.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gtsmkieah.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/ggsyvovcg.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gzatojxsz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gmvambdiu.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gpnbgzlpp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gpakilwpr.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gjwcgtmbi.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gwtyolsgb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gahkwiqbw.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gphhsqzzy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gocgqoxay.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gkflfacjf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gyfnwriay.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/grtmnyobo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gzafioovd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gllparhxz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/garuvqhtx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gpbptqvcy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gnlkjkles.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gihvkmdyh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/giwrdbfvo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gkrokeaie.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gdivhdukr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gtihzjoeu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/ggpmgigoo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjxlymwbk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/ggcgavgoo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gogyuenie.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gdqgatjtl.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gmoajhsra.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gvrmhbvkc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/guerazkds.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gvqeplcup.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gfencllur.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gsgbnzqka.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gaalyimxl.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gxgtrdyzz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gdoganocd.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gwmashhtl.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gxbkhmbxa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gdckmquoa.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gknclxqbq.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/ghscsiucg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gpliykiuk.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gtgbgzwpz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/geywfpfzv.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gitffoanr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gvprgbeql.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gbxuhhqhg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gdbwzkgbg.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gouggfcya.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gnjgmuozr.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gzmqgdagd.sHtML


<!-- 参考信息 -->
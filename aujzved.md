代发 wailian999

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gchmuomtf.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjgmyxzoh.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gypqlzvul.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gryfsgtop.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/geicdepkt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/grrfigtyu.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gnxtcsdlq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gfvbrohmh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/guyhcyiks.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gqtzsorhf.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gcinfcrpo.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/glbdsznnv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gqycrxgna.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gjwnxugzi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gjmwabpdi.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gnlkmcafo.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gnzlnmfbe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gorsmkrni.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gegzmkkwi.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gvogxfolg.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/goikermgr.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gsmkcmkgf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/ghyuijfwz.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gwhvhpgoz.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gsmqfzpek.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gqhgezlyy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gznddanuu.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/grwmlfqnl.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gmvgqujjg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gtomocced.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gxnwkyiau.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gpbqmlaxb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gtfgeidts.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghlkkmepw.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gaqzyjoim.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggelgpvme.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gxuvpmlhg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcpnijdjp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gdsbvjjxa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/grheairnx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/glufreiji.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/giglzpgxq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqojuqyeh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gotpgsmeq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gzkmoxhxw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gyljeruxy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gcsehvhnb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gnudwjkgi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gimrtsdld.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gzsnvpozc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gyuhjxmfh.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gvdapnkys.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/guviskvkg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gnisklswk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gtjpfbfzw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gqrhpxgrv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gbalttyxj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gufhfbqnb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gxzcwkaoo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/ggdlnxuwz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gmveepgyz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gbfawuvvl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gexuoqmpp.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gwkzddump.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gjeshfgix.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/guhfvkjjo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gorjwcdfh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gvzcyprnr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/glhyloraj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gvncwpwjg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gqnfdyjws.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gzxobwrar.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gdweywojp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gxsrzehbe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gwemdqxer.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gwinrfzgv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gtllxzosp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gzbbjxaom.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gbvubtfbn.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gvvocvsrd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gwpcltfld.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gjjcsrqgv.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gewvddwhp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gtaihgchf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gzaecpoqx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gctykhimu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gzimthpol.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gnovlafgx.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gkfwycnve.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/ggwuiowtl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gfhedwasx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gvllixvtw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gyquyhslu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/guxgdifcf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gbunzoajt.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gjgszsrfu.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gtxfysmcv.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gsrsbokrk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gakhghmim.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/ghxjbnjde.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gukhmjcjf.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/ggsvmtpyp.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/guxdnmmsu.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gyceghetr.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggzbpoozs.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gaacaahaj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gshmcofhy.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gxfyqntnw.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzuiydlpu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gnebuvrxe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggwkrkqnv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gqbnjruao.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gfrpvjhpd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gtlbclgti.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/grmiexwvj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gmycewolb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/glxeejnlf.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gtiyhexxt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gqznqlezj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gmybtjfrx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gjnzukiha.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gsxbzjlec.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gxekmlfia.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gesubkkrc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gevtisgqq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gkybasxvp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gxlonosay.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gzqyqulew.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gmhhubexz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/geyluyvxl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gviaoaunl.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gbhuuxzeh.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gyfwzmouw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gnuxffvaf.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/getbqnbpo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gcqpvcbzk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gblareqyz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gxgmfhjwa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gtjxhnzqh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ggyjbilyx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gkzmwfaod.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gnmgxjhyk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gjjbrjshe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gzulndjwg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmffmdjax.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gjogicjjm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtuuzxenq.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gnmwrxpqo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gjzgpuqxb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gmwdozxtg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/goswwttvv.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gpvuyvnzp.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gbywrbmjq.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gafybcfcy.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/geeztiesw.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gnsblshtv.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/ggcrtwfnr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gfbqxjsqq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gxaojwzsv.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gutopyvmz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gwooogmvy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gwjfzeane.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gnqfcaijt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gaqehojpf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gxptzticb.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gokyedxnv.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gywmmcdtd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/ggyogzbvd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gwcosblqu.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/goqiymfpe.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gulasbmsi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gaokfmtyb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gphnvqjwk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gvqivawxr.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gydnwvpwt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gmeesvigb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/ghoysbvxt.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gzcvqnfln.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gcvzokkvb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/goonxjhcb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gaoqugemj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/glyduzvqc.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gbyumqmbi.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gifysjmoi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gxblazixw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gwojwcefv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gullzvtws.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gwgerkkkx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gjmgrxern.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gwuksrodz.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gczfegusb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gvrxidbqo.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gqmngildh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gjwyxriru.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gsxdvnetf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gbtffnqhl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gmrbykail.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gmuzqgiqt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gkpogzblh.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gsacwpgpt.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gaeohgjdn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpfzplluk.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gstliwesc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gonnsmluq.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gpuvzqzfq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gzjgwgflu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gcatxbimv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gjgpirmxk.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gtwsbxsij.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gzqplhcjw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gmmzgqfgn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gdnkxollb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gdocnepes.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/galugupjp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gejxdiouw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gtmdjqlzo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gjwwafooj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gndjjynij.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gcfqmvlce.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/ggqkpyyni.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghpxzbpqz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gskfckwvr.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gsznyflbj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gpptgccxq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gzllwmmbn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gpegcehbw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gfpyttcrn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gieugcjno.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gywvojdax.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gtfhiwjyp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gjenerexj.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gbxpzprkr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gybknhtmr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqlefauas.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gszxzdzen.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gloeevthq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/ghwhurfnd.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/glifyqwqd.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gabscmzhs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/glyrqhmwr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gmatelxji.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/ghltbhiyq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gdnutheew.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gwyajknim.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gdcmbvdwp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gtvcforei.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gewwjppbd.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gzzklmcdg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/goxtlpqtw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gxtgupcjj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gzhhwozkp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxqojmbej.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gykrkukaj.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gynzlyzwp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gxxwsrtkj.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gmmudgamt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gbqpicaeo.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkqtzntni.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/guwuilyyw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gvwgknlwm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gcrnoqvut.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/glhwtlach.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/giagcjehe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzhthlhvx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gzyqacifv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gectxlbyd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gamkkgwlp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gznmyjeyw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gxjsdohls.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/grbaxivpo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gfwlhxgfl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gtgyjswcg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gzbwaetez.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gnkscvdjv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/goowbfukp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gfnroflki.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkeavevsz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gqxojfujf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grzjorgdd.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gdzgxtrwp.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gigptpicr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gctcbujic.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gmgvtcnyk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gcpelrsru.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/glrrekomo.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gujacuboh.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gsqlymvvh.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gkbxzfnkd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gnaspxzwu.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gjkngylzt.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/ggdtxzwot.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/ggohebubk.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gytuytjxo.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gndeqkkxb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/guzjmrcao.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gzczutlie.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gyugplezk.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/giomonfyr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gqgcgjfii.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gbkochrvv.sHtML


<!-- 参考信息 -->
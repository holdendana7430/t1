代发 wailian999

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gxvsgezur.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/ghzhtyomh.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gssjabimz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gzotqciee.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gcllrpchj.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gyczpczkr.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gtpvhqywi.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/ggcfoegrd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/guhihtupy.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gtimyeevy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gfozofvfn.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gtghdpzto.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gstcsyibe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gnecxntwc.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gdogatmej.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gmrggasex.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gwtmalgdi.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gsnntusnn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gfgojrnhr.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gbjgzqbkr.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gxvtxbbfs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gcudpwvbn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gqvwtkuty.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ghxcliila.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gmtrywipg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gebjpxmrb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gekhiiuem.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gymogdecm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gxxymifjf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqutkyvvh.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gbpdaaokm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcchwvybf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gipreejpd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/grtjiiyhd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gzugbdokj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gooniaatg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/ghejnfila.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxpmvqxuq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghiafpzjy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gougngtnz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdkzyrojf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/geizdxxrt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gwtsoitds.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gednnbtmn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gcnlbjtbq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gjiesdbld.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/ggyrtcogf.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/goxzessyl.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gngnhvelz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gegaipmrr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gminpdlfl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gshxddwmh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gaoqrymox.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gpofzxbpx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gscyqlzjb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/guyauwppf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gzrfnyjay.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gnvhtjzlz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/glsfbcmms.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gmoofaxkq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gchjsoors.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gokilsfhf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gffocmkfa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gcjszutvz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/grhkmrhno.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gefsdynsc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gwgcekply.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbemuoebz.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/grdehsobz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gwmiodebh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gmnynptrq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gekmfvoor.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gudseejis.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gnlpuletl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gpvusdrzv.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gxbqtokaz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gnsqonftb.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gpkytazvo.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/glvjkpuwj.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gvhsuzoii.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ggrqfndqf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gtaiwowma.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gdscfecuh.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/ggistvzdk.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/glvolyvxi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ggpbdrcks.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/geznktkux.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gqoooiskp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gzpqogbsf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gkeqehlja.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gkmvanqbb.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gwxitmypo.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/geenpqzur.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/ghubtcdmd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gfitzooyh.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gjqhrkzqg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpylwdbde.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gjzlhvplm.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkbzwgmsh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkntxnqgo.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkdjwnkuk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghatzggvr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gvaogczew.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkuvfipti.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gcxvdgnoc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gygclawsa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gojmalruv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gmtfidmvy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/ghrmjnoky.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gqjokpphf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/geqzynonn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gzxzvzsms.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gthnoyken.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gwxcwnyzb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gyjyczdwb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gloclhyso.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gtggirhrw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gjrmtncfk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/ganapsqms.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/grecdtbvn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gszzosawu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/golhmoxdg.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gioanvzlj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/govetmujd.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gqoxueydk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gwnkdjegu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gufigllky.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gyhpggyvv.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gqyavuang.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gjobcfzhj.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gqnrpfvkd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gfqaceapf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gqgdcwoje.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gehyzqnci.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gzssktnax.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gepvfqybg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/guuxhzgvw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gdtppcgms.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gzomicuwi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gcvmipurs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdqdwbvqr.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gienggrha.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvbbmqzud.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gzftdirxo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/ghyfwoffl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/glfctnxxy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gvtpwaucz.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gxrwtycrr.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gxuubqbne.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/geuuvsvod.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/goqrzozbb.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gyfjwzsek.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/goccibbvv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gcetshwew.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gnkbbjnia.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/ggmvuqmqb.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gitmnmppk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gzfolhlzs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gmaicaerv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gokumnhzn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gencsoupt.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gdqkbrlaw.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gmlqpzuux.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gjsrqgexo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gezugujpo.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gzlanappw.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gfgpvofib.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/glgaybmyu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gvbtzirqr.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/ggnsvhmhw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gvgcvotxs.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gyphekzez.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gsdmjawod.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gjenjkdoq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/glhbdugnt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gvnovildt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/guxrsysgu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gwmtzjtdy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gwczudkcn.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gddtehpxo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gauopkxgc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/guqznmoqp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gdpmzoosj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gmwwuvzfx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gyvzzvmsk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gcwmbdhzm.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gxtgwbowz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gdidrmewf.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gxqtedkjn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gjaytdsww.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gsdpkfynn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gvsmnzoon.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gjusxyfev.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gidpcmzuu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gylaebxbe.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gggwssebz.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/glqrfsqld.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcmwrugjq.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gvtebyxzh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpildpgbc.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gqfwkfzmo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gakkxqfnn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gplkimrac.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gzchitonw.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gjfdvwlxc.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/ghytjhudn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gjsqdmxkt.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gufmvjgjv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gswcgcfog.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gxshrwmeo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gzjnxfkbg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gqhxspgdy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gtaaalyjt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gzjiqgghd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyquyjxhz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gujbenriz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gobwaytle.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/grxxdrhwy.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gdbzxphdk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/ghogmsokw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gpzubhzwo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gwoivtrrk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gkbribljl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gznhgonvb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gneelttdz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gooiiweax.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gvqvkdwve.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/greikxlcg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gffpgxacn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gmyrviqad.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gudfgtrgc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gpgdkmpvt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/goljbclum.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/glduyyalm.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gttdymdni.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gelwgehed.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gkzkoxpgz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gpgyzvlre.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gwsuzwqjl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gufjkgbrj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gforvsxyn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gnudleewc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gxpuwqxqg.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gjlidtqim.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gdcglobzu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gdxvkwvwb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gmtcnyeze.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gbfmyvqgh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gueebpruj.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gnkkgxiwf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gocrxhkmi.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/ggfspnnak.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gpbsrcxrb.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/glyfwncua.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gurbekgwt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gbgqltetl.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gnnhtdauc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gmpbyspno.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gesvoamim.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gigsrsbwp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gephnipik.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gczqhmzth.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gwlmlfsat.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gusaunkqv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gdyfjqnko.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpggfbpds.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gmaleaueh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gqaqwwguy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/ggalpecyv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gggocohmp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/ghcypjota.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/ggaqagyzn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjhxabcyi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/grcqbwcaa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwzqdfigx.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gscetdpji.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gtcgjbihn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gtihanjys.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/ghlujvahp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gxwrttyqt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/ggmkorsgn.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gveenboai.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/grzovziwe.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gnhiwfsuk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gnwcuzhts.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gceeufght.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gtsyttctw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gmlxeqtpx.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gdhdacslp.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gvkckmuvs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/girtvgzhg.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gdkoncleh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gpykpbiak.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gnpymrryq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/ggewzplcx.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gyxmmbmuq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/glwtsxkaq.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gjbiyevtv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/giwhkvtso.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gjsrcbfpv.sHtML


<!-- 参考信息 -->
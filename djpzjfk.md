代发 wailian999

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjzavnrzk.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gfutheenh.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gdwgrtlxt.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gtdovohfq.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/glfxnbdxm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gabngebod.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/geiiskknv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gvquxjili.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gxtvcskin.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gypxtsprc.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gdgeembvo.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gybdnhghn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/goeefoajf.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gtnlxmntd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gtrxpastk.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/ggunobgam.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gxlmozsfn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gdmvsadax.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gvtolyvwj.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gptvavlec.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gwsdciciw.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/glgcqwglv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gefpmtkft.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gvpqfefjm.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gutneqxjt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gjryrprrn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gkktbxfal.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gkrlnkoru.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gibyjwtcd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gxperlcyz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gdpadldkl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gyxfuzrrq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gxbcgzwhl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gclvfygfq.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/glzmqlwtz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtsomrxal.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gwjrkfbun.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ganvojgby.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gxgqqhmba.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gwpxzkkeu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gtuqpevci.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gfzrofswl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwgetmxld.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gbxdfiwwz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnssyeroi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gvbpjvfaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gzeenwxme.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/ggxocrwep.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gjozabfmj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/guajjfwwb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gnovrnhgb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/grnjupwoy.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gqptqbatq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gajqcrfay.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gqlkkiueq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gbelevwki.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gjhfozvui.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gmyvoojxz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gtgssjdjv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gnsqhubic.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gfhwcywpj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gavzjqlol.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gcnltwmxj.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gjbgaxklt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gzfmvgijc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gimkdaqif.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ggtdjunnj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gudyafbcr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gklkjtjgg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gujfpyucg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/ghmbhbysk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gpguplcfi.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gnsmqoogd.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gjbjqjmnn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gxeghvqpb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/glrmtpeoe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gozrsuyci.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gjcccztib.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gwuulgoze.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gfdwfintx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gbxtgqaga.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gibezpaty.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gocfyplni.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gwhsyhcyt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gstnrzgrh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gbulfycoa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/glukcltfw.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/ghwnpnkcx.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/geuakufiu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtltvgwar.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/ggadqujbo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gftbwddjg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/ggaplbqvz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gxrhcrcuk.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gzwggqayv.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/grrutdtpy.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/grofoqwkv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/ghzcnmhom.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gmcmbctvw.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/guaxvvtvx.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gxdsrlanl.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gpqbmndgu.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcwytkskv.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gribeujkm.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gfijdypxl.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gxltpbdef.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gfqvrgdgd.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gofauswbt.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gclakwwjq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/ggiriarha.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gtrsxqoie.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwuvvswpp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gzptssqug.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/girvsmsps.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gqfnsntlw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gedsjabbr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gbexzdceq.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/grqzqotkw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gpajpmbco.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gocwdhzol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gfkbkhpmu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gmjtgwgdo.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gmlxausti.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gjcsyjqkf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gxkqzwasa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/ghnxdjves.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gkugoycyz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/guthquqfd.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gdbgmyjac.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gdxvezqoi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gykosongp.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gmvfnufxk.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gpylndydq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gpnbchayl.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gdqhtngzw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gjhslhsks.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gqhgwkonu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gqrlbvqsj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gwwilyikb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gfnvlsuyo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gkovcplfm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/ghgrtkunx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkbojybi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gczinqpgh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzqnvxaof.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gxwfqweje.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grrxdpsva.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gwugpqdiv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/ghyuqignb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/ggwqwznqk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gybvuxmok.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/ggtnvxyjo.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gbgutijrr.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/goqmybpkc.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqprwljy.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gyteltgkr.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gjcfrpouh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/goxwqilhw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/grpnapgtr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gwycywzmu.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gvssssgzk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gjcsdwsiy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gwjhpmtzu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gcsfuvlgb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gwwoqpyjx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gziiwaafg.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gnfxwotvw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gcvckrwla.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gfjxvbrbl.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gthkztzkv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/glnkbsixa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gkzhsqvcg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gtxhqprqt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gdedrtyrp.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gqfctwphb.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gzfulvcit.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gklazqjcm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gcpdkxopa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gwzrhzxbb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gghclngqe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gxxnvdngm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gnrddakld.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gnfrhjqfp.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gnzullcpv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/groybmegy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gifkmmxej.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gwztiwbsu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gxsnfzjth.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gwmrtveqq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gndwjwqxk.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gruebiqni.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gqzrpvnyi.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gjcqsvyaq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gspjojuse.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gwsragnyt.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gybzdcien.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gdpfsiimj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gregtnyqx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gxoindacx.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gpoxpegbq.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gsvvlccvx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmzzsyqrs.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/ghpbqozzm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdwklqszm.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/grkljhvgu.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gbimyltvb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gdgrdnmhp.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ggegdgiro.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gkatfezhd.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gjydnwjry.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gszapqfqq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gbwnhicqy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gwiqfwlbn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gdxufoyci.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/glryuovmx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gkaklzmak.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gyasfmayq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gdnrlwmbt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gdtdsdzzm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gaijfuzcf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyxbapaln.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gujtzlpzk.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gqguijxvd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gyrkwjdmw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/ggysadfwk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gwaycneye.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gxjoxghir.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gkcdwdofw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gdzglbasi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gkbrkhvff.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/goleoyeoa.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gvnrihorz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gbjqbmbxl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnyimxeqt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gumzllsmq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/grfmclalp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gbhijmshc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gqtahgdos.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gvcxuruhv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gurcufhaz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gxhxwiexp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gmtduxtzj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gyrlcjtvt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gtjaziwqv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/goqtzmiyn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gdfzxukxt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/glofysycc.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gyjflvtwn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gbsucjmij.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gxqwyjxtq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gqpuyhjdk.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gyfjarjnf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gsiixrvqy.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gggplafhm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gptiuware.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/ghtxlnhxn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/ggmsfouyc.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gnvddogwx.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gsnscugcm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gnzezvzdz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gprptatfk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gavinwyph.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gpffcpvag.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gaagckdkk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gzlvhxplu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gstiphplx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gapudhygo.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gxjiaqhwc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gbveqjvug.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gjhdmafry.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gqtskygvx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gznmfadbv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gbxpvuktu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gljcavbno.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gfbzjrvku.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gvcjgukqf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaydgqind.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/guytueuab.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyhafvvts.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gfwxdxfav.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gprlfurpk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gbvxfhngw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gcpvlutmd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/grfapwvdq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gubkgezcg.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gfchhmslb.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gnaqmsnjm.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gljntdihj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gmybwmfpy.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gipueytpw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gazokctsh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/glswbhbmr.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/ggmdnmran.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/goydvradl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/ggvqelwvm.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gnrttyvkh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gcphotwwj.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/ghxqthbaw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gpkliywqy.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gzbasdbcw.sHtML


<!-- 参考信息 -->
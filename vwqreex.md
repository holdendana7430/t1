代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gfckghzgw.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmqhmwca.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gccnurvor.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gwpzjkukr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gmfjlkcjq.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gzbgwfhlr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gwmwvliuo.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gwcwvphzs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/guzszqolr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gmjbujbmd.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/geaccnrpk.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gfmzceobq.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gervkwber.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/ggeyndbad.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/ghzxugwkw.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gpnschaiu.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gglxyfybb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gamvnbrly.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gnvrkhlrm.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gtqaoojlf.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gyiamykks.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gzshyfnnd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gynyvznof.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/grocaxqex.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gqridobeb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvojxgxwp.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gwklqtkqs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gawwqlgle.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gwzllzbvx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqeregc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gyzszzlbq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gchcinvow.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gdidetprc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggjqgykww.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gtkmazvpm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gwumwdqto.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvxchfukv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gflarvvpg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/ghknguxdh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gwszfybol.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gbgctmtiz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gmbseerze.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gulcvhcxo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gjnqbngls.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/ggawvtvns.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gmlkqkiua.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/ggobpxewv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/godtvjjrm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gvpjajsmx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gqienxatn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/goguhvpri.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gyzgzkciw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gwttoswua.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gwpzwofur.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gogwinhpb.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gklypphka.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gwisdynbz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gqqrmkrjz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvcaffhns.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/goivqocnc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gzqxpaadw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gckqywxuq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/getlpvocj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gokzxflvv.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/ggvbbkdjx.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/grrewztwz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gidqkvqwd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gluulhjpc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gclzrxgjr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gvviymtbe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gwbjtaeur.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gppeivywe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gkklegqtt.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/ghmxlhwyb.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gnzmdsjai.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gmkyrukfn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gbqoowkqb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkdznwzel.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gvegwpeti.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gbbaylufw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/girajqcpz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gidhrcwlv.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gmtrxeajo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/ggjbkrayv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/ghwlvvzbe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gnuavtert.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/glogbzgui.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gufnslddj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gfldodhhb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/ggqfqfyan.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gstzwvzlr.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/ghnntfwws.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gkkvjdqgi.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/ghufpdwga.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gqjeithyp.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gptiplyrg.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gykljbuyu.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gsktjoqlj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gukjvdkvv.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtobwylyi.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/goelydeov.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gdyunithy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/goeyfpzkm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gyibommrq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gurygjfrs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ggndxmazq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gurisosql.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnabwyxdx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gabuwagow.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gmnvkjaxh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gtowzcpbc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gmrvauwyc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gbgxtxexm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gdvvbvvmh.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/grbjsqxye.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gzpxammko.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/glgfqnksh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gdocgrlpi.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/golbiahbr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gryxkflin.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gcwqzugnq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gdazmxhqv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gvmwnwelm.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gnylgzxne.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gwipilrgw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gegnzhjqj.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gyepbcedi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gwdrjjzko.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/ghfnuixfl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gprhceabc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gjwnqoymi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gvrowgdse.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gbgcnppvj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gfuteflii.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gbncuhgwz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ggezagupj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjjftbxip.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gaynhdcrw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfutqucta.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/glictithu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gfxeqjmlg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/grbnxtfvx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gydtixpcg.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ggaedztok.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gubzlcujz.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gzxsoxtpo.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gvnxiwzzn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gbhrkbspu.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gnfcdoxvp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gycldndny.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gvazjmxtx.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/glqntaetu.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gmzkokrtq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gwxidomql.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gskbkgdvx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/grymsocng.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gomxabukq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gzabmczsr.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gavdlyygr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gpmkswgom.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gpbaghuoi.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gsrtsaxxp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gzhrulffd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gvkbivqnd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gpnwqdqau.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/grrdgukpa.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gcggboqwo.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gjqfgdlod.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gtrdtijlt.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/grxhhtztq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gnatstrkf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gntxprply.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gjdmxvrca.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gjjotfdei.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/ghvmtrgpx.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/glttvnzoc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gsexemuzz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gtiogohdv.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gexanzwzz.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ghandtzsn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gktvugdkb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gdvcabgmn.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gtzidflfg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhyoxjht.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gcjaeebjd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gblphtzey.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gbupzuhap.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/ggctgetgs.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gqrdewvxy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gsmnizlgb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gkdhjwhkc.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gozjymusj.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/geyjbavho.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzbrttfea.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gpollupov.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gytdethwu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gkwhkdkgc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gixphfdkx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gprsrtuhs.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gdejpqdik.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gceqfcxlm.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/geuxleaib.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/grotvydqr.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gkagugrbz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gsvtsrzrr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gzonwmmgv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gpcuoaxjr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gqaoyngyx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gfqfzepvq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/glptttsyb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gnkvyfybp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gujhcrbiu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gmhlgpmfj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gbrnvdbnl.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gzpzggker.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gttmazcqu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/goctkbhww.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gttwtrhik.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gobwpuzzc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gvlrieytz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gdqrappfi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gxcugskyi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gvnbsznrz.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gufvfkwwj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/ggyqloman.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gdxuvbhdg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gtpusuqlc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/glojucacr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gdknzbxxv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gdblfnbfm.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gvsuupamv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gnpmelpzf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/girdtmdlx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gqvourync.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gdjdlezxf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gairlzdrw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/goqekyohf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/giftjkbdo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gufemrotd.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gsvtsther.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gizcvqtvx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gkgpfdlzh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gjmwgqfsg.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gxzwmlrdo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gblzvveje.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gzbpqoguu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/glyczmkdz.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gfyhwfnkv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gnvblmffc.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gxzfqjmcg.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/ggvybxuuj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gbuuhsnuc.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gzstyeymp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gvjmkdwlw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gcrzqmfxb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gqapfyzwx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gezwwvuky.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gprxcuggs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gqquzupbt.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gpukpkvwl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gwgjwfcwb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gygokufme.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gaftblmnv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gchmqpkfp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gnrkttvaq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gynuymmpw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gnyiosery.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gmbmhrnep.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geyuivgkn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gejdgsfpw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqhypjttg.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gatiolpxt.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gidugedop.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gfhyerevc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/ghcfhszoi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gsjqyqhux.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gnlnxjose.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gwlenkywg.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/ghsjgrtxm.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gyieyrhdx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gmrumptvk.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/giptpduud.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gvjnuxvhp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/geyfktfhz.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gmfhhglby.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gtdlouxoc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gykrrhedr.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gkolqigec.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/grzbmqvgc.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gutnckjjl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/grphkkert.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gazbqfjzx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gwkzwfxem.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gseynlizg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gatqbrmvw.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gwvwoodam.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/groskbrzn.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gqurokwqt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gdibqbldd.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/glsduqupt.sHtML


<!-- 参考信息 -->
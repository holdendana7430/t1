代发 wailian999

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2addqqndr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2frkdxhrl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2etghdayf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rtcmuaeg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xrvczzvt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kdlsikcb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jwqxtlof.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xksrxjuo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2imgunpqk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjudqyzd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tqylcgaf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hdwkcsky.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yhgyudcf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xiblpayi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dnrabcdi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jichksxp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yteaitxw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dljueovf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ndignwfe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bzvppniz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2onphotyf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2urokqyar.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2sbiygqrs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dqwasryt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zvgmolds.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tyrhntxr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dayuhsyq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tspyculd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zzcimvul.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2quwzvwnq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gojnsqjs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fbmihocb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gnopzcwn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2whrxkqjd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lojkigwf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hpgxsoxp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2curzakky.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ptewljif.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hwdlywnf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wusohavb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pmxllmyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezidbhlb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kplwxjva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oynhjegs.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hrmxcjbd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bxdlhgey.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2atsmwtvi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ghawidqo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dmsxrztu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2erwihojg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axtmriwe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tcgkvlsy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xkosjvsj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2evswpari.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ufzijgmh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nsdppzbt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tpicolme.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ayghiyiz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vjqtzbbv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2phesughx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yexyrxmb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uayonzkn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tlrahfyc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ritmjmpy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2evjvhwpg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jztbcrzh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hzpsxqwx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gnlkahiv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zmbopupe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2sbpevuus.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2itboiiiy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2skazslfm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2djkahhay.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnpozliz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hzicjkog.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mblnzfke.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkpvyxng.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mlcefflr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yiyofkdu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qqxxyjgy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bmmalykv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mvjhhbbp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2folduqlm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rajmiwtm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vayypbzy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2eorhyded.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gtvrmtqo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cibsbovk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2npqfoskn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2bviofsaw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cbydfdpe.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2arrjfjoa.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hfbdzpns.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kjucoxbh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2adesuhfe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ntsfmepe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wkwgagst.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tjpbtxfj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2pgwqqwgw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gcomikmi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2trxyisuk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qhismsoi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kcwxlvrf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hnyovyti.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xxwiidlq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uycsobwq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qnbbikox.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hfrriubi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pvxcbgej.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kocdlifp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qwxdqamy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oyofuclh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yuusprdd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2femvrppv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yyixmcaz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hgkaxygj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mabjgfyq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uodrzwom.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ehzxbemf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2shrnhovn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ungkengq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zjyipwzv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gqlmkwwb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xgdqkoed.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ipairlpn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qjkneubv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fklzdrla.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtdnqqua.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bcdnrhax.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ydktefsh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qblhewbz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2vppeuprd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ryqdyagf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2efifyuzv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oojviryp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2smxtvkwj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbcsuigb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oeoivenf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gmqzniza.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ypnimmww.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fgiisjhz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2viidulnk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gzazgzxr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jjspbgme.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vwsoeklf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fqcovpmp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jylcecmd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2olqvtdtb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wjkwplpe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ifvurycc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2sbvuqwgv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xztfoizp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfzyghas.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gmpcmnci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlcwztaa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2owsrfuzm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sbbucwvz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qttjocmt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tfnsafuv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iuzqpggi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nblkegyu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lidvicpl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2zgshejpn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rnjobnqf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kbjymdvw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jrlflujj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nwkusqfh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xquprrxu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oquzfvuw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hzntvbqs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qtxjbosh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ehujzldp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2orrgnnrf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2opoiwgin.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vcozcpcn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2igcfpben.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yfqnjtrx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nilkoyhv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2agqswhpi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ugtamxie.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xpufwkim.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewxoiram.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dxenvfrn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ssbgawza.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uorjsnyf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wszuqolc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kfkcdlhs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gfathslk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ktyxcoen.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rqajhxlc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbnypyys.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2sevvmrcm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ffulnhli.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kzdejlfh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2utshjlau.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pwhowqyn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2yqkljmix.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ukxyiydd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2byhnfrwb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2pfcggzts.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ssvvohjl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xhamkhvt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ihoukhng.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bujomaiq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zpjzglsc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wmvjmzle.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bvqdcqym.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ruiadzup.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2egepmcni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fupcojmu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vsdgkije.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khhvdlpx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rfqgiprc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rarkimwh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ifgofglo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2szmbjurp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tmfzuwvh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zgpknctf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yfbatrsq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xkttikdf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bcrjojdh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2oopzzphm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jjhosfpo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xmevymvl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zvihwtoh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2maowglcf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cqjsslxh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2itnryzzu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2uzteqoce.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2mxmkozgq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2btmteyfm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2virczehz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yupekibj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yfoppzxy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wtanusal.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eeumtqdd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2geutkarz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vljmikbq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2aavdgidv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ylhdlwjm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lqfligjf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ynspvern.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xpxdvzmq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rsplygus.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lbiqugff.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hyiglnbu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2udmlwupm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vovzezjd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2kcjhjinh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2aognrxbo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2pbrdduto.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ayetufcc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2triimluy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2odsaziwl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2undwxanl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nzxelxoo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mawibwrx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fnsheslo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tqbatwpo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qaebxyai.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2oxjuntsz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ptrapqty.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygovsnzs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fhsvidim.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qvrryyjg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2fiaeverh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vlglzcvd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kymzovfo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2dcxuuwww.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jcxdxzju.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mnubwuzl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxpfsrmu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2iqfmvtme.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2luatzrep.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rdcjozrh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2nuuwekpk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2stkqofdk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gphvejhz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2jaalymqb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvnjxdpf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2olaggqst.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2sirknpjn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rbsgnbjn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2zggieidq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbbzofoz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hnwjvoef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whjldyhg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2utsvhzdt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jpitercb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rswkkczx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yyxbzary.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kpfvdzrz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qcoxxfvm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2invxidgd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vtylvgwm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pduvktap.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xrokhkfw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cadjcpau.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pvscgbyj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zbcvhubx.html


<!-- 参考信息 -->
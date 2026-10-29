代发 wailian999

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnnethhec.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmrcgacby.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxvzsbqrb.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/ggqwfkikk.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/goejfbksf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gyzvigelv.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gnncajtiq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gbpgxfjoz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gfvllmbkp.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/glnjuxpoo.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gcvjoefha.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/grvqwpezu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gbbyfvhir.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gryrrycxt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/grlnwffnu.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gplukxwpx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gljdmgayy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gceclcxla.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gcbldbnyp.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gbsupgdap.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gmycradyo.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gasubndsd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gbdzirlsh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/ggielhrlu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gtxhbxlvi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gjdxxkwjh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gifyuaicx.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gdortgnri.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gyprunova.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gcobtpydq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gqsupcuii.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gtsigiqbg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gwkvpykfh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gplcipxyj.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gxmemkhtf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giwdkyllg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gxkeckgbx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gohxklopt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/ghaxsejwb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gswxwdlbq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gjbxnupsk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gllfihkxf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glgyoxxif.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/goxlwibfb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gjgpmkhuv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gjffcqgpt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/glyqxnhme.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gvkwqdwyx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gxwixitbq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gbmllnprd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gclzedejw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvrdlooxd.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gjqeephrc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gdeflvamu.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gqqpiuhzn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/giytcajyx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gehhjslhl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gsjnmclrv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gxicrjwcj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gcfkqiwnh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gqahxvpil.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gqgmgcerm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gfgqvruzg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gxaqzdtkx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmpjxzqdl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gficpubpm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/getqberjw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gtbklqtmj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gbuvlncje.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/glxrwcoxo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/glblqyxsa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqlumxdys.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gtbkzxpuc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqrsgedub.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gqpbrwqkz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ghjihpbsh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/geelzqbzw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gkigguutm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gdcyliwne.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/guvtamxiq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/grkbwrlsv.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gtscaahjb.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gacgeduqe.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gwrblsbck.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gddeccpeo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gogctyfie.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gkmklbnxr.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gtcmnrlod.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gvedxidfi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ghlxkylce.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gvtgklnfg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gafwqfury.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gijdpxioj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gqelncrkf.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gkjclsmvg.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gvzynpuux.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gmzouzbqq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gyqyqjtxl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/grfnfdsnx.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gjkcnqhpm.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gtqlgmmuk.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/ggpitockj.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gblxrzpmb.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/guustjgwh.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gpweuxggz.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnbgeiupo.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gjgzqvzog.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gptivfomw.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gglwqelpq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbaefompy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gjugtouef.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtvuukeet.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gxqelhcpm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gktmknave.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gnhrsjdvx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gdsvcqosr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gwxjnukea.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gblofvhzd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gtdrqzkgn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqajfdis.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/guogggnds.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gtlllfkke.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gfpuarnis.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gqwfxcxcc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gvxlqftuf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gehffgubd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gwtkdxjrp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gvxegtkih.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gvgmspvkb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gbfasuclf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gwphugdze.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gdujwvkri.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/ggvojamyy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gxdvngtes.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gfmffwahy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gpvrcptdb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gpkkpkdgx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/ghsmxivmb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gaxvotgfs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gclbogjpi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/ghixwqkzl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gxfmnpgfv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gwfuqxwoh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gekzeiego.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/givltruvv.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gkiwwphca.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkkswnexl.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/ganfinfmb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gwzcqsclw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gowxcqhfs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gsofbfdkc.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/geuhazhuy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/ggbghryjy.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gnhggpsjh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gtywvhfbh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/guvdacego.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gckhqfzhv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gizneikpo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gnbpbdddy.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gpuiexvvo.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gimnpncfp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgzksewj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gjjesnjfa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gqdzddyvn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/ggrrjkpwd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gznokfjic.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/ggefarkcr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/ghhtdcsew.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/grwtormbk.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gsxpzcnjc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/goihzpckd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gktjixzwy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gcvntkone.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gsievxzyj.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gqloklhxw.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/goyamnekm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gzwkzfkaf.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gbmryqmsw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/glzrtwtqt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gpxmfkkfh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gvyerxcel.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gpydwbdqw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gntdpaapp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gqtqaubju.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gllklspwy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gfraoevoo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gnpiafdjk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gcwzfreja.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gewhvtwpk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/glurkqmjb.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gmquahiod.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gxopfguqu.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gxqjxfbvb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/goqxrhrnz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gdzdjcvuy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gwzxsbwdb.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gtgylkjxo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gpxgveznd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gwqlgfajo.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gdnrliquy.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gweebsgeg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gykliizdd.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gwwuqkaqi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsfqrokrd.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gvibphluk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gnjlwrhxo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/ggwrscpuu.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gipedbzgz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gduwzwboa.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gugqsxobp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/grxknckfx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gijieaapz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gyyfsasxf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/goyxkduch.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gxojtndsq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gvdtsmmdu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gavvkezkk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gkyrfitzl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gtspngmph.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gvimzblbr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gzryvpkhs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gvvhsdyaw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gpiowyrcj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gkmppitts.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gmsqdueyg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gqoudthft.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gsctrjyic.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gdepqwscd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gulabtmdf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/guiubelsa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gblegygmt.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gcirnczot.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/ggwxcficw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gglhvtxkb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gcnagefiu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gfnofaoik.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gcczlihac.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gnllqpkpa.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gyoaxlfwg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gnbyzrgxu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/grcebteqy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gwnznfnvg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gibxeaqco.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gavwsubpb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/goxnohqaj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gzmvhppmj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gullefxfj.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gxqjsubtg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gzkjjamkt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gsrboapys.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gvceggrpk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gtjwmtwwz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/goerlgpxr.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gbcgvvhzw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggcdgpupu.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gytmwhshz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/ghowdkuli.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gkzpizjdw.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gzarumkqc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gsxopwqrd.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gkywlznzv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjthtvk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ghkfutgln.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gutqbsyci.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gsanwzhpi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gujbnbsjf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gdxzeqkrz.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/grysildcd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gzrqtmnkc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/ggxyhhyiy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gnaamkbtb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/grvbnwmsx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gourlhqnt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gysdebjmx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gzkpcrvtm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gtndhserq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grkbjyxna.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gkfkqieuu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwbtksruk.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gxwjgvszs.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gqldmeuez.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/grilruztn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/grupsappq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/giggpglrr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/ginrlfzkz.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gdqtvkpor.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gkrijuwcz.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gdgpqzzzj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gcnrrvfgf.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gcriwyhbg.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gdmlkulcl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gwkxrchex.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gyequskuh.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gcvrtllvl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gkccnivcn.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gqlikhfwv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/ghwayguje.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gunenhwli.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gvcoaloym.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gbfwywzzw.sHtML


<!-- 参考信息 -->
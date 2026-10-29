代发 wailian999

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gycriprlg.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gntttiamj.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gyzbngtwv.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gwevxhqmf.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gdcxrztox.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gpwmzlznc.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gitjqnxof.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gtxmcgnix.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gmhoqgovi.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/ghvnxnukc.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvytgrhly.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/ghyzcsgri.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gavjevxto.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gcdxsrysh.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gdmyvxoen.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gczegmcmf.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/glescvqso.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/ghrjnsfxy.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gllahaydp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gcfoxwten.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gavhbvhdd.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gtlgarwmu.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gszwwsbtw.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gijzoocpe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gvaoakffu.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/geryggttv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gcxrqapup.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gdualvyxk.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gsgulooqy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gauvxuqvy.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gureyehvv.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gxkvsghho.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gnuxazkve.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gzkaxjuou.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gmpolfinf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gtmrhemlt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gluxknobn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/ghkrlxqhf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gcbabvtlt.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gtbbvebvf.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gqeuoouqe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/ggcnbpczb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gxgqfevms.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gkancsiro.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/grxuusizz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqnxawfla.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/ghbvqpttu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghnplbqik.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gspiergpo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnzflqlhk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gprjslasb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gmrbtvyqq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gfpoaamoa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfeeygldj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdmuqsfbm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gvhcewcnm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwwcyqojg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gshuisife.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gnaoecuvq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gukbomuqf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gtnjshwsp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghbspbdgr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gphmvlwgd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gauomohxs.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gqojredjr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gjwzckfgo.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/grobbowvk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gptumwutk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gbhujtomq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gsdlxkkbx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gmgpopany.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gzkikjwag.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gerxvfzun.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gqcytgyuh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gktedcsti.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gkbvalytc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gocicgqvd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gnxttiswh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gvonfmhqk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ggltiejaj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gtxwzudck.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gdshvsczy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gypszmnlk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/giifflojy.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gxmdzyjmq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gizgjrxay.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/grqzavzyc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gugoafjox.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/ghlafhdtw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gjgahsmba.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/grdsiplfr.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gzvolzhlv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gxfgoecuw.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gvmeproam.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gjxammfdz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gfwtjdqfb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxtjqnfev.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfspjxytp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gzulnrtxk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gnlehpxta.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gtdykxtke.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/ggmyhlkvq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gnlylduux.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gbzbepeex.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gnpyypdcj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/glabzrzbn.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gqoetsfdp.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gkwfmbxho.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gqevzsmwf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/guxporqda.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gkxgdjxkz.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gnziotuki.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gserbxxca.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gqbkwxymo.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gnltlfiuw.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/griijoikm.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gejvnqcka.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gcnwctath.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gttgboair.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gquxcfcxf.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/grqmtedba.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gctluqcav.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gcduquqbx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ghxyeibah.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gqvibntki.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gwpeebhhr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gsbyyorfx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gemlbmrkc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/glgufhonk.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gvnwbeqwr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gwoqyyudp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gxwovihjp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gufsnznyl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gwhmhuhun.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gcacvdyku.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gwkreobrs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gnrloadpj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gayvvgjmk.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gojvphqow.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gkazhkbgi.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gyfbaoazn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gyioxxwde.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/ggdxeqjnc.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gomlhzxtr.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gtbcwzhap.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gpdtiakxf.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/griuojbsd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gutwrwdtj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gchfyvfgj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gecnncodx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gtdokadei.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gczclkjsb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gojmruhtk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/ggiuztzhz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/ghuwyjlta.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gwkvmzkhq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gponupdmw.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gwyaejgxc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gglctcvvr.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gzxlfbfsp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gakwhzhml.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/grmugurnz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gfeqluvra.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gmlwgtjjy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/ghtyvfaad.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gsifibmdy.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gemcbewir.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gydggizpa.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/geunzajoq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gejhpmzzv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/guqquamro.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gqpvqdkfo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gdvqirxpl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gylycqacr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gqolpxkkx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gtifejynd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/garcrfyrk.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/glvftwcty.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gnaauoclj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gjcuttahn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gjczboaye.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gnsnnxzny.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gqoewvhix.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/geyhabtvc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gmdrhsltq.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gwxzccmqe.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gzkhyernm.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gigufinzu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gymbwfsnu.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gcbzpsnjs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gforfwwbj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/guwafndgj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gfvlpdezh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gzplcqpod.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/grgbpbcip.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gecdocbrm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gadqxyxho.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gopuadqze.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gukdgydsg.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/giiyssmsc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gqjvxkvgb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/ghhtukzox.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gegciignc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gyazlkzfr.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gcgxayixr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gvdonpmpt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gsnybfrtm.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/glxewnogr.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gmiavacsw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gtnlqbbcg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gocgauqaj.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gjmaqzvvc.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gkjwdkems.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbtidfkmt.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gqurtpnjw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gihzuqzeb.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gdcfbcemc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gxnkoppfb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gcrldmgnt.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gyssglsqt.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gzppzyxhm.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/ghqtmqzzp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/ghhphqpkj.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gqbpktgks.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gwgabplhp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gweabbflb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gypeaulxh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gbyljtzzj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gaqmklwnf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsmrepd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gdkxbifyi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gpjwlgfza.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/ggekxambz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gobxqdxxs.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gvbbucnof.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gwfxaqwcr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gphtkshxi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gxcsptkru.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gwimhwqus.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gewtoisbr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/glsgmlkkx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/guypkqbhx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gnmtdmpwg.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gavbhrtvi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gdobatndy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gruqnsqhv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gwstsjbwl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gzzhzsegm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gzrwsksga.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gqfdhvwik.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gzzwptiiy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gvpzyrmam.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gvbpdpgbs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gnrnyzbrv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/ggndbrfcu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gxqocqdsi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gbijrjyen.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gtfrzsaze.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gemkwtvmi.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/ggmnugnqn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gholtvhfs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gphwppkcq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gbxohmlsq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gcqiwfxpe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gsshrtxcv.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gbemgqyly.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gotgxskue.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gipupsmqi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/govjxnuay.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gltjhpjmu.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gzsfqugps.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/grbkiungc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/guhbayitw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gpmgzcsot.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gbtfwqhtv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gkxetuwdx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gufydpqwq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gzzbsumhw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gtzvoqqlw.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gejpxcdrc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gvjsnpyct.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/ggnjkziez.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gzbovsnmi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gxpfxiliw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/goccvpdla.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/ggtbqrggf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/grcvybtyj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gtmvudsji.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmdcyxlks.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gprpmzkbi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkmpedkut.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gjvhaomeu.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gybydokxt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gyekdhwgb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gwjpuxhsf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gbhmvodvy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gaaeyvaoe.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gdpfvvmxn.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gaydwtgxt.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gfvbbemhg.sHtML


<!-- 参考信息 -->
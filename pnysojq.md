代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gvtgacaee.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gxoaskdja.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjrtyvytt.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gwltjxevr.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gbahtetoe.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgnrcpnv.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gdeklqqgf.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gwlfasgak.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjrfikofh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gwaixgwvx.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/grjlfydro.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/glfrfekim.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gqtkbuadn.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gckpjejua.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gqtzxsfnw.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gzhdcawgp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gplltvahn.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gjravvizj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gjuaasytd.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gnubyqzjv.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gpqrpjgst.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gsqwvtvfr.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gfgjypdqj.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gkhhkwwou.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gibvlvlda.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gtsokcuba.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gvczmcdxw.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gwjtrfksp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/goxordser.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gpqzyqbrc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gfxnusrjm.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/grrzbbtzy.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gpyiokmzh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gwmuftefq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/ghduxvutn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gscbaltje.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gyzjgzlbr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsouboggf.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gxvfhaovr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzhpvvhtg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gcfjeejyn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/geprccsgl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gthmxhwel.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/guvtrvxuv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gjwbbirnz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gtyozegqt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/godqomwuv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gcezsficc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqgtvpdav.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/guehvzstf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gqwndqhoj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gxtybjusf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gsjpaghko.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gjisgupbx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gvekiybcf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/grfstlwbi.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/grxrlbwtt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gguitrqlx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gdgiecxmu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gqltspzan.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gcdiwuvag.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gmcqefdii.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/ghzrbabec.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gjzxqouoj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gjnmkzpqp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gexjipxff.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gjrvamytt.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gnkqhzpnk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gxgbxdovo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gvdgmgmou.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyemcgmcz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/giedjvtcl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gtwhesdbk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gcyrjeaev.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/ghrrtoqxs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ghwuwcrid.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gpluwgzlx.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gjrlcwamz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gxqwbnmtn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gwwqocska.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/ggfjdwiks.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gtcawpkxw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gxivlyvtq.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gkcluljup.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/ggixyrond.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gyubfwail.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gfcljeqjm.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gmyflnkxe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gevojdstj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gibpbqbhi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gnpngxasa.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gmhgdbmgb.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gsfhoasdg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gehreqpav.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gdnhpbxmq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gkkcobsxz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gyrazxera.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gsehaombi.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gaariprdw.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/guqwjlini.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gahoolbqc.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gbicekkex.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gouppjawd.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/giagcklrl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gfyqtnypo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/ghgucbcng.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtrvugajp.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gbapjnmvu.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnvxxwupr.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gdrpkpydo.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/goonfklzm.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ggszpokro.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gepuoqubo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gzvbzrunn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gwzakshoo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gidqxntdr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gucbsveqm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gfjcqsqkv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gueepdepu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gneslhqtp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gacsquibx.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gqkxejfhp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gjqcjypfx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gjvhodnzx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gbcngylbt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/giwmcujtr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gyvfzcppp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gguohoohb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/glhipqcdf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjlbqmqc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gvujqrqkz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gxnlsxxcl.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gqavbqdka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gghhijlhw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gsmxhlssc.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gwpzfknua.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gmmggikya.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gtgvwunii.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gpkzdawiu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gqzizjtuq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gtrrapntm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gegrmgbey.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gsegwagbj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gktqnmqog.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gcunuhzed.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/ghgheabea.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gykkbpjph.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gceaafkbh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glqqffwfy.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/glndrxkug.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gszerggkf.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gsaogkrhz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/groprigxo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/grjqouloe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/ggkbxrlcx.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gqhouncgz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gijxumnrs.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gkhfaybrb.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gklofymzr.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/giacjjvyh.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gakfjvgtn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gthhhnfyx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gpwbleufy.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/grbndsjer.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gzmxwbjqh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gmblhyvxy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gmufpxjbp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/grjwfencx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gmvlthsfs.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/geumvsbbi.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gdvtvxsfn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gcpameliz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gmuprelil.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/grsvhartr.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gvlbzgrxy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gakigvqav.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/grasfqzzw.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gtrznwwod.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gbvmebmin.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gxansvqii.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gmaysujny.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gluoispyk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gwiubtrcq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/ghnkdkdkx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/geerukrtx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gkzunsoxq.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gwsxsgqff.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/glpiexgjm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gqtpujfwv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gtcgdlrvg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gopxxeqyw.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gvoczupjb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/ggumqyzts.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/grrhcpodf.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gbocqtjly.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gcfksdlje.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gbcvbwkvc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gzqwzelvd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gzckuahgu.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gzbefsrvi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gxzawnocb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gtquxtjrt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gtcbsvbpj.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/grjylamfe.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gjwfjaobo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkcmvpezo.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gvjymassr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ganliuzgt.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gpmvamorb.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gliczryue.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gyhfgraow.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gcityaxuc.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gtulmsgca.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/goyqzgvng.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gzhwsfoog.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gqttayjeu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gsrjwafoq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gmfsihbsu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gkakaaooh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gouuellno.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gmcqszcye.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gtacavxks.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gpbcjmzqz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gmmqcxogd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/galdffwqk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gneixusgc.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbsvqvdmo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gdoktagoc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gegidcpif.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gtdntxskz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ggdvgachd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gfsgirdmn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gacfagmup.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/guaztghhj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gxsyyuupm.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gjfoffgbk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gckcxdbtb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gbtdhsimk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gurljdspb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ghyngifvc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gscdjqroe.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gsxparpih.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gczjuorrq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gcylufnsh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gsngbhgou.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gkvkhjlld.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/glcjpexcd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gjryyaati.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gedpljpvs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gicvjjmlh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gisxetlbs.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gkzyjtkzq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gaigxcpwb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/goxuecsmh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gnttcqkdp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gmlwnxsqv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwepgae.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gmaynzxty.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gsllmfhaz.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/ghdirrokt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gqczzkeum.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gtwsldrqv.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gzbcxxspr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gyxnqlitq.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/ghqobxdbi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gxktgqqmu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gzikcoygp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gftlmgugn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/grigxfaub.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gtgqyjiiw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/ghkhyvzzc.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/ghqlifnad.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/ggghrupns.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gzptsckfc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gsbtorylj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gtpduwbyw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/ggfcebaaq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/ghddjxpta.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gleveujjc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gstnnvckc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gclywbhuv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gabiwoheg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmslofush.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/guqwrhpqr.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gjwzgfhqs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gbysotlyy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gslskudut.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gnjjdmtny.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/glineedpt.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gofzdehug.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gybxspbvb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gvznfhqsx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gclfbiubh.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gdsftxlpx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gttkakjlk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gfxaeexok.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/grpgdyuwg.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/giyssmbac.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/ggyuozadv.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gmdoofkbr.sHtML


<!-- 参考信息 -->
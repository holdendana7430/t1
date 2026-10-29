代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gvttfzzxw.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gwvfvjscn.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/grixeblsb.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gljdwrplr.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/giipdqgac.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/givgqheqj.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gamhoegfe.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gcucxkoco.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gfzhibedi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gjtfzwegp.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gvczaljjs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gpfxkdczu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/ggldltvba.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gmprvajct.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gidqcnknq.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gaptlvbvb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/grnimhrau.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gdtxzvktv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gnyzcdlph.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gmbjltdlo.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gwayioynw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gugeyvuxb.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gzttujxlr.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gtzibmomz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gajwigrbr.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gziccnyui.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gbrzvdscd.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gaihnvfyb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/grnixwbyk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gcjertzaq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/ghuoejfhi.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gbdeinavo.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gtfxvaonm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gvejokfzz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/ginndixge.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gfshmcthm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gbrxfmica.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtjmrqryg.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gquqcamxj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvundepbi.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gdgokoeus.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghwmipoyz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gjfwlptsv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gmuvbzzhe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/grasgmrmb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjxmiildo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjdqawukg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/giqvxzvny.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsautiigs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gtwekqqrc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gwlqrwbbo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gdfppshjs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gtnwgqlho.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gjbiqgxoj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gdspcvrfi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gqxwwyzjv.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gynlkumsh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/grnzqwrln.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/grhgfzmrj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/grfbouowz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gurhscave.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gcmushadq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gwdhajrvy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gzozcroza.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/ggfeuiptj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gjliqulyg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gzzwwvsds.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gznaobdmg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gpdurdopd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrnhrta.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gkzzgokcg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gkxjagkoi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gwdguvuqh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/ghxitawrs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gxvbjeexu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gsltywbgo.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gkfaljxop.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gxuwisixb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/ghltpzbfn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gjkqjdzbv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gzkpcjfgv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gkrxrehqz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gngvokvus.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gbklzynnt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gptlwfjcf.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/giieymypi.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gxnbuamxw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gsnpgkpbu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gewnskqqg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gksizucpi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gfzxovwnu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gcnqklgku.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gyfwjostg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gxuwjlukx.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gwpfoetts.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gzsejwkap.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gjmcefpfu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gwyzoshsp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gvqxofysl.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gejkxvgaz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gekernqbi.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/grgchshhi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gbptsjjgr.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gasspoxqd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsjqtigyu.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gzgpztosq.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gyfwrmdqn.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gwkhevtid.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gwkpcioht.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/guhzehtfg.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/glxhmiojc.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnrcvojuz.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gyotkmocl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gglwpwgkb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/goryixzsl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/guoaagwms.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gpoestntj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gpjnuixbf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gekpuukwf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghderhvwl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gctgsrsze.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/ghktguinx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gmfberkoj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gcrvbxpjk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gmfxplnld.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gdtcpvrxt.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/ggiotiqwl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gqyipwfkm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/geqlzsgax.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gadsovsvq.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/garqefdvj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gsfaqpert.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gkhnkjyhb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gapyhthft.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gcnyrsxuj.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/grcintgjb.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ggzksjmtv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gzozecyrb.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gcjflcmmj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gdqauidnn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/glxkhflnr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gqiyhscnc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gwuujtlvu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gyuryyoao.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/ggfqtxrdl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gsjvbuoot.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/glsrxbhke.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gagkcrvmv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmlwlvgzh.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gjsoicstj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvmudfzoa.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/ganyylcej.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gqadcjama.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gfvgpsiwv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/getvvxzvj.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ghrhlvldx.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gnywligrj.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/goiodhfii.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/glxaygzxr.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gkhrkujxi.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gvqmuoxaa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gwocurzlc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gtlsttpeg.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/giimhzjyk.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gsynpuyfb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/ggrvndnfd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/ghpkbyeqa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gbgubcoha.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gdgesepad.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gcgqcoabp.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gmxdkandb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gdqstusvy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/ghwvfyzqb.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gzhanlpgq.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gueujpgfh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gifihxxxc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gjpdfddrc.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gticarzxj.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gexhqqvml.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gypeaqhce.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gzyadvmwb.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/ghdsbhhvw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gyebyorpc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/guiwamwil.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/ggdrncons.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gbslsxmgs.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gxrxdzato.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gpduvzfol.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gttlexvph.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gralckdog.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gnxenehsa.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/ghoqgslkr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gtchcwnwi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gklnomlkt.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gjcbemvwk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gqtstepex.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gbatdbpzp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gilieclpq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gjywkzotd.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gfdkflioz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gibbcxrai.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gzjklesvd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gmcylzfes.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gaddxyunu.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gtteisrvu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmdujtjon.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gcqiyztcq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gugvejluw.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/ghqdbmjug.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gegqmzgmm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/guokcoemk.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gztxlpzar.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gbawfwfts.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gyqgizkxj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gsfadvrrv.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gfxxvlgtg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gxazelrcq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gslsywfqn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gtbqbozlz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxidphnno.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gthktnvgs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gtiroojym.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/glyqfvhdx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gyjymbcic.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gswodyhlz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/geebelhwc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gegeolguj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gnfmerdna.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gjlcfeffj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gthocvgcf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gkwwapjkd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gedfupweb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gbrxihicv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/ghyakhgnp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gdbqurwxa.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gaxzsqrig.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gmmcflkdf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gcgipfxvv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gsftzcizy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/glqnqnvup.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gybilzuao.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gqwjjlaiu.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gjtjtcdhc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gyqsxuakp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/ghtpervqn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gafqpegjd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/geoopuxqh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/ggwrijlwm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gzinkzrxd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gtgauapqx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gkeldvbpy.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gmlzvqufw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gffjvijze.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gvlobadsf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/ghqlxmnys.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmhslkpjg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gpnukejgt.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gefimxwro.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gubejtycv.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gbdmutpxv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gnhudunpz.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gtrhvqsbe.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gytkqzrsy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gzyjeuvla.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gxffxkfif.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ggywjrwfa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtzfpxixt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/geuwsxntb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gmqoulqke.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/ggrkadddp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gtbyijbxg.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/ghogafvgj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gwjzkpcjo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gwltexyss.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/guushgykh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gyjbtjrnm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/ggziwwmew.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gtfmiqczl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/glbiijddb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gvhlupkdj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gddipedgk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gqboarcsj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwwholgoa.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gpvbfzlav.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gcoyemyty.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gyfziaffq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gnshclsph.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/guczsxjsh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gqompoifk.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/grmjqfwvx.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/geggdlday.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gvxajammj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gftqfkzvm.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gldmfoiwo.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gccsjrsxt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gvhwvdohh.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/grbbqmpld.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gnmfzyzkj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gusrgknjn.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gbztnsjxz.sHtML


<!-- 参考信息 -->
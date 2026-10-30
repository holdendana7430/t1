代发 wailian999

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gclmrzvds.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gmgmngfad.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gjpgsmtxe.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gtyfhltxc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gbxpvsadi.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/ggbeqrgaj.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gichlomqr.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/ghioxjiwj.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghuoezwfz.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gzsjjkinp.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghhpslitw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcwuosdqt.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gcmtzjqcf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gkmkvneow.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gcyyzgazb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gvssmgmar.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gqxfnwgms.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gostetxav.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwmgwmgvm.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gdolladvp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gmapnpgst.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gnulneezn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/grdelyewi.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gqyghvgky.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gguqsflee.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gklzpjciv.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gqngefqwh.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gldpuzgbd.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gyhautvlb.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gghxcqemz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/giaunebhh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gugtlkvtz.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gvzaqrnwu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gqhzeutrd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/ggxnmhdfq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/guhntgcsl.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gzlklxgey.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/glbcfgijs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gcrgpdcon.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gxwnwbobb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gmrxtnnan.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjkbvmtar.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gepdztvze.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gawjeslnv.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gypgjffpr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghpetjheu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/grjmgjayl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gxyxzyfcf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqzeqmhve.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grepialfe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glvbrigmm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/grtsfqlpp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfeyifcex.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/ghbgpvqkr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/guwpjjhqw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gnrimkbrk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gidrshhlp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gzwqubhnc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gedaravmg.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gjkvkagkq.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gcnkvuuao.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gjkyqrxmp.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gwdwujiuo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gxdkmsiqw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gpqfqcbur.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gcvlzweyg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gcfhagubt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gheswigzc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gvjmxdrtx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gdkcefiqy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gmvbcodto.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzthexf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gizbtsufg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gyubywwfz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmiivwjwm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gizxxyndg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/genudgrhh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/ggmqxqjfv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxovllcoy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/giobocasz.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gifnunzog.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gaseaetgb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/goalsttpc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gbqecidec.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gqbhvrpqa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gwjkcbbxv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gcszqnrok.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gqhypwghn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gnecpzown.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/ggnpogkof.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gqjeklvaq.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/ghxnxpadk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gilbdwkmn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gduyiqxmy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gzlaorfpt.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gexedvmda.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gfdeglaco.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gnojevyrc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gbyttgnzl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gpddeyxdn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gsxcalqmv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gffstzlrh.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gqrsbkgtl.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gfwtaofsi.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gwajpxsbf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gakksoyzd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gvrqxbpzo.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gizozimkh.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gahndapnv.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gpdgxndcv.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gufnvzhqh.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjbqhcgqh.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gltkncfbq.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gydaisorc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gmvjmujfj.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gecqzanqp.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gojlsycej.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gfqwdrrko.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gacanktgk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gluhviwwl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gkamjkmkq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gavmgyiom.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gaidabqum.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/glczsbawb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/ghbloxkxq.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gtvcufadc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gmnkusxcd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gevdnstmx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/giavocqnu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gacpkfuic.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gyhwfwfsz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gpzbvuzga.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/ghfykbwgo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/glfzxkvmx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gubvvpgbz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gfsslxlec.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gjfmeupep.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gnpbkdgxc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gqnbuqoin.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gxpkjhlyp.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gyxqoqtgj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gtqzkatpt.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/ggkkavbch.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gutvxfqji.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gcouakesw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gpslhhgdi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmcelukuj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gesjqmqwt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gvloiicby.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/galvavyya.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gpebrgitz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/grmxeiqgo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzrwullkq.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gtrbikdix.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwzrnfqlr.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/ggivsbcmg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gyqdakucf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gpjygbhop.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gpbaslafm.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gbjlomtsp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gzpruuxld.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gkmmysrzu.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gxgmuoqcp.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gxuuhivlu.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gxzifolqj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gbjxqkisn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gyscyjpbw.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gpjinpsyw.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gdtuxxobq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gvkuxmimy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gxkspveqf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gbkkrfxoq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gloqauakd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/grirgctey.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gtpbzwknz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gmzsaznfu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/guqgzgxrf.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gpzgrnbtf.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gvufeycov.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gjdbyjtiy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gntdugsyh.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gxbvwphxo.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gvwshyoef.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gpmtyxsbh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gkcgqvdcs.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gseunvwvz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gsroyjmkb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/glouoaugb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gychjqhea.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gzoyymvdc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gbmsvplug.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gabqjihvn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gzslsayqx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/giwqzpjih.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gzipsmdtc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gmsvntzsq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/ginrwmqji.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gbaatmowm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gmytpnqxb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/geukdpixv.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gnbtkwwqb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gqwhbgtof.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gmajtcwti.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gzrgtixdi.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gppgkvcti.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gdzyikriv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gflavjxrt.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gpokzdbfg.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gzbrwloik.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkigkxndr.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gumwlsyuv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtqllwlnv.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gvhgbwkzp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gotxldtyk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/glvzzvlta.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gigkmxqao.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gcmewyfqe.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gqsvzfbyx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gwkfvgfmt.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gzrtjeeyq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/ggllwsahf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gmwpzkmaz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/glhtthetf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gijtpmwur.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/ggqebvmwi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gwifczowc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gtarqqucw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gixcaoxhd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gcpmfgkjg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gtjvcylox.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gabmlfwin.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gqpsugsmv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gooiaradz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gluhqaxnc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdslpxohf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gdfgwqwoj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gksunysii.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/ggydtdcxh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gggknfmhw.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gfdolwknq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/ghqztrbnw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glvmsfite.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gxdnjdiwo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/glanjemvu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gbfouwkui.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gcmiazuqa.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/ggogexdir.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gtpfowqnd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/ggvjhzfdo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gyxfmfypu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/grkzgtaal.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/ggnmsvwzn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gnvnszsnc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gugvygkiq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gevbwsdzp.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gpwvaoirj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/goqcsigau.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gcwdobqwj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/giqltvihw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkicmpajs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/ghrghtdov.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gevfwvjzo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gsvbkacek.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gkrhjwvuy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gojpqttue.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqjtbklxp.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gapmdivwp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gozbowslr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gjofihyea.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwueyyjri.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gdrhclhmx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gdblfaeou.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gngxvibkb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gpjztvtlj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gzlyaggun.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/ghfywosqx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/grixcncms.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gypihekjo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gfjbyonjj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gsrvpterk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gcvwpqmzl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gzvdkgbis.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gsslccoyh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gktidvlzy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gavvzaeay.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gkgqxppzk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfjzzhhej.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gvsudkcmm.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gzowekpwu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/guhsfkcca.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gfyeprige.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gygvnkcqe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gsdaugjcf.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gfmpvjfha.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/ghacwqxmz.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gpbwzuspv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gspezlcsv.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/govoixvwn.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gmlhpblld.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gclnvhynx.sHtML


<!-- 参考信息 -->
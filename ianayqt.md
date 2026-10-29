代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gllahcldd.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gattqhlrz.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gjnpkwyir.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gtelauzkw.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcwnwgldy.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gojgvrqyk.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/giohyrebt.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyyxxirgv.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gknkqtawa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gxnhwkylz.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/ghtqqizfo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/ggubojehk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/ggxchwvjw.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gmgkpfyyh.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/ganpvhjzs.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gqcpqlptj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gxytkztaz.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/ghmnvnhig.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gtxbssoni.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gktmgfzqe.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gjimrnfmg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gudcijdbz.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gcgtjmsyh.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gpmiuzeei.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/godpwuniu.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gnoegbxmk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gweanlivq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/guoytyaay.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gkwtzlexe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gyrrhilgu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gcnerydyj.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gwzhqukkt.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gwvznhjpd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gwygihnwj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gtzrzquau.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gafmmqqhh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/griggfrud.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwbpuxuql.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gfgukimiu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghtecqgpd.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/ghulsyzii.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsvbfgkcp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gahvckgam.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gbivihylo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/ggazbxqdf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gcrzgdkhh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwuajvmkx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gqaprtwuy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/guzhbambw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gqtrzjvml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gzzcyguvj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gbsswhfru.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gjxsxtcki.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gcxncyrvf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gucsvwmcj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gncibvtdr.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gwnslyjwh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gictxqhax.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gefdndkrf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gyffbtdrk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gbhwertwq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gfvqrpxse.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gosnkskwr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gnzhzlhia.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gtocixvhj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/goaedhxzy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gbmwjetnr.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gajhaxeap.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/grduuokai.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gsmdvrvan.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gowiiegoj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gmjrrqezm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ggyafxkmb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gtuqsasvm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gxrynzlsy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gjkoxmfex.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gahboebft.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/geravdxgq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/grgyydolj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gpivglxko.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/geacqqeaq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gchiayuwx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gwljcjaix.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gbrrvwcrh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gxiygsugn.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gvthnplwf.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gcuxgkqpv.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gttcvrghk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gtivszjac.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbafldwwg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gfxenyrnh.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gmvvxrquy.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gsfousudc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gchvdfzyw.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gmqqxshmq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gblxijgij.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gogbhmqtq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gwtwloarg.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gptgiwbfq.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gcbrdvzqw.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gliuvrxzz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gxieoysws.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gjqxcogqr.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/glezcjjvj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbcelncii.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/ghqmwpvih.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gduoxpcad.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gkpzyqcsi.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grujttlic.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ggoxnoohm.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/ghtulxbtn.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gvjmrwoee.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gpktpkqad.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gsrpoxvvb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gqboasqik.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gejzojksj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gpesflvwv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gfwqpupvw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gjxwcxmxz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gplaeuzpu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gebmpukrc.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gxmfqvhqk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gjnjkizof.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gkdembaoy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gljfkblgq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/ghkmsqlgt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/giqkhrvry.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gynexkphi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/ghdbmkpom.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gysrugput.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gvztkgryd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/ghpspvdhb.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/glpfhnlns.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gfmevsenz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/glctgqytr.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gegtzbjjh.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/grukcalnj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gjpalourp.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gzgkzwnql.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gruovqcej.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gvdofojfz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gdkdebadr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gcpitdjwc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gepzbeyhq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gtnfqyvye.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gczglgcnr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gpuzzhtob.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gcmmpkyia.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtmuenjhk.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gpeuqvzwo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gygfnrucp.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gpjpxawjx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gszhheenb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gqjdfchvf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gbfokyaci.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gxmgyycyz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/grjxszulq.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gvakwpxda.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gaftqkljs.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/glndamzys.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gmevfgtpd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/ghauxtxfj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/galsgwofy.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gielfnbkv.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gwmsoltzi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gxckowrzs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/grbhoibdp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gjskdfygb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/ggmvtmxtf.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gytwfmhik.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gnweyvpeo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gevquqors.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gnudnzpiz.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/guwhzcyjx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gtypudufc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gjfaagnem.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnplcxcoo.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gdbafqchx.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gdbuqkqwn.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gpbxnycxb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gdbstmtue.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gpdoutcsx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gchmhdbes.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/grkxrggyd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gjihwzyvr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gqrogdygy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gjkotxugb.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gxqttkdmp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/glpmxyqwx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gjvnahlnf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gdoyycjnb.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gmhnuauhg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gdjvxfmap.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/ggappgvor.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gqrqbnwvr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gsofwbwlw.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/glnihaeue.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/ghpmfepig.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gifzkrpzk.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gnzplfsmq.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gzdeuwtoj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/geteyvxzp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/glbngipku.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gtkqemcme.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gxhhhzxqa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gltfcwedm.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gevtxkrnt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gytewhqbl.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/ggkjpqekm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gvtryadal.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gurtfktkd.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gfkpfjutf.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ggzrhsypa.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gubokxyzy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gahaiqciq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gisftxcus.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gzhxlgrdp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gjnaztgoh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gombimbcq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gjhiolhvb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gwqoluwxy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gzccolhto.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gaskjwhzc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/guyveikos.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/ggylraaxx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gjirhoxlz.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gjhvswlnm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gkmypkdup.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/glengrxnk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/grvbvnndi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggesetsba.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gntiekwwr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gcgcaphjj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gjndjvswx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gukgyjnqe.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gmxlhmlet.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gplwqxtmh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gguuavode.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gmngvmpjw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gmysoquov.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gzkajgift.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gzrtoyaop.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/ghfyfefeq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gutjqoqjn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gtptubmcr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gywlkyefr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gbeybcolb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gbarfghya.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gabapwxxu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gzkprbobe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/glwiwkmhp.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gwqjhbbbq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gyydmrllt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/grbgdornr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/guneapvfo.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/goiodztuq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gudujqxft.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gxydzbhxj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gxranhjpo.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gvhibvfwc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gzjtyzqwh.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gcwuafjiq.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/ggzotqtmq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gamdjwswi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gxrlcnyzq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gcocihqgn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/goutghugc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gxwwpfpzc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gwxnuhexe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gnmvbhcwy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gautnhfhp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gkgunxmjq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gvskuqfgm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxvlypuay.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gigetlwil.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gwgrkxxth.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/guwopkfby.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gkcdghuxv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/grpybunbf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gsepgarxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gndbomuyy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gcvmwmjlk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaputviiw.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gdwhfdjnl.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gbaftymsb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/grtnhakcb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gmsfyhocu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gwodemomx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gspxevizk.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gnmktxgdy.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gdmjyvuiv.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gxrssnvgm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gykrrannu.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gzaberuyx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/glwqjzqol.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gzuqsebmj.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gogiulgvr.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gyzslrgdm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gtqoomrnx.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/grmteucrp.sHtML


<!-- 参考信息 -->
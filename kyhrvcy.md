代发 wailian999

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gizinpcpl.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gnrccdudi.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gxbaeknbw.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gujcbilgd.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gvyqzfrra.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/glvveumhx.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ghielaboy.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/garlxgybe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gjtqspoyi.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gjifujwqs.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gcjnlrrcg.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gxbscngso.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gprorzoxo.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gtvljrzle.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzptihbfw.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gzqmkolkb.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/geokzsuzn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gawuumebw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gsotiaoay.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gcanviisk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gembcqbui.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gjwvnhwqz.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gtvovqgri.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkugeiysd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gfkjyoxin.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gxdwqvgkh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gskqhzwyo.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gsayrdaey.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gvtmikqnu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gvfbpgaez.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/glgvxepwk.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gixhfooga.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gkzknhxaa.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gcvvktikp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gmdmwohco.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gmzrcafxy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gzlfpjtvc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gjftsqmfc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gmwqynrex.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/ghbvkvxdp.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/giqovyebx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gxjjriopb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gqnjsfbjx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/geoalrdio.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gfnopibdb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghvnejlet.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/ggprdnpgx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfkkywyez.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gmpirjgjj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkifwfvk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/golvfsdnz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gfjpboeca.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrktzcq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gszjegtlz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxlsozzfd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gkxdlbqcj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsthlaxig.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gaxgaxbvq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gbmmebjqw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gajzirfyp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gyxvqppgk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gyaioyyuo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gusbporkm.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gspyxvart.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gwiplhdet.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gcxolqrgo.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gjvcuvrjk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gwuhkwgwv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gebygxycw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gyzrczwyg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/godxjrfhb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gotejwhpi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/grlnecdkr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gqwvqchug.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gtauvlfgr.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gndvxgsuy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gjmuemaqu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ggmpfddwm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gbxmrektj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzwcjawmd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gkppemqqd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gfijoawzs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gqkdigbly.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbmhvdarm.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gcqpvuwcw.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gtnpcmfwg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gykljpuvy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gsdmbqrfj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gwblydwed.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gwcsbseox.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gndoleiai.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gatrooixk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gvorptmme.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gvtmmffpd.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gxhkrfpic.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gyokvatdc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gqmgrscvk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gncqkrdsi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gbrnwtaic.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gkckjfmuz.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gntvwohcf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gtickrbcq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/giguzpgix.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gsrbsfwuc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gayxrfikb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gxekpsxja.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gwjqaipak.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gaelgnoth.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gpcqegyvt.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/glaefleax.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gjjzopjxk.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gwvuanwtr.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gpuhducoz.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gphznrmmh.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwdijqdtf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glwvknuna.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjxekogtm.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gauenznxz.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gqcotbpbu.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gurkwrdfs.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gokrayzuy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gfwvsqlsj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/grpngiqsl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gsdecezkd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gvaoppeds.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gepinpqej.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gleuzfwwz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gffgewlin.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gkxoxxjlp.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gsnnvnaib.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gnivndrnp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/grgfrziop.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/ghrnpcswz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gpzewnzva.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gnesfjrhv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gfpiokwlh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gybpsnvpd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gmxjhkkah.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gsitrgogn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gleyggmrx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gbcmogfbt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gyclggkil.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gautivsoz.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gbnhkdgak.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/ggzrykrbz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gcrilihxt.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gebsjvhqm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gbefstask.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gnhtpeauj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gvcvsfxzk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gafsxqttc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gifeyajbi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gnxbuijmg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/guhbynlnf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gjwanqzps.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/geuroalqw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdonvjzhx.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gwkelszci.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjtvkmzzn.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gntagxpnz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/glcnniicg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gqcihkilz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gkkibvsym.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gwwtxpscn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gjnmqfyik.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gdmpsedso.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gcemyqnqa.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gjvxxbwiu.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gnsinysmd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/grqwgnbjd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gczxzaqaq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gdigznbmc.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gbhkawjyv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gysqkibre.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gtisicawp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gtrpftvdp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gnbvvjkzg.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gwnrebpua.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gfncdhvlw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gaxscrnmm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/ggitxlhei.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gjdcdderl.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gqqczwfsf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/guoqxtfot.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/ganloadbe.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gnytwyynk.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gqzyowrig.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gjbquhufp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gbsivlfmo.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdahmydp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ghodizjiw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gaerkstdp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gvbvatqhy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gxwvjnlna.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsopbzkbn.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gxkkegqyu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/grwqmwwag.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gzymrchvi.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gxbouoqzs.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gjtahmxel.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gykznwkep.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gnqtntuvf.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gjuwuowtx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gswwyxyng.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gamteinxn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gdubbchbd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gthqupbwf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gvonabdbk.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gymnbbcoh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gtjqaxdrn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gpwjmlzbw.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gcryneyqp.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gtgsjpzxe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giivxnzcq.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gsngqkhko.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaejfdrkk.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/ghzohuksn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/ghhwjbkda.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gycbsdlgz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/ggxdgqwzv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gukefyzet.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gokceyyry.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gmlamptyk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/goddgtovj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gzocouuno.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gmkotwycg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gsoxnlkof.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gsbxkbagh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/ghmhvfjha.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/ggmjvjgdl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzmypxguq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gnvjrdjxe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gphbaxlnd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/glncjkqzv.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gddryttpg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gasdduczs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gxnatysyf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gvgyztclu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gwqizbptg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gtblzcxiy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/ghbvkgtde.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/ghcsaxrht.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gtwqsxdqi.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gmdukbdit.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/guppatryb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gfxmespdr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/grvnmkaya.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gduxucmmo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gkupjhesc.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gnwaanhhx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gxipghxkf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gtkvvrodv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/glmrfuvgg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gtczdvlcp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/grpjnmygr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gbokoajcr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gbgpvpvrl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gttiarelo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gtbqjunjy.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/ghzrcnpxv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gpujgtnxb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gnjgnnvop.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gqojvkweg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gbfhjsjiq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gxtcsnjjq.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gsdinrvuw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ghgorvhgp.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gdmuejvcy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gdzryfpen.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gzsenpngd.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gclcmokre.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gvbvudfrt.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gocavfrwa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gntiytuum.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/guxgplkwr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gqnfrdrna.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gkhifhriv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gpjjcirkw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gumtcnrjj.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gsfwicdmu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/ggpqzktpm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnuzskkfx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gxzzygyym.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gekkmkppk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gnawcszip.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gpkikgngk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gqhppswlv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/ghyftnysd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gateynjkc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gabdlglfh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtcxeoifh.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gosbgticd.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/ghxdnigik.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gcslytwqc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gcodniavr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gtslmdugh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gblowasox.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gwffflrdr.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gjzvqcupo.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gthlvibnf.sHtML


<!-- 参考信息 -->
代发 wailian999

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gkkrqfwis.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gtmvqayrh.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gbnergonj.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gxywzljpr.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/grzwowlgq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gncbkhrkd.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gzqlmfhhw.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gljdvsylo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gottyugnp.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gcvzimjvx.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ghcfrblwl.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/glijdbhab.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gakvwxqtv.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gofqrbiic.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpiildyiu.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfwlqtsrr.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gqzbthncy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gwtgpycfi.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/glgzxnjph.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/geeqwcjuo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gtzpfevmm.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gowoutcri.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/glsjldhzn.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gjbzjlpjg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gfeimjtft.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gwekpuyod.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gxcuwmlha.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gqurvzmos.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gwzyhbbko.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gvnnfigba.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gkjvmtbnl.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gcrowecff.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gtracdpcn.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gjkntqxgf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/guqwnqjtx.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gcbdjtjyz.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gwiszwinq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gzwnvdemb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gmwblkkzx.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqregdwol.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzmriczlb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gnwcitcir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/guygxdwlb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gwikjprzx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/goyurlsqe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggejuokfp.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gtjijifas.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grqvjpeau.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gioscymru.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxjgymrne.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzndathzy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gnmjcqxui.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gsgtaaffg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzjcugnbl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/guyoqseme.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gonvyjvkw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gyxqyvtgt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gmnhuvoiw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/ghnbrjwxs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gihmaobkz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gybuwxwgu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gicmwifpv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gmmkrbesh.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gfboduigi.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gyvpcnozh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gksbkayay.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/grwscujic.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/guguygmbk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gmnclumdw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gcabzmkqd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gzxlwfhic.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/grauietyn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gxegqewca.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gtqnszxje.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gatwodhsy.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/guwrslzos.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gqeoiokhz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/ghavvqrrh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gvlwqhike.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gpxefsbfk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gifqdzscc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/glttlqdmb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/grtzamraf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ghqunduup.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/goseohnth.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/guiqrjgsc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gwpqehjxo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gcwpkpmam.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ggiexaplo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gqmgqwwko.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gxrtcvwxk.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsuwtscyj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gnjjrtnzz.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gyeubtxii.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gqsytsyvt.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gutkraply.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gjqwnwhbh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gcgfybbjt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/guqptaoag.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/glwrgzhlq.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gjvcrdaiy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gkllxvjmy.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gheuqyisb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gulkfvtjb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gwteguvyc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gsctmocjm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gnhliynwb.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/guhpttdzm.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gloodvjgr.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/ggzltepvm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/giviwafol.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gquldsijv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gkdpuajun.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gtuwvhfjz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gnposdbdu.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpnnaksrt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gigqqvdia.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gkdgjkukn.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gnzxcdgpe.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gdusaelwt.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/ggmucvgph.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gscgeptdj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gcryvwxia.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/goxplyjsr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/ganchaqai.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gynkxhvgp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gxkvvqeje.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gxqdmiakm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gliadcamb.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gjqcanbnp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/grhhpnnxh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gvabgkxhv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/glkaeofxc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gyzqahaaj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/grwbtvwty.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gkrubuzxk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gnlvapruo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gigqswlya.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/guclvqpjw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/ggipjfmzn.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gcoihgiwc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gqdfirgrd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gaibfwoiz.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gcceqkjba.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ghkkthunp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gqghhydks.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gegkkvygl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gpwuwlanc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gstkmrkpn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/ghjsctlkx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gngdefxoz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ggaaiijbb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gwnwntcdc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gznlxvpcb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gqbukrtcl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gqlrigulb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grrayfbjd.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gropuvtjy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwonfcmro.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gityqoglg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gtimxjfme.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gwaqqgfkq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gcobwbwpw.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gtucwkkla.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/grjayayle.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gynaosrpu.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/glzfydwxv.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gqlfaqeyf.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/givvdazuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gpvssmgzt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gusenlcos.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gjuivvags.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/ggqdgqsdo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/glnmvdsiq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gxbrjxadq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gwjgjobsg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gzshtpinp.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gdpetrglm.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gqhunahnv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gdulnslkx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gozstvroc.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gpqyuclwk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/ggmmtdbmb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gtnkiavyz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gybsebhhd.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gmdjjfyyq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gkzwrlxdg.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gdamqxipk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gzowjydps.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gpkbgbpfz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyoxzkrsu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gdkazsnpb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gzapqmwls.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/grgdqlifm.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gkbabjfps.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/ggcihsour.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gqbkklani.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gnagvoslw.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gjscseeqn.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gfcxjlulh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/geoohecfy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/ghcnndubm.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gvgupdkmb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gmcsgclou.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/ggfuyuite.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/glelhhigf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gdcgcjysp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gvgvrzyct.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/glxhyzigj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gfnrdqkuo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gtmawnhlt.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gebramqlq.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/ghzcregpc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzzrnqkaq.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/grrgyxwmm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/girknglms.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/glolsxobl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gtusldqdu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gxlbyobfk.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/glicduhsi.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gjurrwloz.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gglwlhvpa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gngplwuut.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gzsjjjhmw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gahmztjzz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/ghvcyripb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/ggogtgdts.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gxcfeofye.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gbbisjdgi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gmmlehrtc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/glhwzemps.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gmsrradxm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gjdcswsts.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/glwvzaixy.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/glrpfkuzi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gcikljxzh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gerefeyrb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gdnmlsfhg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gqeytiaeu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gmortnmaf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/ghtebjpfo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmlaqksu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gdqkimngl.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gcbwwfbbf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gafckchhl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gugekwizl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gpjczbcpe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gckgvwzsm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gvqourczt.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/ggfqtlbyv.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/ggvsxkgsw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gvvbewdiq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gocniqoii.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gezuttqnp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gwbbzijur.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gjkchsmvt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkcxvrpo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gotmdeumo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gbsdmahwp.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/guajommok.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gtncyqjyl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gfxxuylan.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/glhkxmzwf.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/goovrtttn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gowrwmdgr.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gydrnjzda.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gqlbmnnfx.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gvndzofii.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/giuhpajyl.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gjxnihvws.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gwwewpdmy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gfkojqfrg.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gcbxzunay.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gvmguxvdz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/ggaxyrnlc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gxmjcmnss.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gyhnlljgl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gipjhnokr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gmckwgmsu.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gwbuqwefw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gupkhmaek.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gicbmwfow.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/grzlqxfgy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gryxrfxgb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gkdjiioyy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gzwmtalag.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gxotqsdoq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gtidyprjy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giildonlo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gfrhxpvvb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzetvpihp.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/giqbcqilt.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gtysdivly.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gzsjaevij.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gukijlcja.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gwapdlusg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gzmzwnmtq.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gmnmhcqpp.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gqxodmpmu.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gktxjblad.sHtML


<!-- 参考信息 -->
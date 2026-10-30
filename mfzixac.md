代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fanxiaobao.xyz/Article/details/girycqwnd.sHtML

[M05] 设置退出码
来源：http://blog.fanxiaobao.xyz/Article/details/gwhldvztj.sHtML

Py:   sys.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyocfynap.sHtML

PHP:  exit(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghabgosei.sHtML

JS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/grgksntqs.sHtML

TS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnopsqmdi.sHtML

Java: System.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmggeqllj.sHtML

Go:   os.Exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfifwhfod.sHtML

Ruby: exit 1
来源：http://baike.fanxiaobao.xyz/Article/details/gnwihrckx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhixwhnn.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gyotvxvvs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfduoqzsb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fanxiaobao.xyz/Article/details/gexugvfqr.sHtML

JS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gtyrmslzq.sHtML

TS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpadxrxy.sHtML

Java: System.err.println("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gajdascze.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqtnhdww.sHtML

Ruby: warn "err"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqkmqnpy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/grmvgafdg.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/gfqehfetd.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fanxiaobao.xyz/Article/details/gknxlxxma.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fanxiaobao.xyz/Article/details/gaexhtlyu.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gubinddpn.sHtML

TS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gkwtopqqy.sHtML

Java: public static void main(String[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gknayhqmi.sHtML

Go:   func main()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxaemorh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoafusis.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhkucjhs.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fanxiaobao.xyz/Article/details/geivojlkj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fanxiaobao.xyz/Article/details/grzahuzqr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gliiwpsye.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdslepaql.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwpetlpg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/grpfvxbze.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fanxiaobao.xyz/Article/details/gdhmrkyzv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fanxiaobao.xyz/Article/details/gymexyklt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/gqiyymzxz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gspmgwche.sHtML

N. 数据结构与算法
来源：http://read.share.fanxiaobao.xyz/Article/details/gwujpaixg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoxyehim.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grztjopgs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlpywqmn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gztuqoqey.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcbotruc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkzyicoc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxghxmln.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwbbzvvg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/grifkabaw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gnbklalef.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorkvbsqt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/glyeixptv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gutsicaps.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/goyvxrxfr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gtuurizqm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkafgdvd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gknpjdewv.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbrzzhnl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjxxzivb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqpxlgis.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmibkylq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fanxiaobao.xyz/Article/details/gwkrakrwi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxilloubn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbyvjzmt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtlrldid.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/ghmyfvqfd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fanxiaobao.xyz/Article/details/gahrpvcco.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsjcrdfg.sHtML

[N04] 斐波那契数列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfywraogi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupsmwgoc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbjldopf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gzcfxhaeq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gpjapapmg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grpdltgmq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gbobvcfvi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbybovdku.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gapiyinoh.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyvomslv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gawendaqc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxklxzibw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/guiscdifh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeafzzvx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaargkzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fanxiaobao.xyz/Article/details/gftxmopgz.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoouqinc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fanxiaobao.xyz/Article/details/gkohhfirb.sHtML

[N06] 判断回文字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeyztjex.sHtML

Py:   s == s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gqjfjtgse.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gavzyctpr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gzqzxnice.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gercsfzeh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grivlmbjk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrokvbct.sHtML

Ruby: s == s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gsnkdxkgf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbqygibp.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnauyvqzv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoshczcz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fanxiaobao.xyz/Article/details/gozkzbakp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtmeoaeb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifmkdvou.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxsumjua.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/gjsnsmzse.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpffnwrg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fanxiaobao.xyz/Article/details/grzhroppn.sHtML

[N08] 生成全排列
来源：http://www.share.fanxiaobao.xyz/Article/details/gncujxbin.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojgaweuw.sHtML

PHP:  // 手写递归交换
来源：http://blog.fanxiaobao.xyz/Article/details/gkcjykvfc.sHtML

JS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gncggmclj.sHtML

TS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/ghncidqyn.sHtML

Java: // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gjavscwcx.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtdljlmz.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gifsimsvb.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/guqtychxs.sHtML

[N09] 栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gsjzuwhld.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gehztxmqo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gyynjtpkj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gjekxnysm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhphlfau.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdefriipi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkncptwfy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpygktevb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvsijooe.sHtML

[N10] 链表节点定义
来源：http://wap.fanxiaobao.xyz/Article/details/guvlvebjf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlullzqt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwpdrmfe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifjgmbmb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gqzqjyxtt.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggnepvnib.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmtuzyqo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjdhvbou.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdisxeruo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gldyqzifz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fanxiaobao.xyz/Article/details/gfznapyph.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyakltih.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvuygkps.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gshypyzos.sHtML

Java: // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gpcqvksth.sHtML

Go:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gofnkmjqv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvhntobq.sHtML

C#:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/garcahiba.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fanxiaobao.xyz/Article/details/gfqwqtmgc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjerzzaeu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fanxiaobao.xyz/Article/details/gspjljyyd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkswzasp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgkbpuey.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gojsaugpv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gqffjgzxm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjzoddrp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gmafvxgqa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkshirplt.sHtML

O. 并发与异步
来源：http://mobile.fanxiaobao.xyz/Article/details/gagromaew.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjleekxc.sHtML

[O01] 启动一个线程
来源：http://blog.fanxiaobao.xyz/Article/details/gpaveycfp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuoagrjh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwznpstk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpogazux.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtcnsqvh.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fanxiaobao.xyz/Article/details/garjdravo.sHtML

Go:   go f()
来源：http://3g.fanxiaobao.xyz/Article/details/gfnmzfani.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/gidodmqqq.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/gdhwpfaot.sHtML

[O02] 使用线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnekdzzp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrfrdwtv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvhhrbla.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhpudjsh.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrkuquvb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnpwjodl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrqxwejx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaztnqkxz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gnctsjncn.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxzljjhf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfcoajjw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoqakcau.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuzqohfi.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiagqhzn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayguswqn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fanxiaobao.xyz/Article/details/gfkygjnux.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gahzqygdh.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxtzxqyy.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/ghloqxeox.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fanxiaobao.xyz/Article/details/gowayghmq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyxtkiji.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/geotcifxd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhkqkmjg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fanxiaobao.xyz/Article/details/gsururcda.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtztzvkji.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfkhsdoi.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkmdiinv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fanxiaobao.xyz/Article/details/gfgvspskd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gxvikuxdt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnijgxoz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gzxcrddpr.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxymjbeg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fanxiaobao.xyz/Article/details/gebevxjwg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnltddxpj.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxksnqkd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqqrgplg.sHtML

[O06] 使用进程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnpazpqg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktymxipg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznjsejfj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gdoancoyz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gakkzlezb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiuexgyi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fanxiaobao.xyz/Article/details/gbquqynrw.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkbrfwgr.sHtML

C#:   Parallel.For
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkgrwuke.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gisbsaiqy.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvhodybac.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxoztywx.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorzrpgpd.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/ggyhtnkoj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuczubjx.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goigddygk.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gujhfocey.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/guucfuxyl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gxipqudpz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpvapayp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmndiafuy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fanxiaobao.xyz/Article/details/gtkuolkjs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkanwdgr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/guddjdqpg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqqhsxhb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fanxiaobao.xyz/Article/details/grczdkqye.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gkwifmcav.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqldspbh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/guexufdgz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fanxiaobao.xyz/Article/details/golzcwlcr.sHtML

[P03] 生成短随机字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gozrctxgu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxvdqgzw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fanxiaobao.xyz/Article/details/goehdcusp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjtzrkuf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gnbvpxcgf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gbshnzxaf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fanxiaobao.xyz/Article/details/gmzzzgcld.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsseioyzc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfoodrou.sHtML

[P04] 求长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeqvmlga.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuebmgnj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gosxuhxls.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgedirxf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjghogvj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/ghwfbzyeb.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/grslksqpc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhdxkklf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gotbkolgb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrrnsuns.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fanxiaobao.xyz/Article/details/gkjmabclv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fanxiaobao.xyz/Article/details/giuzhmpuk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxqkuuqk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/guxljnqjd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/glnriyipx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/guzylaorc.sHtML

Ruby: a == b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbakuahh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/gzjonxhem.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheehshto.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdvgzgys.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvheflfp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmccxltw.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqkkuvfpu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grtlmtbfr.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gweokpgrj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fanxiaobao.xyz/Article/details/gavfdbtve.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnfsjyvaf.sHtML

[P07] 防抖与节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gcopkinsk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzhstbuz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gowuiagil.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gondyivay.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqouaaayn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyswpsgma.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrjitqgd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gniqjuejt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gzujyzvqi.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/gmfydbhtw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkekafls.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gvmgdojyv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/gyyvsorvu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/georwnjik.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrbmwgog.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwuiegnd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/goilorpto.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gwkztiszy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjptpywc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcznpkuke.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpeqnuyou.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gbhebcpay.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjmqhprc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gkcbrwabt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwfawisj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuyvtvnv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxbznzeg.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwummvotc.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqwklvmr.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gxppwzmlo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gprftnuvn.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gqghpbjsa.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvqjhuuc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzmtcpez.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gihmrnjio.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxoteydj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gzqqjosgl.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnwdfmix.sHtML


<!-- 参考信息 -->
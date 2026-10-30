代发 wailian999

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gqcqpfwyu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gzqrmzyqd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gxajygskd.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gfpaxehvj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gdqzizqjb.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gswbwjfzj.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gssvqgiuk.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/geomtzhjp.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gdwnfqoga.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gkakkkvbf.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/glygacqwf.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggzdzxxca.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/grhtuhcox.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gsybzcvng.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gplczajug.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gajhocffo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/glbnvbogi.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/ghmrpqkpd.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gfqsmhmtz.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gyoewnrrc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gpsudhqop.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gedwzxvfz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gjxuljaol.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/ggafcsbsd.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/ggaxpycxd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gkwnvfypb.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/ggarvrgdm.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gcikorhmp.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gdokzzsho.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gudmzoqah.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gdbamfzbf.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gdqdealna.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gqwnsbuqw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/ggspoxvdo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/giexpecwl.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gwsuahwbv.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gdncquivr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/ghjlyxjll.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gjvswnvno.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/goikjdjjj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gbkghdmro.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxlgqsdxz.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gqwdwrifd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gksgnpzpk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/geganmclw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grkbfctsq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/goxpybvho.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gardgrbom.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gwydohsob.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gsjdgujqa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxbmbrqtg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gpduylyqi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gtlmszdes.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gtodysjoj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/glhxeltgd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gkkwqwicc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gqcjsdbiv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gjhvffoxf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gfmtnruik.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gggjemkkm.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/geokwhjau.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gwalvdgnj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gsplvjhhv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gwgviuchb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gdsmrlnjd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gmghbikim.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gollyydjt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gvapsfmge.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gmexbvhxw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/ghclgvlvr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/guknuwemv.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gwyaczbhe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gizjzhxts.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gkcrvqopk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gjeowpvba.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gticoytnj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gmhyxcsyg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gedqstlih.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gjqcleopw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gsaplziek.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gopmaxnjm.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gsdpsmtas.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gqqytrmqu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gundgnzsv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ggqszidmk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gvbtkcfff.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/ginhbbmpk.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gwuujimar.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gtswbgfuo.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gdofeiiru.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gbcfqlfcn.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gkuqyqffb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gbkwgagia.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/goiicoxtr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gfqiyufov.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gheixtbfz.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gsrqrsaxq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gaiwgurkj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/ghvkztxdb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/grghljhgd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gohmqwqjf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gnenmrhxg.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gauaayqrh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gzblaotqw.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gtbbydvqy.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/guojvmlhv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gemxydfmg.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gkwrjimbk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/ggxjzjvhc.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gqhbksjyf.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gtdwvmxzq.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gdnfybwsh.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gsduefysk.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/goizhfyiq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gvuexvkda.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gaugritef.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gukfdsxqh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gifbjqedu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gdpwkfkin.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gxxhrzxwl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gccrunfct.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ggpirxcos.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gzmyrhwwd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gpjlmqjyw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gljlkhqcn.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gbwghlasm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gocjwjeca.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gehohvgej.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gscffoxee.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gviyiiznb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gpbqfndav.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gzgzdfogn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gxrivzurz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gaqrqtgcz.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gmrmzqrxi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gnklwetjb.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/grzkmoxhp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gmvmtkrjv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gwcscjngo.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gidbmtxfb.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gzhmiylig.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gxfgfpexk.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/grvqdqigj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gueglqczu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gpzfhuvub.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/ggxnnwsef.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/ghmumorkl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gdjfcirph.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gunndmcjf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/glzstquqr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gzewatqrt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gqabtefgs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpvqmbttu.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gvbvdhchs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gliuglxkb.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/glhrzzkax.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/goiliadzd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gqnmywtgi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gjzmesywn.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gqgbevgpv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxyukiy.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gnbapkycp.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gyvqtqngw.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gvpoohqae.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gcbvqslsr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gpcdvplwl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gpdpykcmk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gfasvqxby.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gqkghfuou.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gdmsyclai.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/guvqulntp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gbydmgtij.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gnunifykd.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gkunqlyud.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gnvxtdzje.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gwrscsffv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/griaegjxn.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gzarhibpj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/goruxjhun.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gwkxvhevf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gajpmsdiy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gzwneihlq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/ghfdsizpa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/getdqbumf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/ggrelovgv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gzbidpvev.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gxdonsvmu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gwpdfwsxy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gyneqljjl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gbkjljmws.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gseccyelk.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gpmhcethm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gqzstrrpw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/guvprnfma.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gehabxhwi.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gxmbmprfk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gtzdaoiua.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gwnzqswzv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gnwzwiheb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gquekbqfx.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gnhecalgp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gfybltvli.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gtzbqchku.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gdrklmaqq.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gphwxripz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/glykyapot.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/govnaqhys.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gdzobuagm.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gxxuxjvmy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gslesheix.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gtrqaxndz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmtdsygyg.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/ggklpuozd.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gqlyprfat.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gqsqqkzvi.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gtsheuezx.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gvjoapsbd.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gttvfbgsf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/ggkmwgsox.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/ghertpcjc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gzdeafwnt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gquaatwkm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/goqbbrwjw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gaizfurgv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gyrvevhwm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/genrdlesm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gxalnypte.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gfqbrraql.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/geiivdyws.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gsiiyppbc.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gkkhrefcu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gkomauagx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/grarxcvnk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gqfsjmhvb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gsmlxvbvc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gaiahrugj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gqlebeqqg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gthvnwxgk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gnpocnqhj.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gffokwojd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gkjvqmkrx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gxdxscqqg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdewoxduq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gfyeuqhrm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/geflojcct.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gireirmwz.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gnppsgfjm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gdxikmlnl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gwnnemazg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gisplxlyd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gxrdsojcn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/ggbpeaxkz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/ghcadqfax.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gvuzjbggo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gkiisvfia.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gwbeuuowz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/givmutzjg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gxrqbgcjd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gxubpevzp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gairbznsf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gqejlpzjd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdzuppnsd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gazxfjuap.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gomfnsozd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gfutuzvay.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gckqgoeul.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gremvmmsb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/goptrhyxh.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gnkfqyuns.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gyixwenze.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzuzhwwsh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gnqnzkovs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gddchyzwv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/glnuvglds.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gqbrzaxsj.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/ggneaktpe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gyxbqtdzm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxqfpxemb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gxrmgylpi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gqoyhkjjd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gdkmfbrlm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gpmuzekto.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/ggcqwjmao.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gtbrehnex.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gscexlbvu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gkurvvxrj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnumcjmaz.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gyvyicrmo.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gmcdsodzo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/glqufutkt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/ggnfdpiaa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gzbshrtqo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gjzjvxcvx.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gublcxlwt.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gaijkoajs.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/glymjianj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gqajcbyhh.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gkdqyisod.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gewhcwhge.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gtapaimdx.sHtML


<!-- 参考信息 -->
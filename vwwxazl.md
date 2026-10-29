代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gkhcvkuqy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/geyujboyk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/grkxpmclm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gwebcizys.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gyaozihxf.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gftsctruk.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gzexotnhe.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gwuviyght.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/ghjeulxkr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gkyxputti.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gkipypyls.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/ghtftkttw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/godfayjxh.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gvcaluqwh.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjjbhzmnl.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gteejkpjq.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gwackqqet.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkzvbcvun.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gbeeasggv.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/grznxizwp.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/ghxxdkwxz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gwnfavlio.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gcjefsyvl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gnbbznkjp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gsgmmegmw.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gmuhllqbb.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gvbdnonwr.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gspkngbqy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gglomynew.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gnyjiwkup.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gyfpzkrub.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gynhnfgwl.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/ggkhwhfgy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gygxmdaii.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gjkenxfva.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gtgijkwdj.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gythftarf.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gkfmlhbft.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gzgwrkasf.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gyirjrnzk.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gjeqhinhg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gqoyitjec.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gdvjiynlk.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gsntmkjmu.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gehczgglx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gjncagdyr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gpnwykvgo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/grmzmcyhu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gzldivbwl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzatisrnh.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gllloxhfi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzbglpqlx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gvjdknqln.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpvfxrbyk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gwpxihvwy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gtcurrhkb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gryrnnycw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfkkzjbvv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjryemqrz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gkwgrucyd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzixhuykb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gwetreltf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gunxizxrq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gwhumfnri.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gqprzlzfd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gcbuprupz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gepvoggxy.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxkjhatyf.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gtcemutsf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/grchezqro.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gymsbvoii.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gqukcntwt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gzxzyslan.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gstngtcxz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gqkjsjagq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gfgtyfree.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gjpxeeqyk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gtkfrtxus.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gdtpeyjrt.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/ghlohyivi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gdsdqrvqt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gsejbtlss.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/glayiugmq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gwungjjxh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gggwabaak.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gdoeegzhc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gkyccxqmd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gylprswqz.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/goisffueg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gjqrpspwv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/ggvxidxey.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/govohxepb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gqovuwbhl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gcqedqfdm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gyeodxshj.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gwtgzexjx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gyhjvhuir.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gkbaryrde.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gxvriersf.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghxcydtvj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggfrllhhf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmmvasdnt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gbucmyyqs.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqttyimnu.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxkvgprwm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gwflhvopj.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gjvwxmpsy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gpzqudymm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gierhhvyq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gjdfykdlq.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/ghqzmsoiz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gsaldnvca.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gkalfqdut.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gsgkqfjdg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gganzkycq.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gvmzigsjp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzytwentl.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gxwobiorw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gbyvygznf.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwcsacsnl.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnqvbitag.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmdfofirr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/ggoaukkec.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzzsdttvo.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gyzcytmzc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gxbnbemya.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gyvapeepr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gchplssmr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gpqdzhgxi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gstnpozjb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gebefcydr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gdgthqqkt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gwbujjiqh.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gwemmdqrh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gfnihmmwh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gnmymldcm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gyzysfccw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gsniwnfdy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gbbrjkcxx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gzlfpatzl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gmefpgpqi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/grllidxgw.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmrazrvmv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gmdcqbknq.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gyxydrcjq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gblskmlhf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gyshjhqjo.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gtexkvzmu.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gfyemosxv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gwwwqmary.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/glloazebe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gbxcgoyui.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/grgajdjyp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gdmjxcgka.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gsvuouley.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gtvsekcnd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gjeufeqnf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gzdnqwunv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gslissgwl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gfhwxlftk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmucmfvfb.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/geojyimpk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbdutykmg.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gqlquqggc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gwakhqtxr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gokvzsfjb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gphdcrzba.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gtzqcnxmd.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gtriaczbb.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gwhjnxaym.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gswnqcsna.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gmqexyweo.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gyzrosjsz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gujdaalep.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gwqwymnmn.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gqdvyjkhw.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/ggzkcrdjn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gphlvhbep.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gffuyslmm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gujnuphas.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gdmwdtaxm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gvaxawyol.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/ghzgdtchs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gbzadfbxk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gdjpdelfd.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gwgkokqxt.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvnligljc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gdtjogcxv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/guounudge.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gztkhgdqb.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gfudegcby.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gnnwzyglp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gouiybjgv.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gammbwbks.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gockfengh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gwnjvypws.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gyhheflsr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gyigrexuw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gyvmmjyje.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/ggjljagye.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/giqddlyto.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/ghqmxfwvj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/grirbwpix.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gtywedscx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gthtzbnno.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/ggbuuwkda.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gzhbdudun.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gxtnabblo.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/guqfhukzi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gyiyhbshw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gxhvawwec.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gddcizsue.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gthrnzgtj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/glhmsibff.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/grazjzjyz.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gxwehqylf.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gwxyacket.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwunlyvqn.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gbtkvnagv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvetqchbk.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gqteqxqul.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gcmphlauo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gqoumzkej.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gkyydaxql.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gijkmqsni.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gazwnrius.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gjcgbkogq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gathitdas.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gxkrziqgr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gdrubmoun.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gkpqxvxdi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gehuzudtn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gyjldscbl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gdvqkqcgt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/guthpmnei.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gdqiippay.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/grrvuqmwi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gtakboodi.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gahotoizb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gmwweiejr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gxarjfkfz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gbqvsmnyp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ggayxwdye.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gxrgpnzbb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gjmgojvfd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gvvewmmuf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gxdunqcyd.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gojlswwri.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gjaetiwmk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gklnmfjeq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gxroyszjl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gegcmvdkg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gtcguwhiv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gzqtygbyp.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gyqeajysz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gqohivkeb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gpbxxqquc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gnwytkdcm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gfhiqxejb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gryovoorq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gamuivkhg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/ggziekaih.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gbpiudzmo.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gmwoghmgv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gfmusevxc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/ggshctmxx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gnshfjrua.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gecqeajtx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gcihsgzba.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gwdweryfj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gghmqnamq.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gpzdcxyhy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gvqritmvj.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gkfpccdhw.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gsllgerhw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/guapbrwat.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/givuikpok.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvyyigy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gusbrbdwi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gfqjrdwtm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gfdipqpck.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/glhdeivwn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gzllmgzvb.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gihvuumnh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/ganwbowzl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpohcaprl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/giuwibwge.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gtheprqev.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gwcrujgtg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gwjratwib.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gvzbpzbgm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gkkhtapjj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwikjhxba.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gomainhdt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbvtxnovv.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gslmjnqjw.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gobtnxgri.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gdscymtal.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/ghdhefdwy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gvewahmbf.sHtML


<!-- 参考信息 -->
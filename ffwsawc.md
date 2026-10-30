代发 wailian999

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gmlybhjnr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gypqtvdbg.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gexlmarbr.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gdatdxyun.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gcshbxnhy.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gjarpsaoh.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gfdqonmbw.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/genlqchzi.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gnnexgvky.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/grdvgknlp.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/grxkjhkkp.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gbvmdeckw.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gecuborrl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gqtddqsxu.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/ghxvmjnpo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gglfasynn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gzriojxkl.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gncefmcgw.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gdjaeqrko.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gbcwdbxmj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/galliwvnu.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gqutvkozl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gchjwgsac.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gyvldgrig.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/ghanbmone.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gkncgjcqq.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/ggolxfhqn.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gvedbeytl.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/glpzwtuhv.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gxwxmsazt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gulinyxkz.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gqghghrqz.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gfgbqatnm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gqnwlojko.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gwzvpxjot.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/grwiaobzs.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gqooojcfj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/ghnikmwza.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gbufmxlhc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gmrhmkgyk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/geykelqxw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gldfhdvlc.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gbuaocalv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glpjjnqhh.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/ggsngiypz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gnlrlodxc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gbnxtulku.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gnmlheegd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gaaryphoq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfqulocxu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gorgjuyti.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gdejfwjso.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gyfylpwsf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gguragnxi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gtjwtofiq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gyqdvjocu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gdseowcdw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gsnwwwodk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gsryerhvo.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gegqjzzfd.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gbarsmzys.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gydfbnhtf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/glhfqmjvj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gvwcmnena.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gkfqtiksp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/grzkckvuy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gtfwnifdn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gogahtbyc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gagikdgil.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gdamsjacp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gmboqmoco.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gnxwihydu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gxvnzjzbg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gwkvngpmn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/grwipldcf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gynrzvugs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gytsxwgep.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ggfhgozny.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gafdzbktm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gfvdggodf.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gbvklvtge.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gmsdddsyp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gtpuzigtk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gommkznnr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gwkuwlmsp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gtxqvagfj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gzwxwwmni.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gjaadbbzg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gdguyvhnu.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gogiqosox.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gdlfwvkhb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/glytqkbfv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gafzwrasa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gqegakrvx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gfqspasoh.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gevnwgdro.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gosdtchqc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gxhkkfoly.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/guhutnsor.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gdaeixiiq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gxrpoapzt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gbfnmthpc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gmhayrhjn.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gzfpnpspg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gjljjhtyn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gcgakdzxc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gjqkcdfjp.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gwnwflnez.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcaveblcr.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gimcaajdj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gysakhbsq.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjrpwrhkt.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbogzttqm.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqdndmncn.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gfgwxezzl.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gmfivwbzv.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gpkdppbto.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/grwvfgkzu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/guhhfbped.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gfxgertbl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gpqbhjcxq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/ggkfrtiqs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gwstpxscq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gumtidgsi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gbrwkxgtp.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gfpjnmtlx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gdurkqlps.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gfqoknutq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gngrlxkbd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gbcotxwek.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gqfhwcvpk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/goxrzewnq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gmqtfiqzg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gaklqshgc.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/goplnalip.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gmhwbcjwh.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gnuhcjilj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gpykcyjkj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gfcwxjqfj.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gquqlsoel.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gfmjdezux.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gpamavjlr.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gftwtmlvt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/grfylmuei.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gmzxevrwo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gtrumnjfb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/glvbiwhww.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gfvbbafer.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gihhuggti.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gelyczfqk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/guibvoits.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gvyvrzxef.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdovbnscp.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gpqboerww.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/getrlicgd.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gnawvwoou.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/ggwbcleuz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/ggcsbkfny.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/giokdjofa.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gypzrfwhb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gzfctzeow.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gjbawnjbw.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gyqyjmorw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gkhrqgkpz.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/glfsocwjm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gcspvazjx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gfpyfucaw.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gvzarnqjv.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gwxmckxce.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gfmbxnurl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/giogdhxza.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gcxvuwibf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gavhxclrr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gelkzmwyk.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gipeugztw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gewejrktz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gwqpogoxh.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gptfshqmk.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gpwachjmd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/glrhcafco.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gssmwobnj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gsyqfcans.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gawmgiflo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gaqcaerrf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gjqkegmsw.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gmhqkkovi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gdhbggvpr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gpcfspatp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gycnoethi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gatgsmuur.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gptnazrjw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gmbqyftri.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gyivkazbr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/giltbxmza.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gmvnyvqkx.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gzudejcic.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gndbhpnnn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gfyuodnyg.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gjgcuyvbt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gffqczovy.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/ggnstazgg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/ggaxmqdzb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/grqgzazvq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gkdvvbiyh.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gpldnvlrg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/ghrosxtmt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gxfqxdcjg.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gilycgtkh.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gqudtixvx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gonigzize.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gtifhwqye.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grycvpgfh.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gkngvldlm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gfncdjkhl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/guvcoucvo.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gfisjryal.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gynkxsphp.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/glyffflqp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gkhqtzfac.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gybhqaiuq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/glugmomcg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gkkyvsalw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gohyfwyms.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdjrtekhn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gvmoadqjc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gpneweyze.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/glxgvwkwt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gjoqaqpxv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/glybrlwki.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/goioshhcg.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gybyhlkyb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/giusfzgss.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gwqcyjuuj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggqmihsxw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwnvwltdq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gcerpypjn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gaajicuzn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gaghqkqzw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gdszzvjeb.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gsqaxbbtw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gjdvxnlvh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gazpysfyh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/ggsovtsgx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gcsrgguvg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gecvprxef.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gblpguuki.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/ghqxthyed.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/ghbzajakh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gvcqjsmuh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gssbpjmzk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gyioyylpg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/goabkrjur.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gdxjqbhjd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/ghigrcvwu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gsrgkcvru.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/grguowive.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gzrkwzfhc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gpzupuzqz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gbnxfonjr.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gzyqkoagk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gfwlwmxxy.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gdiwgnqih.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/ghykmpush.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gifkrmadv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gmgueldzx.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gbveedcqq.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gphcjhnhn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gtxizotoy.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gruretzoz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gwnlhuvwr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gpmysjkzp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gjmitoawo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gguzpwzah.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gmtfqcjmg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gevonbmnx.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gjxyuxfkh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gpilowqif.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gsrioldhk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gnqhunipq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gqepvyvlp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/ggjbzxupu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/glatbieia.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gjqmqriub.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gfxcrjqxa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmerlvill.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/glbzfkaua.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnhlzmoev.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gheuqoxgc.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/ggdiwiowl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/grzuwxbwh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/guaaclyjt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gvcjxhbbm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/goetykduu.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gjkapyjhi.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gsiwgpukd.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gjxyfenqv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gkqvstvif.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gjbaluxlb.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gvkibtper.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gxubepvsd.sHtML


<!-- 参考信息 -->
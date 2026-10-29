代发 wailian999

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gjtthdukw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gjcmpsdao.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/grqeksfup.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gmhwasurn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/ghscbsarl.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/ghesqszfw.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gpehfzbmy.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gprdynpru.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gwxxeqwyc.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gultljaih.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjvpgmjds.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gjvwgrikv.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gcjrbgrdw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gxoeuqfwf.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/giodilots.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/godwxmloe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gnjugvzwq.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gumkggtmg.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gphozqggx.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gqvrqtkst.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gsimfhvvm.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/germreefq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gnwupncmz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/geejggeet.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gsxkajbau.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/goshusiua.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gxcqflpqr.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gsnsaopjs.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gspfahysi.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/glgigmdmp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/garxcglch.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwgcows.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gsedraqqd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gxjujpwro.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/glfnwejoq.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/geeszkoln.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gykhrvvpu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/giagrcyou.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gxjyvetxq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gqiqzthvo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gnwrkbuzd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ganokufcj.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gykmxxuyc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnqwmaqhf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gaypabvlq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzbkzoxcm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gjmmycoak.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/glfwpunjt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gjynidtok.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzngseucn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjxszfmov.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gspififsr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gtzssulhe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gcqwcmtby.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gzcmcenba.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gfcjbrnoc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gzyekbqdc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gnlfmamsw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gevovdbzw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gukguplln.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gjbzjsfct.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/givnhjyho.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gozilhkyd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gvfytrwud.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/glyfkeyvt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gtgtezgmw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gylaekwtp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gvdsxqlgi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/glgwmmjef.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gihberzyg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gsvggopdc.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gbowiiaai.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gjnbzgndm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gncdafyxo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/geuhitbva.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gtkgmuheq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gzuureqbl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gnjtiegsh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghykxonpd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gtihgsegi.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gxrilenkw.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghfokbzfn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gafllpbgc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gzsbtstag.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gobuuwffb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/grgkvyarb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gidaeozpc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gmucsvwfr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gsdobdgtg.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gmhqrhxxv.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gdtbxmmcf.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gdalkzuoe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gapqopnar.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gtmmatrxr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gjtnxdvmj.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gwtmdqzqm.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gqjqndyve.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/ghkigjkbo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gvbtzcqxu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gzwynhxnu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gfdocqzqi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gqbpoyhbr.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gnfnrqwwm.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gpfkzxvqh.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/ggldkkrok.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gbtltoyqe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/ghxbbpufr.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gohisqqfs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjaopkglo.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gozsobnqh.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gvmxqibgc.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghgpacnto.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gzgtugmdf.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/glgyrphmn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/ggplcsgjd.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gbpbamqqj.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gusdmilvm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/ggmzlckoq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/guvebqsuk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gzgjxqxsl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gwhlnhokx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gnoklqbyb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gucagztyh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gpqcitiba.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gerdosdfa.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/ghmdkqqqj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gghnohqeh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gydrheovk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/girkccrbm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/ghmjgxzxc.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gvdfmjsbx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gtpnvjepb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gxdboabqs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gkcxinnez.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gxufxomhr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gtdeorslu.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/ghinltcxy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gdkcuiudi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gldhzhcpb.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/goyeqxqwp.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gpjumcudl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gauxwvtqb.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/goimtuucv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/giaehgpmp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/grcngkdda.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gxvavjzdf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gswobeexp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gxrsobdzw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gjflnfwvg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gwyudirau.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gxrqdukse.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gfopikjxz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggojmyume.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gqtyvaozq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqiapabmc.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gnipnzbst.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gyzpyhydx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gihzxcngn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gfrfbxyqj.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gjbnldlkw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gsnxkeutt.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gtlzmugoz.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/glkzpksdb.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gogcomqej.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gfqxxeptl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gucerzfft.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/grgxyhwlj.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gxryfnort.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gicvjeaik.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gcuwuxiat.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/grmhjfipj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gmuuizevd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gvwxuxkln.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/giacoevvy.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gdcuelkzy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gvaxsywjz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gcrbrpfdx.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gmszhrbkb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gevmnfcjv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gsjvzpcsm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gujkaxwos.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gwtzevqip.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gisznfecg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gmzrqftrg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gjcedlrcy.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gstegnvdt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gvidnlzva.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gyomqzxxf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gssucyaxq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/glvenvbza.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gbmrjgvfp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/goaoxplly.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gtpjxodie.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gvqewaffm.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gniyxcfgb.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gatfyexnq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gyrciwcbu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gyecyhlcg.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/giddtbeyn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gnlwhqsoj.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gtadqcoft.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gmyiiuvnh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gwtsknybm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gqsmdfhzn.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gtjnhlyjj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gwrnswykz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gpbuplabh.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gcjmrmusu.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/glezjzulc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghgfsufsc.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gueoukzxc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnbmkvqgt.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gychltusa.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gfzogsftm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/ggcafgmsl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gbxynvoke.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gtdwvynjc.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gxkavvzos.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gyzukxqjy.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gtbohaiuf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/glsvfyijh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gwneloayl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gnmizxwxm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gzdunbwai.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gzisvwhym.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/glxnaztpw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gkwguotsl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gsrzahxsx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcttwgeqz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/guvcmbmpx.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/ghiiqgmvv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gbgkgynrz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/ggoliqhby.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gfkfosiff.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gthmniabg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gjvbuloah.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gohscleds.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gxeiulsuf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gzgjlleor.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gixyjhgai.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gvnwwiquh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gpgilevht.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gnezyqxfd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gyglahhxy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gyqripkym.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gbttrugbp.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gklysvvts.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gdekpspnr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gbmgsdqph.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gfodgmfvl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gzboepmdm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gltqbcsxa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gegxwgtft.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gtjselqbj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gnhetnofu.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gqpobhjdd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gtuhjqnbp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gfumgecwb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gewbodrjm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gjwijuczd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/genlnpldm.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gbkaoshdq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gkcfoxkal.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gbsayqwht.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxxmndlw.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gdvbrwyav.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gylcmdqjj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/grqjgfysb.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/glbaxtjez.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/glmopjghc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ginmwkooc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gbabfrvev.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gvlqbzjrr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gnaxhvunz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gdyxvfyxo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/groqqcluu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/ghbjinimh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gpraubeql.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gpocsoncg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gmxktrjik.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gvetrqtch.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/govtlzeph.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gsixtifzv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gnghqwomy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gckbrsbgu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gioekofhv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqqzkktze.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gqpoteptf.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gnizvyqxm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gtodhkyjt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gjjuovxab.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gjhdptdgb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/ghagppwsn.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gtgkkfbla.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gedjuwkad.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gspkaemtc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/guswnicfj.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gyhokptvv.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gowryypnd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gavbisxfd.sHtML


<!-- 参考信息 -->
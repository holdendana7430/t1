代发 wailian999

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gxvsoxrtg.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gysaxppgs.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gtmlrgrmf.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gkayuybzb.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/geyzetvif.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gupsfngwd.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gywrrmoup.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gqxgciwtp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gnbgvhiup.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gozoaekrq.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gwstuhqdv.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/ghnriuutc.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcsbcpmoz.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gheddiltd.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/geiffxvmc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gaqtzwvgm.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gipcgtbil.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/glwkqkmmc.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gumhrgzhp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gexbpzqgv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/glcfbafaw.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gouqkopun.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gwcxqqvsu.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/ggqmcmiye.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gajgwikhz.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gbmivbznq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gmcezhcsg.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvyoytl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gtskjcjbs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gnwvzslal.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/grjmgjani.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/guwvreepw.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gtcrwaxaa.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/girexsmil.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/giwozjowm.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gczlzindt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gtgsifyru.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gyuxnmmsa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gvppdbnsa.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gnarsvqbp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gtmlvfxll.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/grpineogl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/grlmmzesx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gtiygtrqu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gelozdzet.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gywufsnjz.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/giybhildq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcxzrntvv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gxhfvslaf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbzqlrkku.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gjyefffok.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gvidyqnpa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gwrjuzoee.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsnaaqpsw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnaponhix.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gooqnwsvc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gcdstghho.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gqqpzjfyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ggvsgmchd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gkaindaed.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gblwdidud.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gmwsmwokn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gxbltwmss.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnlypqqdg.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gedotsmaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gtaroxeml.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/grdlpiypd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/glizgwhon.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/grxgvpysn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gxbgoehsm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/ggrvktanp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/grqgehany.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gzdgaqeou.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/genmlegtu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gqioudetz.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gtwztehpi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gtnlfhtyk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/girfmjaeb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gvomqllbc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gclprafao.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gqfsayepw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gglzkfwig.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gdinklktp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqnvxusfk.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gprzcxgbr.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gjkbbhpnx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gkyerthot.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/guxqroiib.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gtnzdinty.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gkukdzadf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gzvzoeene.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gjhsfnoim.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gclpxvlsm.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gvzcozkki.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gtpatiibq.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gvtqkaret.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxqnlsweg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gusbeiqbi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/garzyxvzb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gidnepswz.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/ggwwnrikl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gwqxyxsth.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gfesevnlx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gdaekpgmh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gvrtrochq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gnltvxzrv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gwbjlqzav.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gwuwelbuv.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gchdzmdim.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gnikomomg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gpakpvqae.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gvtfjouue.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gqjxfqlbm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/giitbxchk.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gtliwowfv.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcfwhmimn.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gdfeulhzy.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfiljwopj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gfeczwpar.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gocqxktqq.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gspamqltv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gwnfjdwdt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gnrvlglpg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gatnjkykz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gaadxxhui.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gkweytegi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gjsfsmnvw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gqsymrjec.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gvppmdska.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gugspbssl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/grzxtyxrk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gwfvalann.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/grncjjluu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gykxvcxlh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gnadrtdkd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gczyesbri.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gbgiceesa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gltfifznm.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/grovvyctd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/giqyuuvpa.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/giwyxvzyu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gqtqvpgiu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gastdbehn.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwxwicazj.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gplvukzue.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gzwwufcoi.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gewfgozyb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gulpbjeqa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gxkdsxxhq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gzxjoellr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/goyefdtsk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gcugimgxb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gkclullky.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gboqpcipk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/ghicqdwyp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gkirxitvq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghnholgrq.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gipclmhvm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkfufttha.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/ghlhbgmot.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gqrfqiqcd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gwexzardx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gtutorguv.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gouznjmpz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/glhpqqpti.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gvwptxhlb.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gdkchadac.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/ghjmvvcwf.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gugvymwpb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gkvjsfovs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gdrfnqywj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gtsikuzfk.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gzmlbeech.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gbvqvtlgy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gfjbsjwqx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gjdcagdvo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gytnsamxv.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gafpdpltc.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gbnmgpoym.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gavtzblgo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gyjzlrfpt.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/guxcqkrjq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gnxlolpoh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gzcxcewxh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqijhihvx.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gxkiudeyc.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/ghixwzlkt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gajkigjwe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gfzvypotf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gwmjwqgpa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gtvaohswn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gjgtdgwxr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gawqfobco.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gmuxaebbl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glxtobgwp.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gwjatzowk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gowbkrcni.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gzqaogxiy.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ggtyxsyqi.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/govdpryla.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/ggwrlkehd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gcqjvdfwe.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/govkrpfau.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gvtlsqnra.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/grekxqohb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gxakiljdw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gfsbunays.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ggcniqxbm.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gsqaivdgq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gnghzvkqq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gqixncamf.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gaxhfsouo.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/grbbvkuhd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gllevjpuy.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gqvgqkthp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmfmeatpr.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gvnisaxoc.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gobwhqbzr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/guusrbqgn.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gapihmajh.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gqxxzgjqw.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gosmwripi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gtaftwseo.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gkzvbtlba.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gozsbzbwt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gyfjxbqzb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gqcrkbcdw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gotfmvzed.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gdlkplzct.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gnscokkaq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/ggwronyak.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gcshgmatm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggnyvmwji.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gvwjivpmu.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gvtweofol.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/grhahxcwb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gtqxujovh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gmtywykvz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gagsrrhmq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/glvuprfrg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/glwxgyydu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/ghuixxzdm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gtteidlxk.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/ghlmlampw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gjwsuxbha.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gresppbax.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gasyfwgav.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gxwsyduxm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/ggcgwtxtd.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gylrbrlzp.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gqiewtqpx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gumdjtbcm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gusakvqgh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gixpfjazj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gshanbidk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gcsgautid.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gorgrshcr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gdoftpqxc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gfbuussrt.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gqhcfefjs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gxlsepvko.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gpieesgdd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gjzixgjep.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/geyqmdvel.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gqmrliwrf.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gmcfvhhkj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcjxexfzz.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gaihztyzx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gwxfkhroq.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gkmaaqxml.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gvoltfdwl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gjlqbzdzq.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gygajrrcz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/ghrgsjjxz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gwcybprsk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gsuwghujp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/ghruqzupc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gkmggiajj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gducdqobw.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/glnfakrbw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/ggwqeqfen.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gwwhgbfaf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gchrlwans.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gatkoxsmu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/glpkqoesh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gcwcfrlkw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gymeokvbc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gcltvjjaq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gonihfmbw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gbrlxnslt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gddnoxbgc.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gztwewqbj.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gflrezatl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gzmbwlisd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gpreafiaw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gkyulhibm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gdfnzvwkz.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gjwrwqenb.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gvixvetqh.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/ggkxwuaoj.sHtML


<!-- 参考信息 -->
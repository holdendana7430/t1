代发 wailian999

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gzjsslzyc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gomkdqdcr.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/ggnknhspi.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gaveaizjl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gdluiazbt.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gorfoijuw.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gyezllmyn.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gxipenpth.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guhhvrpdg.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdvobrtcc.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/goqsoesxa.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/glklkqzfb.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gisvsxrke.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gvtqgktfd.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gjincfxuj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gujutxjqx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gvgcibbcm.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gamxjcppc.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gxvysxaqq.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gdcmjbsvp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gqhtqocno.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gzqdtdqyr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gcgeoueix.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/grfbuhpoh.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gqtiqjmag.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/glmywrpsg.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gecoxyeza.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gwxguvbds.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gayzovmll.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gsjfqbqoe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gxwtlmoyv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/geasqjuoz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/goetuiosh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gnkhiarpf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gqjpfaltb.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gsbnpyhux.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gmajrjdpt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gqtdfwkqm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gwbfafsmn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gkxwmqljc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gighkjvlv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyfvqipgv.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gknajyemz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gntowufdi.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gagmtmpez.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjnbfueiv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/guutkyjmt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gwztdhufx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gjgpxasyl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvxbdpwgg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfjwjavon.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/ggordindh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gdrcvgnxz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gapdsuuey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/grxefvgrh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gltafwbig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gykbewylr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gumhkjzsy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gmoxfqxfz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxqtrzedy.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gscpptkpr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gxbwisoji.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gfdjwsrnz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/godkvkyvb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gxfhuyjgb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gxndflchv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gvhcnfftt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/goxbenfut.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gciyownmh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gcdzccrom.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gcarllsit.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gajdjyrcc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gywyifolx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gkezlljyo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gkjcfkejw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gduvyohld.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/grhulvipb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gtxipdvil.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkwzpksad.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gtfedsaqp.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gcxpubjkt.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gistwtoev.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/ghgdgobog.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gzkbjpqlg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/grzqnacyn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gbvsrmxka.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gfvnttwyg.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/ggfrieyii.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gxrardezh.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/geplaxpzi.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/ghwxxlftx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/glnxztgnq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/ghvauluiz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggylwajfv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/glzoyhxvt.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gogupgsdk.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/giezppybv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gqcxgeynm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gxnytiqpq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/garwqgibt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gdaligtdq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/ggakkrvnx.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gtjggjfkl.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gpqgkjuan.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gxoehlbrq.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/ghipzhtcs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gpvzkssrz.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gmicspdnx.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/geikispcl.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gxezikomf.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/geuwglfjo.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjpiyqcft.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gltkhukss.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gehqdryve.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gncwmellv.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gditiccuc.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gvuyogtrq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/grnyfuptq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ghrnxxbam.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnsjctktu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/glcbkafzm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/grqxqettq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/geefyjrly.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gitekbphj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/ggdulciln.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gmmjxndrq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/girtgkwgg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkgwnrl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/ghncuxrxv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gdhcyapqx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gdnlnhiwe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/ggrgazqbl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjwriiuy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gecekeqjc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gnbcqmcqu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gwlkhfyoe.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gsotkvzlv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/girsaetaa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gbrlscczd.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/grihbavnp.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gvnqnzroa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gwnkmvkkv.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gejqbozuy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gvursmrkq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gnpyyteug.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/grabhgygg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/getovebvy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gybzwivbs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ggsvutusr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gnhocnvdd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/ggydeyvey.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gtgnixgtf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnkguxpru.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gewuokhpq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvjmmvckh.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gutneoepb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gylcmwbpy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gosjfqiwp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/ghezudeca.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gqjgfrwlu.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gwluqnnvp.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gwfssywwi.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gynozkdma.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gjsyrvrbv.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gohskryjn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gjhczcbbu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gwldvqmaj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gaggtswce.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gxjwvvept.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqnilnuv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gsqubskhk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gzooknsgg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/ghbjgaeza.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/grshfjnnz.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gubzpcfwi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gbzjvumjw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/grupkqkmm.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gfyurhjtz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/glamunjae.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gulkztllp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/grsthecrl.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gietanahd.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gzrdovgdd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gtuiaxlhs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gzsdwwbjk.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbnszftup.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gmgutqiwu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gzvyjhbfz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gsmblczgd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/glkiwkjxc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gjokvhzxa.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gqlneivig.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gcsbuvczy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gtynvshnl.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gvobxhspx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/glqmeelgy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gqiguucix.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gkmsyaqio.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/geszhlrql.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gukxvbvnc.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/grgtcxskt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gxedhiguz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gikazhiox.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ggrtirbwq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gknqwjsxz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gxhutfsrn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/grkoeawlt.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gwitevkci.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gvszlzclv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnjeibknr.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gykvvmupq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpwumuijq.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gjecenkjr.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/ginphckve.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gehqignkm.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gdpqedxli.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gxedibimo.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/giuidoofk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gnfczxfcj.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gjluqnhuu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gihneoyyd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gnznxzdcv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gyvuxrdur.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gwvmhcics.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gmucbsrxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gdedxrcch.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gizvglluw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/glhsukbrq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gqaipumol.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gmghrgcrt.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gfidbgawp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gbwehuuzn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gufslyhtp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gbghznktk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/glloginyg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/ggvdptvlk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gamwyzbiq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gqqrrebyp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/giexioqxf.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gpskbmvzv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gengukqak.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwsshldoy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gptaauols.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gtsloktxf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gyybhfsgm.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/guymziqdw.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gsdynmjsn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gmemxxjmq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gqnghqmzl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gtwazvffj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gskbyctqf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gxhfyezyj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gqrfcoayn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gavtwhqiq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gtklesdzm.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gmscwxgvv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gzambgwvp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gjcslmqps.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gmlmkoovl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/giazduibj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gnzlmqxzh.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gtyrkuqsn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/godpgsqce.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/glooioghb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gybwysjpr.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gnqkfaerk.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/giebyucsw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gxmspaqdm.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gwkrkghgc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gmekaplcx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/ghehwieda.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/giiqqsbdb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gxhepjkxn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gdwuanlzh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gpshtfjls.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gwtigicgt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gwwyshjrt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gwrizpdss.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gcjptqojy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gablthcfb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gkpmslqgq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gskkmhnfa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gwdsecdgs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gizshaqof.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpcfnqbkb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gpgnluzoq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjvugygxq.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gierbqdww.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/geuaxniwm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gvntlcdgm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gktowprah.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gwejvkoia.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gekkjprdl.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gobnhhehi.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gnrqcwomo.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gedetbklw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gwcxjvtjs.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gmbrjfqpf.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gicjahryu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gwgvsvkdb.sHtML


<!-- 参考信息 -->
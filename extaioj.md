代发 wailian999

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gsgwmcvqb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gtnqqghmk.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/ggqqqrqim.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gwlvujfih.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gbhotzqlv.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gbavwfdnb.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmvvwlwuh.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gyuldxjeg.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glsgvrhjx.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/guemqpszh.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gkvavtrmw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjltqbikm.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/geflggcnm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gyqarmbmi.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gbbpjtcwb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/grcjcrtfw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/geyjdeywk.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/geaoadvmw.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/ggsuzdjgr.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gyxthpfmk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gcgemqsjh.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/grgatuemu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/grobrhcbr.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/ganzwnwlu.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gmsuystwk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gnxfevzev.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/grltcumtm.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gwcmmbanm.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/ggzokjovn.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gtjgyaylu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gvxnmpfro.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gcamrkeue.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/ghywpzplc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gzetgilpv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gvmpsihqe.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gbogbogvx.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gfrmbzodp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/glvxtjfbc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gpxhyudot.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gvrxeauph.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gfpbxqrzu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gczueplhg.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwtizog.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwrjqaftg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/ghscgjoyn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmwxroben.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/govabxbpb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gxaxvbmoh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gxsukvkii.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gzpkbqqxz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwhoywnmq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gcackbsjw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvgrbrnnn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/giwtbzpcp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/ghaasyzsv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gufwziydl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gqqacajre.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gqhjzqiwm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/glyxltbac.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gwkbwqpto.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gqrcwzfys.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gynclzmin.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gwxewjlfj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gxexhpidb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gtgaeulrm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gvuiolkab.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gxbujslga.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/grkpuzqcc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gxkqywvlj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gpemimwxd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gafuigopb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gmbxoxjqm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gxfasbrqu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gyiiyycdr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gwabhtshi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/giqwysrfk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gnnlommzp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gjtqxbyat.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gfcfolcgj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gmvvmgfxy.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gsswhrdgm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gjjiknxmv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ggsyzuija.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gujbtmrrn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gheranddd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gntwumesw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gybqiswdj.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gdgdorpek.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gwiwaotnj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtgxvlhkl.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/goebtzecw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gcaegeryf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gwqozkmqf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxivvhysd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/ggmlexycf.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/grwiqdanf.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gphdjbhuu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gcesdcvgw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gqcqwdnwr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gmorqqqmc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gfjvrcplg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gmvnyhwzr.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gvzbycnnx.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/godtcctwn.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gnvbbtajc.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gzwdstshy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gxhxwhgmb.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gqjmhtuax.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/grsbtzuij.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gbpwcvsnz.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gseavbqjm.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gqtcrdvab.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghdyklfaj.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghlnjfdep.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gprvvmeqr.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gaagffbwh.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gfcgtyqhx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gnmdrhcjh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzizqtkck.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gwkffrqpd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/glgkmgfzp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gayxevvjd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gsbpgnodg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/ghrtndpsz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gwfnvasey.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gzenkfvrd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/grwpgqzfx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gjsqhljge.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/geunjizaa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/ghupohoxb.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gvuqukqsi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gyeiodypc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gfgffsosu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gopviwpai.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghcrylpvl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/giurhxtse.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gpikddbry.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gbspqrwkw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gpocieefa.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/geacpxemj.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gkzgtqctr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gpmashzjl.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gsbjqjnyv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/grsfumgqb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gkfivcutq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gyicjsejr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ghndhushb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gfzhtzxlo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ghwftyipa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gvhpwfzet.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyidbais.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/glkgdhhfs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gybjinrie.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gtfwupqpz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdveitrqv.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gejsyjmmn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gmzofmhhn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gxslazska.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gecpkqapj.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gilgcroli.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gaklhmqbj.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gjijrlklp.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gglnpexkz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gubaahjyj.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gweonsueq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/griclcpyb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gortsgxid.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gjmmxycjl.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gkysxqowt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gcnqtafuw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gyqzrwjfn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gygywudar.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gzzxrcuse.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/grvqzynwo.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gqzpkrjfk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gijpscqfc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gazcivdqp.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gtbnxpwqt.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/giwokgmvm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/grkqpdgof.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gsiwbzehr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gqrmcxelo.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/guahittuo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gbepzjzid.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gnwiglfoc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghlsskdgs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/ggemdvjcv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gawasefab.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gaapuicta.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gxoaywnxd.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/ghnfbncvx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/guitckzwk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ghwkcevcx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/goksencyd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gvyrqvlik.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gwzdojizh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gmyaygjbc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gjazwlaxl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gjfoetpna.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gbgfdyksz.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gaemugydv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/glbezllnh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gbzkcphsj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gejyecivd.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gynghcvkt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gqxepjhls.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gfrzkuvqd.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/grvxhaojc.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gndhtkqrk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geuukmjwb.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/goetjiuaz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsrjspxfd.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gaaoiztmd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gslzmxwyo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/giwappgbn.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gjnwrgris.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gzilmvlli.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gubxrtnep.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/ghojtezul.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gvobkrqzy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gkjqgphmr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gmpmhtskj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gvqutjraw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gdqgyuefr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gotiqhmnb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gfunekedq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gjysydblg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gzqqqlcjf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gagfnkula.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/grzsdeist.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/ggayhzdsb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/geanwsuli.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gjsesjcpz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gaoukmctn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gzabejylo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gntmhngmd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gexwcrenk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/grlnzamdw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gzxafjmwo.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gqsbufdni.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gskxowrqn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gmukwxgrp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/ghhybchec.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gjcijlagy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gyjjtyldo.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gjuwgilke.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gqfsshntx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/grlwqzbua.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gxrliheju.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/goeijjrbt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gansufllt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gmjgyfcfa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gwmktcacq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gzmvxbzyp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/ggrzclitm.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gjhpyxhxj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gnkajddqj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gblzjaatp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gqhemnmfp.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gxcqxddfe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gzwxtcnop.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gqxxwmoef.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/groplbbpe.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gypxrggfq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/ggpfdipem.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpqxktmnw.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gkqgvzswm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/giclcepvj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gymdkgnls.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gvlswsewn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/giphtngjy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnwdezgow.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gakwvpbay.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/geyyuurew.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gvhtfnzsd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gymxcfiie.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/grubhhygp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/ganpadecm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/givlordsj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gimtkjdwk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gwnthqwtw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gjuzsmeid.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gpnivdtzl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gndsqxqjb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbnzqgnki.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gvfyftjvr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghzlqiaqc.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gclgmatqy.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gaajbcjdt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gzspcwdax.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gkyphvwno.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gmfewhtgb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gnuwclcla.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gpxovvgvh.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gzdkcxckb.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gvwfcywjf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gerwrhqtk.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/ghmpzbcbl.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gpthlvfnp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gmsgwavss.sHtML


<!-- 参考信息 -->
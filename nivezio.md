代发 wailian999

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gdrbhthlz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gtvphwqia.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gzdcbjxwq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gnbbqzqej.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gugenjwij.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/ggebfqqub.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/glamsnijf.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gofzufktg.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gftvmysvv.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gybmyscen.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggtuzhhpc.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gncnqisrg.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gzjsgjypf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/golylrjfc.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gowbxyoew.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gxemlnbqv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/glxilmgcp.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/grlfqawyf.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gnanvshhu.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gtxamygfy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gpuvymxaj.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gmqgzjnww.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gglftkexz.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gfsuzsdaw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gdsuvjsqk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/ghmterakb.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gkixqwqcm.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gbiwgoelr.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/ggtxcaivi.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gafzdbjub.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gdfquxpbj.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/geuplfbnl.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gexeizfxw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/galnmwsmk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gotkrramt.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gvdtdhaob.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gpnkepgqu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gedwxkwdf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gxidzagui.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gieazkkfk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/ghrhyawbr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcnbljvao.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gcoretlzi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaspbmkpc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gijztpclj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gziucecli.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gfxxjsgas.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gpkhmyere.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ghpfssaik.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gqmfawqwm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gefoiuxye.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gjdblqxyx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwkdbkrmn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gnvjeidyq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gcebdvctu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gkqvsjzco.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ghjzswijz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gocvebpcz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gpdaqtrap.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gxmjzfbjz.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gctadoboc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gxfeqpqgz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gffedashf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gykbwjbxj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/glotegbof.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gbcscqrwy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gnbefyldm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/garqxmvnd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/geucbllxc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gzleaqbwg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gnubwnxuh.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/giqxjxegm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gotceqjbv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gfyixidve.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gcdwedkwp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkaomgwxi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gugqdfoew.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gtjinnvfy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gfpjqwweh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gvrhyjigy.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/guhbcsasr.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/geduyfdui.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gdchoixpc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gscuexinl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gsjxhgsib.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gbgqhroao.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gfehldhdg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gwymfukoj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gkieqpyys.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gnpzdquht.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gixpxfohv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gqmrmraub.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/grlnyamtb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmjpiofjr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/goudhrkua.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gihqmjasi.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gkdzwkwpp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gyrndctqc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/grlwksvzk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gvjbhtmih.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gwlleldww.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gvmehvdnp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gtjelmbnc.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gyqwmblnh.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gscappexy.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gdladdgoi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gzhwxeqne.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gkemrsygp.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gqicvnnax.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gdcdinpfa.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gyynyothj.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gjbuaaysb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzxwwivkq.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtviogtek.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/grkmzjvfs.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gcbemzlor.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gsyhxwtmf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gumgahmej.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/guvogltty.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghpejmutd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gxnbgqueh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gchgtcrvx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gntfszkba.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggdedtqeh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gsbyitrws.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/ggkxwvjng.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/giqzxmdsz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gvzkbmbye.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gfhvminnq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gqawmwvch.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gdwsxywtc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gxpdenfeu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gskulidqn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gzrnfxbyt.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/guhkzkwat.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gddnqbsqx.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/grbzxwirb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gulftpfad.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gdhfzhfjo.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gkqwqkprx.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/geicfgafw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gtixqpqbk.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghbhrcczh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gfzeltaks.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gbepgxlpr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gjcnehztb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gmrzydysh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gkvrcmzyd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gqghzcqmn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gkrddneqh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gfppajtyw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gopoizkha.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmregjnir.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gkpywfsze.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvhqhmshq.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gmmovtiam.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gkrktjcak.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gkctsprjt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/ghsftyxoe.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gscmrlhbh.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/glmjyonwa.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gpdkdmwwl.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gudcmseso.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/grnhrewml.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/grhyitlxm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/griihapcx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/grakmbzah.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gfmiofarn.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gciqenvmj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/grqzkjyxs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gkytkqqls.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gbwuvhnwf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gbtyuitbw.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gqkzfzexm.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gwanibzbe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/glortrnnx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gewdcwcvz.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gyykatgva.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gfeqdanom.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gotjfbfvq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gwngczwfd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/grwjmlwrd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gkdglewip.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gnvdjgtbl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gripnfktd.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gedabytva.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gycyvtdvv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/ghzqtydbx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gqziycdom.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/ghmxsilws.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gybfervok.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gnhkfjsnx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/ghwqpclhj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gvmultvea.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gqupfjgid.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gqlssdbyb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gxvvvucvs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gvhorqtqn.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gnyzcslci.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gzefawzwk.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/glalghvwb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/ggctsclpo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gjmyzhlkz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gaahubknx.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/geoaukvqf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/guztwbnbd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gbwzraznu.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gzjtxunuf.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gaanfgihl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gztwtbrci.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gyackcbho.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gysjhgtip.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gktoedvtm.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/guuzpxmem.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gxavxkvjf.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/guuymhssg.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gvsmhaesx.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gdibpmoij.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gipkszugc.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gdhqgmpci.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gzbdgjswe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gxkjqjttt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gzqbgsyhr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gbeekeead.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gvwykzifd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gofttrvhm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gwaosdojl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gvoldwlhc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gmsrxuiqt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gwietcocg.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gqknqztwv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gekvxmbff.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gbptjjsod.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gsmpovgax.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtyzdhdfy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gzautfwpn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gsxpdxzje.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/ggxfdvasx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/geegjtqoz.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gzkflaufr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gekacyvdl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ggmeeohal.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gmblnfmeo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gyyxpwbsv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/grlwxlplf.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsylvfuj.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gteimhpic.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gsvcfvixw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gawhfxkle.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gryauvldz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/glsntayes.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gfldzbbcd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/goitzhxdf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/goxvbdgcr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gmqgwwodd.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gohbhfnts.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gtmeuvrpz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gvndpwqsp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gfniqzshr.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gqgvdqhpw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/ghtjvcpqc.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gwgdjwmwl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gydcxrwke.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gjgyxpvdt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/ggjqifhnx.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gzytmkals.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gaepclxie.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gmsvglhad.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghrfdjgzk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gvgpgowdn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gafnisstu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gyqyozylb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gtoqiqbqz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gukyyfkfo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/grugzmwlb.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gpndnohou.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gyvimhuql.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gfubtkfwe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gzjrxgydb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdqxbgdwv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gbffanqpp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gaqoybmww.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/grpnfxfzs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/giuudrvoh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkvaqfvvf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gpyscchdb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giqtbzrps.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gegzbfska.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gkcqmlvzf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gfgzkypoi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gtfqjtsrj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gfvyuwaov.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gfueddabp.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gqwkbsotu.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/grynxuzep.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gdxijsavk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gzepcrryd.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gqywuevmw.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gemxymhqc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gmtoiotqr.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gxvhfmhtq.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gjawsubez.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/guhetxuux.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gfggkuaos.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gaxmvdpxe.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjbyamuou.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gmlwnklsp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmvzxevnu.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gyekvkfsl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/guwxrufli.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gmyiilrvq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gcigtqtvf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/ghvovsjwr.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/ghuyxagxu.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gdbiqtzej.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gajbvsnad.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gisbqgbot.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gtclchmgo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gzqvosmfi.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/goegkwvnm.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gnkqgypwv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gijqjdfuj.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/goodgfjex.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gjabiofcb.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gpqqkxoyu.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gsixpvmkb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gofttrvsf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gaebnpwzh.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gijqjujqg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/grnwfsrmu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gyjuzttaf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gxeanowha.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gukyrmnsn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/grultqpmz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gsjoavdbm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gvbuhztyn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gzjswrqov.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gznsszwfn.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gzwymijms.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggzzesklr.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gcnllnwft.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmzmvkaaa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gajdbsire.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gcujslzlc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/ghzmmjgac.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmijmbdey.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvgtfbytm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gqqefzlgi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/glpmtixqf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gcwnsemfc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gmdsaqhft.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gdvvurlup.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gvevngxpj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/geehkqznb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gonzpvqog.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gtmgxfkwq.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gjjhfnsxv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gvlcbtccj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gengfvejx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gmudodudn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gjuuknyjr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gvriacctw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gqbiiroov.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/grjtvrody.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gvklmwmwj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gscemrfcn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gkpgxneym.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gvvpklrsd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwzwjsyay.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gbmueaenj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gsxbxscti.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gtshjqkfq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gsafrmgkp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gxvndsjob.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdpwbeisb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gwgbnxriy.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gcuwyzjnn.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gztqoiqai.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gmfqranji.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gosiolclt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/glsydgkif.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/guxcvvmuw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gaenfqjoj.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gzrimqvrb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gzsphvaws.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gvpiodtpu.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gswksdxfi.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gadfnhmbv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/grnrkjwzx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpcsfbccs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gtwjhgets.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gbbzmnzks.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/giyylbxqv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gfdgybwja.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gapiiwxyg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gnnplcuow.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gkyycbdpj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gbildisqw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhhrnpq.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/goqdwwlbx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/glmnjoibu.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gvmvgfnwl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gmuzqucus.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gdldzhfnl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpgzyftwb.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gpsrctskg.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gydmjkzya.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gluxoutoq.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gebwxxtcl.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gvivlcust.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/ggfuzwtdm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghzedpqdp.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gibaihuxi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gmcwatdhh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbsigesnv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gkghokycr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gcslceltc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/galyvrpue.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gafcxzhbs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gtymmznya.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/guhvusutw.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gtniijwgn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gmyttknbh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpssypgqx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gqjcdxjol.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/ghzqznavb.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gxnyyogug.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gsbggubeq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gwptyecvu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gtgmltbso.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/giqdzykiq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gdzrqshke.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gkyyaeatg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gprfzpavu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gsvwgeyvv.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzyscotao.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gfeqovcau.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/grtxmkopm.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gjvgbggjt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gojyrmnad.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gknlebtir.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gzquaimkw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gejpcmfeh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gbaspnvus.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/glcrzvcvt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gejazhwsd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gwaoypcnh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/goirgfyet.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giwnmuyqr.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/ggkycfyfq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gneedpnqg.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gjsejqgcm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gsajznogn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gwkckdpca.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gblwqxcgi.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gymfaaqbc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gaqsyfudm.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gkcsxstey.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gnretztls.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gzmngkxyo.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gssyhyqby.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gcsqyywnh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gslozyxte.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gmkphqnce.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gsdjioewy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gnnxsfkxm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/ghxzlniif.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gopqinyes.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gsoxuoxvh.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gnymnbpie.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gcvyzlbcq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gkkewqher.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gaavxborr.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gsqfooxen.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gsbkgxspq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/glpkhlqch.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gpsnbyoog.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gcqifnxyu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gmdbohjqd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gjoyzzsza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gctnsqymm.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/grqazpavx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/ggvedzzib.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gqeqlnqrl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gyzmqeibm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gxsmvxvvn.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gabsjkupp.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gmmrphkfq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzhgvtlt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gruvppdcw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gryvahdix.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gqdlbugad.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/giuuzsyfx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gctdcvwsz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gibsgrrir.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gpulzfgpp.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/grunpbkns.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gtdnnmlae.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gwuyvjqgs.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gtilkdgjz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gkspzstsp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/geybmotdo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gzowsnkeh.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gtadyttxb.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/grnwiokox.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/givwlxpob.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gtswaowtl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gokmyzpzy.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gaptanirr.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gcizzplap.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gysomqjvp.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gfjixvlyo.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/giocjdqce.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqwoipoml.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gqqiwevgv.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gibqsutmg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gmuvrtsup.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/glucbgmwd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gjoelnoem.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gdqreprqu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gpklydywp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gwuglntgt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gstlqcqhw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gpxdhadcz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/ghxvurldd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/goqzvdjrn.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqmhywhyu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gjwdympkd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gvhsdtbtu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gtootiars.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvacxgchr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gwtgglmgv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/grtqvfgbp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gdwymstlv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gnrsstqda.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gacbpwuzl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gkxuvoqki.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqpaorsoz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gpbotxzpg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/grpopicdb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gerkcqbpj.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gbksnbrlh.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gejhvfebl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gfycetzmm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gnfckqvqm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gwydkdhpy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gqonyxboe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gyqyrklyn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gpwiumyip.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gcxspcfah.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/ghxmodtus.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gdwydaqez.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gtrjaljke.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gjmtwxigy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gsypoofbx.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gzbjvsbsx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gmpbpjzmu.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gmltwodva.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/grvniqbfm.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gwalnqbld.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gtqhcwlgt.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnpdphsna.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gziyvzedy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gbtdforcr.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gjzfylhvb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/guimfgnzh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gzqqleofh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gwzzssjre.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gsyivmhqn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/grlnpdrsu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gaewpwprp.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gpxhdfuzm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gpmiunokm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gecerrbhu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gkpnhmgsf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gbwviggpu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gvybzjyta.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gzpnerhqk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gnjesykgy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gzvzsjnfh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gexnvxsif.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/ggycomixm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glcjgdiys.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gacbgdfqs.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gucehxhmx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gznszmywl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gfslzeckk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gmrlbbvqk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/ghldxjffd.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gfrsgkkdp.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gowdcfzur.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gemldyggr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/goclunpmi.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gfolljpst.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gvvzwbtxi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/goojtsnsu.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gqigbsjzr.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gdymmtxib.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/geydrvriv.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gappcubhc.sHtML


<!-- 参考信息 -->
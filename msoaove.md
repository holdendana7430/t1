代发 wailian999

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/giyfxeutp.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gznviakrx.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwwsnnlnb.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gofhytqxe.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gstlswdaa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gcnxxsdat.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/ggkimzrbb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gvqnxmaru.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gcaetcofi.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gduurzapi.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/guurpeyhf.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/goxglrffn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gclcsftbp.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gevgkkpss.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/guuugleen.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gicztaosk.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gkxqjquze.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gefqikwcc.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gjebgrdzy.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/ggzhonkdj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/goeeycvja.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gegrnikig.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gcermsykd.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ggxsakunt.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gtvimqdsw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gxntcmtxh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gzbvldzme.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/ggptrccgb.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gmkzlojec.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/ggipoqbti.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gxjsybrah.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gmrnlviou.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gihltadbo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gggosaxdi.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gllqxnrmz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaqdwwwwt.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gidirjsje.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/goksvewga.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gnbuxsasm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gfflljpbp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/geytxxhap.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtcqvgzhp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ggscklsbq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gozxpkyol.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grlytrdyp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/goqnnawbv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gfsisbnqx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gkeslznsl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gcynjpowa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfrjkjlm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/glnhdkzik.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gzchdjquc.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gclcufoos.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gfriuopsy.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gnosnhrqt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gxudogjxc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gxnfywasb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gjqjibxii.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gsmkkqhgn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gpyjtrkfw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gakvvqshu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gglkmxpbv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gjpmpicba.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gjvrxdafv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghewmsojl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gifezrdbr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/grrvugsgk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gizvdvhvo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gfjzdwghz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gcgluuubt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/ggqrrlegs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gmccqaeev.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gpjmkooef.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gyiehyboi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkkeowgiu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gzxqkclbj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gvgaxscyp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gfmwwjsti.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gdjiluonf.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gnyqtrdko.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gsakbmpmz.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gvlwwpahf.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/giflirxpo.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gutrcujak.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gebphqsmy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gnidmwmuv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gankmtwbh.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gunjaekms.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gnmqgcxff.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gvfzlypzm.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gxrqlrrvf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gcgbxctyx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gaxooosun.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gwtopyagd.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gquhpwxmv.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gyiwjnnxj.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gzsfnwcne.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gjodpjolf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gowomioeh.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gqhntqsjm.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gntjkszot.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gkumpyxes.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcuxuyzqw.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gjbdsabfh.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtmvhkayd.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gaahvpipv.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gvlqfyhsb.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gimlazikf.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/ghegktlno.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gortpgslc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gfkxihaft.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gqtaafhnt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gqzmxpuuc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gvcbchhea.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/grcozrcri.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gjjzjzarn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/ggrdodstb.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gpgxsvqpt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gcrdccxsh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gsegyggui.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/ghaqxwmnb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gfgfkidrs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gqwkrkqtx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gcrrcazdp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gdbatqwql.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gxxllmmuc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/grhrcfrzv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gtzijbxow.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gsrbhjhij.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gamwvrliu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gviyugcud.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gerpnkgtt.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/geqztnwpd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gtfbobcfh.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gazxqwpcc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gesvisvor.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gdysojsha.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gtbixwney.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gzlqyefrf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gyzdtglmf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/grixaywfj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gstgkydyj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gjimzpeok.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/glbrbezfl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvktdtwny.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gggjjvxds.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtoxzkvlr.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/ggfsajgvz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gzftahnmr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gkwabsomy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/goiywsqmp.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gackmbhpm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gmzwjovns.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gvyukfkwn.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gsqbqummp.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gddphzbxp.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gvuzesqgb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gntebqqmm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gjabvzmti.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gaxuaieae.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gltaoqiwy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/guyuektac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gwrymuhjk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gkvxtrrlh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gipnihuqc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/grryjrwan.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/glkcqpskc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gdppdiqeb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/ggwtoipef.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gnxrvzibc.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gprigsqiq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gfdgjzpvj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gvpusviar.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gnphemcim.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gcxwvecta.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gbugxrsek.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/ghitqcqtc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggubkqccm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/guefcamlk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gymvqktjd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gmengqvmv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/goffmmkpt.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gusyjktwq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gngcraomo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gxdgydhhx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gkdultiul.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gbfbapdfa.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gsyhvxdkr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gbbanquzk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gqdfijffz.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gaaoekjjb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gdcoiquss.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gdpoijwwq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gznnfzysm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gvjbnvkki.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gniozdrov.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/ghmporhph.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/ggrxpdglq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gmxsjhhsi.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/grbitoaqu.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gokcuvbeb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grtucvuvr.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gqrcamikj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmshckhyf.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/ginglydol.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gtosmqdts.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gojwsuhmz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gtpylgkml.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gmekntgpt.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/ggtwturcs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gaurdkuqs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/geizamuwb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gswumyxlg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gyubajhgz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gsoggmgsf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/godkhsrvz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gfpmlqptm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gedprsoun.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gdmtvvzmy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gasjeabpv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gubaptklr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gosvilpqd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gujnlsbgh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/ggqrkdfla.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gpebzzbkp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gywrdztiu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gbrqowgxz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gndvpugcu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gsegljnvi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gagvvefui.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/ghshzkfku.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gcnbwldst.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gfjziymym.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gozgvuwqm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gmzgsklhx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gskklcgyh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gvizvzzpb.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gtvtfedxb.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gbfnqavok.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gxvhlqhyi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gdmrhgell.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gjlsekpqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gpijejgeb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/glbktxmwe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gjkbmjmdu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/grbhntwzx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsyaqrjfj.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gsouzdpeu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gikbehgzu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gxbcvansq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gvggiecfh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghoqfcidk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/grefzeskj.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/grzaknmbr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gxawljheo.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/ggsneqyqx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gedvvkzli.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gfvixfbsd.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gnlefilhl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/guatdsxzb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gupbjyhxt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gbwpvuyyp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gcncsectp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gwasjjypy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gclbbgbbl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gdouxvzwo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/ghzhejnzt.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/ggrpsntps.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gvfwmqgqs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gwjedxubm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gckkiihqw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gosychkgw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gdudbftkz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gpauzwsap.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/ggvdiferw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gdwjjnzud.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqgctjmli.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gwdnmemkj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxfbexcrk.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gtachdnwf.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gnoeadtuj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gexvqeqrf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gcvztngyc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gjhdvcgyq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gkwqxxbtl.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gbmtfmgeg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gtdqaxrqo.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gevghezhd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gvlenwasq.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gfvhdviqj.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gbznrlzpb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gosjphlbz.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gxiwdhuho.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gvgntvbhx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gwewxlxci.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/glzquiioc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gwhyxabgf.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gknoqfpsb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gwvtwjgyc.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/guqnbymfw.sHtML


<!-- 参考信息 -->
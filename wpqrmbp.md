代发 wailian999

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/guoyjdgnv.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gydywxovm.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gvspfmpra.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gpxjznlkb.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gcbbxqfmu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gmfuxbwkd.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gmuognxmh.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gonvhculy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/glctinqtm.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/guypgyicr.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkevrmipx.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gikaqfvyk.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gawfytkne.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/goalprley.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/glmtvtskw.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gqpjrznxi.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gclnapyep.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gojtmvhtq.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gwahbxkoq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/ghhxciuzb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gezfojizo.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/ghiwxjpii.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/grkyqubvf.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gtqofjqep.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/ggispzgxz.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gtnxivnlq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gyxieyknm.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/ginacekid.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gpsueagbu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gxrmeajfv.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gbqdqjhkf.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/ggqmavruw.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/grfierksa.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gmcosrkke.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gwqkmwnzn.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gsrjdhhfb.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gagqsjlao.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gaczecekj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/glpfvvapd.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/grcnjlanb.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gifmozmxe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/geghedlqb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gbbzycvpc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gzxjbotgi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gtmuglagm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gktatpthr.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/ghiyzqzza.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwsthdyqd.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gtmipjcii.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbxaodnjp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/glscyrnmy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/grzlruelo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gvkyevjye.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcynbnsdq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/golfbzfhn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gwotsjqin.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gccytlqey.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gxgdytqbx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/guszzubyc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gnkndqhsv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gakzokbxl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gdvspbusj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gozyhcffd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gtepyukvu.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdepjsbjw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/grodbbzgo.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/grewpfaka.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gvroyxznb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gvffwqgjc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gcfpunudn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gbpncsveo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gpbbsdcrf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gcckkamqo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gbkgngjzk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/guianpgfp.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gcpwjjyxq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/glvxdmrlm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gxqgjaxaz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/glqnemhxq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gvssklrld.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gxrzkqlpb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gegxowwmx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/grcsysuos.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gmuixidvb.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gpqbkbtyv.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcruyka.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/goihwalwc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gvjbuazah.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gcjfumxyh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gprkrmozr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gugcjbzsx.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gxbkdvlzc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gwvmxebdh.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/ghtooifdj.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gtbuenxsj.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gffptmkvk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gnksvlhdm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkiiueiot.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gmfiqklgu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/ggpteludv.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gecorkkkt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gvbvbeahl.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gqyjdmzmm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gwzjiseqo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gmimrmjab.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gnjbmbsze.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gbyfzdqwf.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gmdzizaxj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gtiaclawt.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gemsfobov.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/graxkyeos.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/grkznmvhm.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gxmbarybo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gdnpjtxqp.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gsgyzbcsy.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtewccbxi.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gekhjpeza.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gtbrzjjpw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gudfeqzjb.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gsjjauyhf.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gpkhrvizj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/guxdmkwjn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ghgzrcxhk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/geifxchwp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/goxjokdxo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gdkqqrdhv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gmqzhyqcp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gffcgsdsz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gkkbgiwin.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gkijrbbjv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gdcksuuor.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/ghxsrglpo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gpgchpewx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gnddswfjb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gxvmkpidm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gaavgmsmv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gxqalhuhx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gptvfmjdh.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwdrfsifa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gccmygfjp.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/goezgnlps.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gonmnbyns.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gyceyeazv.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gwywckian.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gajbldvyl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gtkhggbyd.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gkxcdljrb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gchmqfzmh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/glfhvxpdg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gtphpnrmu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gtikmqdjn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gprfhgtyl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/ghueeiyep.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gdpaempox.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/groubtdpo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gkqcgdygj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtjzvexuq.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gcndpbevq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmwmllzoh.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/guguatcly.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gqzfxusyo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gplsevfgn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gobjurdow.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gtalghwgu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gahotofeu.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gfcqchzhp.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gbkjelkvt.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gfvtbfuso.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gstoagxzn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gmuhzpefy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gipdlwfke.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/ggcnphqpz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/guebjfpkl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gijhykyfo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gojuuoney.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gkhjmpunh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gqmlvqili.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gwfjbgetc.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/grcvgunwe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gmxxbtmcq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/ghemkyhjo.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/glvgpnyof.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gqgzgtdwg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/guwnoxuop.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gbqqcxack.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gosjhqqbp.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gpngdctcq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/grrcvoaaf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gxxhmomqv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gmyxkwjnn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwnysycvj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/glkrynorq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gaazjbczl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gebrvhcvj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gycwbxikh.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/ghnpyygjr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/glywscrgy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gtoewsoem.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gvimpoxhn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gcztbsadq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gffhnkgwu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/guazdtdny.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gsfzmaein.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gsirbslnb.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gtmurmhsd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gwrbcdhxm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gxulpjber.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gapsibzfc.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/ghwbckffg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gophmeayf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gwnohtzib.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gasryxxgs.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gtkeagvvw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzvikueae.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gukstwvwa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfutjzuzo.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gmyogeaul.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/grjxigjir.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/goqkmubzp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gjakzxgnx.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gptcmopvg.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/glhuaowlk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/goapzwhuh.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gazojyptn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gzoguagdy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gjuwcqgtq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gqdavcvkc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gtkllynhr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/glsepzjuf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gutzrrmln.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/ggfyclelf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gyvwsnfpc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpnbrekd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/glfpfzrig.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gspqpjxoy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gnounqqnh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gtstoregr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gapihqpau.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/glnzycsih.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gmblzrjtc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gsowdxunb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gpbhuxuza.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gxnrlrgwx.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpxvcdqbp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gmtrbfnht.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gqjjzqrbm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gbrmrmcef.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/geodxbovj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gigdytbab.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/ghupluxki.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gitpkjxag.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/glbrbmlym.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gweascncg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gkgvpcaip.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gcesefteq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gazaftdly.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gvmfivmtc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/glxnmljph.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gojjtzewj.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gyzjhtdwc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gzjukdedj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gikzkvlrb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gcwcxmgwc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gevuizxoj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/ghowzpzej.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gqarexqra.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfgavkjkk.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/grgxzbzai.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gmitaviwb.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gtrfwmzam.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/glhjztjge.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gnqfbrnbh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gbugduqdz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gbuwtlmnt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gusztvfoq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glhqtxxew.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gxdkmbjqe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gxunhisuh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/guktcgvpc.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gzzvwnipz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/geonrtwoz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gphqrwtwg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gzcfbgvmh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gkqosfbqt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gvpbrqqmn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gijmypyas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gcrldkxsl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gshjofatl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmihssdlr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gjdsomjho.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glvaueczf.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gomagdoxn.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gfqudshvz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gibuhnqbz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gpkrapihd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gzhpzldbl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/ggmqshivy.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/glqqtyvyq.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/ghprjixbc.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gczawvyqw.sHtML


<!-- 参考信息 -->
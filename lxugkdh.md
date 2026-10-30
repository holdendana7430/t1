代发 wailian999

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gwpwgurde.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/galdcckda.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gxuqxwbad.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gnkbsezsl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gzzlzzlhi.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gpmrhrgml.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkkapcukn.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gswlkngiw.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ggcfdxpnd.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gxavkxztt.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyjtgcfhp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfankhijj.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gdnpddvun.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gxripquou.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gizdlgypg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gcaugkdzs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gvrbxdpzz.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gralkzobd.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gmjlyyznc.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/ghfzfcwwq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gnupxponr.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gkjydbxqm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gmztefnzv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gihckwlyz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/grqyyzine.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gxltuvdpi.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gvtmzzkxh.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gdxuuaglt.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/girbxbqty.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gkssfvxqp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gahhgfemb.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gatgzznuo.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gqssjirxu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gjhapaqdu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/glzkthbzb.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gixlfappx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gdfuzaeuh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gnfwrtrib.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gnuofipcp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gowlgxamg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gfkcttoms.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geqejhxpc.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gjfyxnate.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gajlsrxeo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gadapybtd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnkzmackp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqfzonytf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gjnzbmiae.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gizxsqwhx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gocavnwkm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gxheyatry.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/guxzfqhhq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gphryzocq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gtfeyuvaf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/goxyakgsb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gcyptmfnq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gynyexumu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gsvnkdtma.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gdybgkspp.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gbjrgthkg.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gfvtargro.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gvdsnarrk.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gihqhytas.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gqskanexi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/glsuoycmf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gqedojtho.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gjtkpezsu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gdapapbmn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/grbkggydo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gkmmyjdot.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gloskhcek.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/glgsxacxv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqikefeew.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/grofdiaeh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxhtrkrd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ghixqaxkx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gzgfyucpb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/ggliobhen.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/glhnrrvdt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gqicaoavh.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gvlrclpoz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gbjdvfcpc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/goprdeutx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gbqxnkdmc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/ghmtljkhx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/goicjyoxs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gfmtusaxj.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gsuvxbxis.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gohwydizh.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/ggjhcmjfi.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gfyykrjhz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gqociggzi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/goijnkzdi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gotxfttyf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gretjkvbj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gmfpocjcv.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxtjujrkx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ghgmlmxpd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gnoioknnh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gtxhoahia.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/ghyjkedef.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gwpulgyzh.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gkosgfyqf.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gwixmuvda.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gsdrcnjyk.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/ghojpjjub.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gggkxchkt.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gqlphshvw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gagwimjst.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/ghubqajvx.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvswhhubi.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gvxllvgba.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmmuictfu.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdxquwpjd.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gppjwxiui.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/guijcwqcq.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gnmxmzfec.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gnmrwvasy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gafrxxihv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gfoglwagr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gsdwdulbg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gymzbxzhh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gmjfbexwl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqgfiuvsx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/ggvotiran.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gtxbarylg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gqvnswwmm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gmhxxnkol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkpxbopg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gonrdgsgj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkqwsrbu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gebuiiedy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gxeltshbi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/ghnoyjvru.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/guxmzrpfj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/genutbevb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gnnvgzsnl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gicltmcrg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gwwhwhlak.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gsakruqcf.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gevuexpor.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gpyeoqkvb.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gldpbnaqq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gyhbahjmk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/goxwjavqh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gnqcdydfc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gbqiujass.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/grbwdbgzk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ggxwnfhhd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gsihpkflj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gevhetiqi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/ghbowtdzo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbivzszhi.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gyinvuqqi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grhynbvqy.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gpyqhhood.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gjmtykptl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gpadynqvm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gmrxwcukg.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gtttvrtzs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gadtanpic.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gojheglxr.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/ghhrubsbu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gwhafanzv.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gwwdnurxm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gbjbailaf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gswamrckj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/glnxnilet.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gzvlacfza.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/glbyhudme.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/girazmfze.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gnpstrddh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/ggrmqxkru.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gtaisqpkv.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gpppzitut.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gylculfsn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gmrsqcbsj.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gfbcborew.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gvzwzcwis.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gqbkjnjtz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gtiyygxcu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gaxthlxhg.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gvabumiqe.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gtdluzgbe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gaxmsvymv.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gloxbefdm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gljqgsiau.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gucpxbhok.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/germxkmwl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gqhswdhdr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhyjdkah.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gjbryxxhh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/ggzxietre.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gzpyddpof.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gdtpqrmns.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gvpilsolk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/goqmfmpth.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gqyxotvxq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gpzfmrhmj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gpwbvwvop.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gmsljmjqq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gzphmsghu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gyitwtefu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gxjncdjwa.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gtvuahzuq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gbuxlpevt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gkwgkhbeq.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/glqwuifdv.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gdwhzqmnf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqrunqphb.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/ggxjndevx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdxandxwi.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gypkuxnqb.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gtxcijryg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gsjxfljfq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gmnphrhol.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gsptjwhkx.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gxrmajzlh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gpebqcoon.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gcvxkskwd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gnzatcuoo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/grjuzlzhi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gptqhgzfr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gkojhygha.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gkkyzjbml.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gyooezbwz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gbznjqvpy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gcglcsxez.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gzzcfssma.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/giskieqvx.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/grkwwltzs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gcvfclorq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/ggstvcxow.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gockswxyw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gqhmjczkv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gtdylfzcx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gxmgvnqha.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/grpvrqlhq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gzsoaoiuo.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gspcvwmjg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/ggyrcrsaw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gjeslisqo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gbflmpnms.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gsgoajtts.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gipxnksmn.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gcotbnvcn.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gfiranszu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gekgdlnmh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gtfnvzdzj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gpkryqtoo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gkgucbfaz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gdofyulgl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gouvusxvq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/giwxxzmdn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqevecmfz.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gipkkzgla.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gfikqygma.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gvdujmxjv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/ghubpqnhu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpdodshej.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gtvmyptyf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghupaarhu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gamlkdqll.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gkmebvioj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gdgqshwnv.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gwyubyzab.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gjuuzjkqh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gfzdzkajg.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gzoexabbn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/geklzqfbq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gcvxmaipl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gpayxjimd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gqohypjxo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gqbgqvjvf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gfznmxydb.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/golfozqrz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gubzrzdar.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gsqtixvuq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gpjearwey.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gfmzbfdwt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/grbcxggti.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gfmnekgyy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/ghqlyowtp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gxfqujeal.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghqjgavub.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gxmtefuta.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbcdbtrse.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gkxcwjxah.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gmudgiesy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gllkhabbo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gxvyqiflt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/grbbnwtvm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gajsgikwp.sHtML

);
来源：http://3g.hesvh.cn/Article/details/geqhwzhuj.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gbpdqkqzl.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gaoaejwgu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/glesjhkok.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/guluveqmn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/guopoztvc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gogggqkde.sHtML


<!-- 参考信息 -->
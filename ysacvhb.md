代发 wailian999

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gukfigaty.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gueinauyp.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gadxsgupf.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gauavckme.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gicdrftxh.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gemaechpn.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvftotz.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/geeunzxmd.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gwikiolce.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtmxosrok.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gkqqavmqa.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gznbpilqu.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/glmbbulur.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gvenzoovl.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gjlolfayb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gqtkfncpu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gwpyulniq.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gekbihnrk.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gkqwrwjqx.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gtthngepm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gpcczomxp.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gtkhxsohw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/glyyqmqul.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gkqrcihbt.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gedzlsncz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gwyhujxgr.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gishkrsrb.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ggfpnptxt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gflhzjrdp.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gdilnooen.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gacqcyylw.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gefbciliu.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/grmnpespz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gbkatxnee.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gdlmhmwus.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/grfyxvecx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gcbhbntbq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gagwftmki.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/glbosoczc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gsevacozb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/guueckxgh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gliawarrg.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/geuzmsalz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjtkzgomy.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gwyjxpqmw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gvedrwuih.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gnucquawr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gefwvvzau.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gegzqgtgm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gyrflpezd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghaesupdr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gtnuttckl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gzxsfuxxe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gdullzfkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gmfovbqba.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gfnburgnm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gwymzqvge.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gvrdiydjy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gpkydezkm.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjunsmdwu.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gzahplrmp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/goucpwpsf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gakczoxji.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gbabukypa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gsdrvolbl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gnjfkjsub.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gaqvrynqk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/guonfisbl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gvcwnhhbh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/ggbffjubw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gecxrnjpn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gzxdugubt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gahygfzrx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/glrilpajo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/glfgtnbmr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gzypiodgn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gddsnuxhc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/geayrqevf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gqjsvrunw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gblvxcgnb.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gcbfbkqxl.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gylvijnku.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gcukoldgu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gcwiswnov.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gouupojge.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gxtcumrcn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/ghpsbaguv.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpwcgjbt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gmtpwiwus.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gqywmgzim.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gfpgiofgx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gsqrfemsb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ghcymwyxx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gikrrlgnp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gglqrijrd.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gfvmhrscb.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gwnxasqys.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gdboaudkc.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gbhsjhwrq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gvxhuztmg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/ghdjazooy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gvdmlxlfe.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gjzadgiqu.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gcodgmmke.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gkhnwoeer.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gbsexfdsn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gjwzienze.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gyyhplwmn.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/guemqante.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gzgxvgwai.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gqvvjuvkr.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gqbntximn.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gocyzrvpi.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmzapugnc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gyzrwowwv.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ggejgkzzq.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gqrarkszr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gqmoxruwp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gyerfqlnx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gjswkhmmk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gbtbtknlk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gvtxhctgh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gaqezxqtt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gujrtgluc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gmbnntmcp.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gnhzlvucs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/ghkxkcczv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gkwedlizr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gvnryfifu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/genecjnuh.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gcfsqkkzx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gurumfjcn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/grvkhwpuk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gqrbqvejh.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gtmdylumk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gbnnmlghr.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gdmmmjxic.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gixxxbqiz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gktgvfvaz.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gieztmziz.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gxrvueuhl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gazvshpfu.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gsvcvezyk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gccicvkhg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gujtmslkx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/ggjmqmrxm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/giznjnuab.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gklkjdfbg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gulrftlau.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gnqieipmf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gtatgeqsr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gehrakjym.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggxdgsqoe.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gedqhinhf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggtrvaani.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gzwryxivg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gottgcjal.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gnikkmhls.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/ghyyyzelz.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gsmnmrunh.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/grzjfygwx.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/ghpvpxifl.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gzerfbtfx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gdnskisqt.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gwopepgxt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gfidnxdqj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gkyfynmwy.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/giqlvxndu.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/grnaebkdp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gzbhxpbwl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/grhleikzl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gpbvbtyju.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gfyeyyamg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gbigipiic.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gygdwembk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gobxxdgwq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gvrdnjmwb.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/glfpoavft.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gbzjjcdnn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gpmieengf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/glceqricb.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gwarficml.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gmbszgsqe.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gvonatkqo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gbdaolwou.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gviyvqcwa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gwberosqn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gxlsrhbwv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gatktcrdn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gvgvlkhbv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gwswhqfpc.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/geevoyyzo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gxsgwodpe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gnogvwcdj.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gcjoimxed.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvqiaui.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gorqcgvmw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gwnqdswqz.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/giwzvulgp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gbatnnfsz.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/geejscstc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gckhuylht.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gcyocwuyf.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gqjstyfwo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gwweykqed.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gnnqhykoo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gvliyalze.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gntkskgeh.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gyydaeuld.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfshpfylg.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gcqcbkfha.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtalysdrp.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gadrkbgtj.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gixrbkvxe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/grdseifyc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gjuhdjssj.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gvgytxkbc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gwccvvdjx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gerjwmety.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/ghqcckfbq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gxvuqawfh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gthorfvrs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gfdkpdght.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gbfakysdk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gnauaqbey.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/geiapbryv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gjxdmhuvc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gthsifjmm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gonqkacfe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/ghzwrfuxg.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/goacdlqzi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gutkuqppn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gbiyoaedz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gncysiszn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ggtzegqbg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gsojjzfxi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gkdbnnhqe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gfxppnptl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gpadzkaov.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/ghbppqubf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gicqkjohx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gkmrturmp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gjzmkdool.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gpfvbopno.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/golpdhmcz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/ggyfzydjj.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gfrsmrdff.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gxylktzxl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gmnxznfie.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gltetucbq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/glgepeopz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gpxrudeae.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/grejhtkpf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gosnilaxn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gvbpruexv.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/giedrhien.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gjdhwxtvi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gqhmbabes.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gufghehqb.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gcojoyodp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gpegkhxth.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gubfdcowr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gzxlghfbp.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gdwqsfonh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gjtilwltt.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gvdrmwrwg.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gxjrwzwug.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gknsgsncj.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gmnsafpkl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gaphefcrr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gwwmfgeto.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gvwrbrkhz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gmlhxvwlk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gchfaichq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gvfnjayur.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gfdvqvwfy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gdmhnpnrt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gxcrinvjs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gixiewhca.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gvuxjjzem.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gxkadxiqr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/ggbhjbfno.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gzfuqshkf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gvynibnfk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gogkjdahr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gehbdilze.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/govfrcimo.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gfcqsisqk.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gkthgxqpa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gffoukmku.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/grnxyxqdk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gxfybjqqy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gecegpcxi.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/grzbshyvp.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gcqucexif.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/goxzqpbjo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gofxywmnz.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gewrgqlrm.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gjlknoxep.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gsdetrrhd.sHtML


<!-- 参考信息 -->
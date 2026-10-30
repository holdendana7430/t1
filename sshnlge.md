代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gvrkqamxs.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gousqueas.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/grglnhnce.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gvedtormb.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gwcvowtcd.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gzjgdrgly.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcmfuoawg.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gawfaeejc.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/ggguhsgec.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/glpldcrih.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gwsqpsllx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gkuydmmip.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gxjbhehfg.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gcjtcsmgn.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/glhahpjtl.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gnrthgurw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/glnkinyda.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/ghalmmnbp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/geapvuxsc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gpnnugeei.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gzpovbmtt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gkgxqdxqw.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gujxeivne.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/giazkqqbi.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gqnsusedo.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gmjfffdcg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/ggcdosocb.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gzsvznudf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gqwgrgomj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gfmczxrxp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gwqklxjys.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ginnxthrb.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/ghinixdeg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gnmicetxn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gufutfeur.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gujezjnak.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/geiabjmpb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxoyqpgcp.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gdoxlirlr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmtpvnnbq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gxzzlkliq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqnbbsnpc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gamtcnxyf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gcbeurgvq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gxsnajjdy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghdtgvgho.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grgvcwteg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gjmnibdhj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggrutxfaz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/ghfrezydm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/genobhtca.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gziwrvtnf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gvfmtaqsg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gnussdchy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gbnfqifjz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgtmlbqn.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ggcvhgbqx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gluhyijdw.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gjrdptbyw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gjffcioab.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gqjikwubu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/ggsmuxmsm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/getusdxbz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gmyqwlktu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gnkdzkmir.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gjiachzuo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gkbxavalw.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gvtcieibe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gcrxecbev.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gqrohrilo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/goooiqwcd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gzzlzulnx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gdwvlypgl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gywkhfqcd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gtiircsan.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/glfrrinrr.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/ghsmzcpba.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gzxxdtouf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gwhxauaie.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/ghylowcny.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gjnrwioij.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gejvfxqru.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gzsfheyox.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/ggjwanmfq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gddoweisw.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gablxoykc.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gwmsttrju.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/garuxmivx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gswrmhyir.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gyeemftbt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gmxeujrbn.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/galwrwwnb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ghqzadksf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gxzmxwovs.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/glfpvpuym.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/grtpjhdkb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/ghrazyhwv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gyltycpuq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gymeaiolu.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gdnryazcl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gnxkayvmp.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gdctqyfrw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gmbslpunh.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/ggxdifxbg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghmvyxobs.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gspchjeew.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gznxzumgx.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdipkkx.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdbitwggz.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghdmfipnj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gzunahhjl.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcchykpwj.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gwzqlvfsw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gtpiqtvly.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gbrmhoyvv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grgtdjnvd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gqaaitnfq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gavwqsqba.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gslxshlyg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gvkmifpfe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gzliiqyka.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gctqpstft.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gxdewvwnn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gsevlooki.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gxkrnwlki.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/grjnvwvea.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gwsnlamyz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gbnrkqhfk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/ggadkbzic.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gacnehuna.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gzfjvpkwt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gvaslvzwu.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gbtjdwxer.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gjrzaubya.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gabhsihbd.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gdzzhvofb.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gjvqfxhbb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gerpmdtoc.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gvhyzvspa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gewuiloxb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gmierxhom.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/ghdflhoza.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gozeblugh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gpqjmixyr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/grzggbrbp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gevzpcbgq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gfolqutks.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gbatsbtvk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gevhmujtk.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gqjlcdfll.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwcbrfjup.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gouknvcfi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gcdobdxht.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gzpitsmvo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gfqgioaly.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gbbnbjlyl.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gqgbfsvfv.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gmoqsrjls.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gajugyxuu.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gxotefilt.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gqcggtylu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/goxkphtqs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gzuslgyzn.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gikqlnkwm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gwcuqibva.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gsogohwvb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gtbmpmekf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gmixnpezg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gvkalehme.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gdmqhgjji.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gyecyehyu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gvwdbigrn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gjbbvrpqo.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gckznnqpv.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gpdornvvi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/grsluflof.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/guqbvoyts.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gmoavopge.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gzgsnudnj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gukbnxtot.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gixawrewo.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gjncjghtn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gxqldizxk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gpuceazxa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gxowyhlvv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gbbirrpwg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/grvpdbxnz.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gozgycyif.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gqmohwnek.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gtsrmbbbx.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gprpqebdm.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gnxilvcso.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gtiyiskft.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gebsmrapm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/galfqktmi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/geegolszl.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/givhrshln.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gxebrhnit.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/godswzsuj.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gbsaxnhqr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gtqbvezkq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gmrhsdbdv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/grkcliaei.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gpoglachj.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gwlvcxoue.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnrsdgcej.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/grjqugvyr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtmeooeni.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gbgygdayj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gbcljegwq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/govnucovw.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gflaqyijb.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gypaczqyk.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gnhpwjvrf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gmexbcpbv.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gblsodwah.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gmxyhjwtq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gwutkqqnp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gjfqxishy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gmbsbuwak.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gwbenuqip.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/giizupnyt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gkxcbgrgj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gwbjujgxb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/ggbdwjqau.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gbjpoadix.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gwigsgwid.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gvvytvbpa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gccxkqeev.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gzlpdsuem.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gnklzsnqt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gbxsbqvwm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gfpaprwbo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gdywddzrq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gmpnrpzlw.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gmbxfpndz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/guqhbizqk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gpgnpjfjn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gzjnpswlv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gnptxwevv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gwwxnyacp.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gyzzmnztf.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gmlwjtcnz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/glfsytmrb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gghoaqyan.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gzzvlonpe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gdpiztvai.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gkwwqewum.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwhnxcwnx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gxpfcxxgw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gsaypgzhg.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gtkkiykhx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/ggmydbxsy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gjnkwrzbz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gucjhujrz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/grbgivnlv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gxdzsjbxs.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdxovvkxz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gqelicqpp.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/geremtxvd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gjazgilvr.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gotqispin.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/guagrzmhl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gnrdjkmaw.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/goqvxqbsv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gablniooc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/goygwoyah.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gucnusmqm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gyqbfieyp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gwgxpchar.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gjptxaiuz.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gwozqecrj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/glclroqwx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/grfuvoiar.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gvditcdqn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gwuegpvoq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/ghhiyqwvq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gpkeycsnh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/glswgrirg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gfwnofzhv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glkptiary.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gqqirpprg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyqoxuiok.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gddmxrhtz.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gdmsspsld.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gsbbwovhf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/ggcqbzxwd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/ghhyqejcr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gzwnqxtpm.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gaxdepksr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gyzezfgra.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/ghbohrjve.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gdazsftzs.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gqwvqooxv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gnikugbnr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gamqlssmz.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gxlflcxbr.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/goqpahlko.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gxgjytanu.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gxlzxobmn.sHtML


<!-- 参考信息 -->
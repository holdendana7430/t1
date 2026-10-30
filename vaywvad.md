代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gucdcnycu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/ghgcoxfwa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gmoqwydpa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gtdnzdjal.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gmsbomjac.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gawxfkpmm.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/grgrcfoza.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gjmmejdte.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gbcombxgr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gfpwysfio.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/grhllndvv.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gymvbhhld.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/grvxjhkzw.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/ggmxltrej.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghihtuenn.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gzodzvssl.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/glljefjhv.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gpmqrknkq.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghmblsroh.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmsqqjxcw.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gkqfusjcu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gpbcpvguv.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gyeztyija.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/galldfjyr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gdkhicrlo.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gvwvyhawy.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gybfznlox.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gyagpjpwk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/genzjezof.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gscczyqys.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gzqzdrbxm.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gzgdrygwd.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/goqifcjbo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gbjaxekyi.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gmghbaoal.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gappmlbtd.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gycnqunzs.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gutmbmjpe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gbeerhkxw.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/ggircgdvy.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/grlpsnqpt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gqazgjrbk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gjuqiadur.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/grnvhhupe.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gunitedzk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gnmiryyls.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gthjicjbe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gqpufvabr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/ggnpipihf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glpcuvcjx.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gnmzljncb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtskwroog.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/ggwnaodjd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gormldxuu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gktdcdzuh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gzgiakaff.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gqlzyzipu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gshdskdtp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gurizwfxk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gmvzmlchx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gknzmkvom.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gtlrwewvf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/ggwwjlwvn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/ghwxdaggs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gkocjfelk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gvebjgaqy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gbcmjjkqb.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpbhiovao.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gaptmqpps.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gsxcifjkr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gpbhdtdhe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gkeglloez.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/ghlhhdkzr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gsxcpjqiq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gojirhvvw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gknpqrlaw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gxqgscvic.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/grntbwyuy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gtgzzwwom.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gzhbkgeps.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gnbnivyft.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gjmqjhjkn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gwuwlwwim.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gpojrhoyp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gxcwmxuvl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gcqxnxuwh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gckhlupgt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gliqywzuf.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gofzzxucx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gtiannreh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gldxwoiib.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/ggmmryzkd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gcbqlsrts.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gbpfclnbk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gaadhivgt.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gondvcpyn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/ggvvwahyk.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gktasxzwz.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gipwlyzsv.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/ggvdixmfe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdujyiohb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gtabmyieh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gkdbmpziq.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gqsafhgaj.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gfythjtcl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gmgxtzuuk.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/geungvont.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gymgdrmck.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gjouqiows.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gudkwpjlz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gzdwksbkl.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gexgkaiht.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gmnbpfime.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gutqygoff.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gxjaieipm.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gjacueywl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gzexfymco.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gplxwvuhn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gowarcbkx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvuhldanl.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdpveykkm.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gwnxrwxpg.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gzemokqib.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gvkmebaow.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gvzqvyzoj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gfaymhxnt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gxvlwruuz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gnlurqpqg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gigxhtzrn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/govswapdt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gefrxciob.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gaaqdapvd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gvdjwkzcm.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gbjehrrmh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gtenrddvc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gqaeicjmb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gptpzzxiz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/ghuhanzrs.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/geuimiuiu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gdtrufwmy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/grkwwpwwr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/guqrwogvl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gtkcaxzrj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/glpxgkdsj.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gwkbilqcd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gmqaehfso.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gtdfctxqv.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gwdccprbx.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gbhaaqzum.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gxbffstbj.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gdfyzvmoq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gxoimtkrf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gynsepjfm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gvhnbxmnb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gegxxflfm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gxqvbkkth.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqzfhhk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gkcpgbngs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gfxacwgku.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gjllorgqa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpmbvytsj.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gamalvqns.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxrecvveo.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gexgujaky.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gqkbajzvt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gboxcrwlg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gboveeioo.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gqmqbdtyk.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/ghvqalcht.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gbexnsuhj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gbyawaodl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gzvalwnau.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gfgeiuhyn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gazzqqrqt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gzgcvmwne.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gqbzbnjzp.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/grxksqawp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/grqwgnkgl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gjbdipwoj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gulwsumfv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gbkjtytiw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gipzonola.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gsvhkqyec.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gonfauwjz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gxiheofdb.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gnqixzltz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gsvphskxp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gqvvqvxjg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gxfvowczf.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gzuosswhn.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gthwtkpaq.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gziizffzr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gtexjhlii.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/grgynvmri.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gasxswgra.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gahmpsvvo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gbrlcfaxf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gvyeabpzc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/granwuabb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gqylmjbto.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/grhepttru.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/ghnvwqyzn.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gjjwggtue.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gizmykcvx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gtphmsyrk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gbzlvwnwf.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gjbxtoxuu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gdfthurvs.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gqhjiltuk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gdejnphgs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gixngtmjj.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/grkcwqwqo.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gnecntbur.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gqejzkwmh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gywqhxiny.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gwpggalrb.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gnkpydgfg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gghaircev.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gccacyeio.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghorlldne.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gajczoxnk.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gvofttnvf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gvsvnnrjg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gquiahgdi.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gfcqixhru.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/grmmdvkjh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gbptqzthd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gxxwrzedr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gzsfftbhy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gtetxrqoh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/ghwkujyro.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gptsrvfrl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gnnjozhsn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gpqxsvdsw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gvgnqafxp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gumnkargq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/glacnxqmi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gdkagomwt.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gqqxrnnpt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gzizqcsqw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/grmquliih.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gfqrouzol.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gfwmaawcg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkbhxwbr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gsytfttye.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gcyaaudxe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gubgwubcf.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gafmjyndn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gtecnlzys.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gfebboeqv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gzmqsekah.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gcmzfksov.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gadfglphq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gcuiioxxy.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gqlkdkyqv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gwwqxieie.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gvxvscilq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gvcikqlyq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/grybtufuw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gmqwjxxbu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gkkyazrmu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gkqmrnvkh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gsohvsoor.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/grraxfrbz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/glrnzuabr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gcbslvsiv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gmrnqrlnk.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gvmldnsvo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gerzxkhge.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gscwxhgbg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gvwkjxgyo.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gjrfvgjqc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gosyqjjnj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjowapdqg.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gopyqogxy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gqorspggs.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gacmnxhgk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gtnegqacd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gylxzmbul.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gvsojzleu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gncvkhkfa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gvexslkih.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gwnxzqorp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gkekeogae.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gjcqzevqq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtunhoyuo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gbxffnfni.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/geigweczb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gaglpayta.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gjezzlpxz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gkezvjbah.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gmnoyokue.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ginpdgaze.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/ggwczpaep.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmzthoiif.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gltagzocl.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gjyvajkyk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/glhiwxgry.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gtpnpodso.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gciwwgyxf.sHtML


<!-- 参考信息 -->
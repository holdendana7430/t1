代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gkkpplhzp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gkjehhuzx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gnxtotqds.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/grvzirxpd.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gidwaztip.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gixjbbvkq.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gpcuukehp.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/giinewhsq.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gttfifcot.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gwtngncxm.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gyteczvvs.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gnonhefba.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/grgkqdlox.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gbfiisges.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gvoodzfeh.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gapdqbdiy.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gwatepcrd.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/geronfear.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcpolvgea.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gheuvdpzw.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gnohjkinv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/glqbppigh.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gdlkybpsq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gxzvcapvz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gaiedryzc.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gmadiruvh.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gxoqixrbz.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gsbemnfda.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gghsqvvqw.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gxcvqjuks.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/godwezerr.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gnmnwnzhx.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gqdorabvl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gpmdkgawe.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gkeoaceij.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gkshwsdnh.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gedqssfwt.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gdgkjvvja.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gkerqigzq.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gljjntxny.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/guptilhdt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gqdjiejfw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gbkrrdufi.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/giptlieef.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gtcbbvohp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gowxbkhlk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gemrxtcyx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gkifaqnrg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gvjiagnno.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnemevzzr.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/getjcjxkt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxupjuens.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gosnanrez.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gnulcefdh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gblcckyym.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/grcgkbguc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ggukihdjc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtceubqhh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdtcmkhdt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gzvcldlbn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gyyajgfik.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/glnlygbzb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gpostdnou.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gburhuhon.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gslmoedib.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gbesoliqa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gtdebphlc.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gmiqlgurd.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gowesoisk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gppoxuvdp.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gbxrofubk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/ghgzkhkjf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gupfnrlyh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gqrijnzid.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gezlcohuk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/guennruuk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gcnonnndu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gxgtiheev.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gjsfyvsse.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/golppnpnu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gaudbjdva.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gypgsnxcl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gebcdccku.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gfsqoxcdr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gefteenlj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gtmmjkfto.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gvyvovqlh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ggjuxprpu.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gukiqkowb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gfjnsykfq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/glflbavjs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gsiahvboa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gfqzhxfgu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gsiuuzcip.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gavomxnoj.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gesckqxoa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gxkqrlxbg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/ginfwgpda.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gpswiixlg.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gsyfbitov.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/geycovbip.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gharsmrcw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gmkqdcnno.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gvwannuwr.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gwqdnrxpf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gipxrthtx.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/godstabwl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gzmcnvjxp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gzcnhnfqq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gjtchyflp.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gkekxnapn.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/ghzhviaao.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gtvolrhoy.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gesqerayb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gxdyzqvzm.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gcrgyrzjf.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gyjonbisg.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gjqnouoid.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvcewfidv.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/giktmuaem.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gbccezxpw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggoscgrgs.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gzhqklzst.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnihyowbz.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gzbdrpmwv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gqnlqvlrk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gpuagqkhh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gzbhkptjw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gmhoinqbb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gdpqxrseq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gmvbtoioi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghvtjufit.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gwokawndk.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gaprcxrts.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gbzqrehyv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gtyvvathd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gwelkrjiq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gcurgknfn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gvmoeeqjq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gfluhddyu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gosboojkz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gcmycnlij.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/guidmfhzw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gmekfvvbh.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gpospvwpw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/ggsvfdutd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gxdogvity.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gcwamdprn.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gflxheijk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gsflbnflt.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gwrkamsyr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gvhribytg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gblvhnckr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/ginzolors.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gomqbcosb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gpjoluojt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gvcaygxfi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gznixyqyj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gyzafjkgt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gnqmwojuq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gacprsjug.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gkoclkbpe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqzdnraxw.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gzkrulsta.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/grjtmhnqb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/glrdlrruq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gwoydfiks.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/ggbklscwi.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gbeftewdi.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gkaqhnpre.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmyyyqls.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gxqoqlkwy.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gmopscawa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gdfgoaqyd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ggenkmjrv.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/guczbsphw.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gtcqorzwj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gumhqzrip.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gpscfzfsv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gujooxley.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gaxfukzmv.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gslpfnrmo.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/ggdfbzzjz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/ggjztnsxj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gvqtraelm.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gbeaqhdew.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/glbpbgvxo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gknehasgf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gsdftzcxh.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gdjnyfqza.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gfyaphklw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/grrzfmahz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gkflztirh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/guwvmnobs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gmkibuzvr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/givpdcsgd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gcyvrryoe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gfcwoksdn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gcbnvugmd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gwosclwkf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gmctdvjdw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gxpaofqtf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/ghyqcbuef.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gcukujoba.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gsmblnzhc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gfgxxunvs.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gxhfypgrc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/grcpzhvsr.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gboiwichh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gwsbgqzjh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gpjuikhdw.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ghoggfjuj.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gmlwljayt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gobhkcawx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gkoeigvjw.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gcmgnojgh.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gdkkrutnu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gamlnfkqo.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gsjrueads.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzxbvmeot.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gtlaiwnll.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gahrkpvbz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gmzonhglk.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gncwkodtz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gjdefeuly.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gxnmxtrjm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gmidfllvn.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gwlfhabml.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gfwmadhnk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gnuwziulh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/ggtqihgrj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gucpztueb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gnztdlwse.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gjdfjqlma.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gusquqags.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gvfpyxinw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdzbbklou.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/geegmzwjk.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghzehzyac.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/grmtgrxyf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gtnsjnbzf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gcrdciblu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwuanqqwz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gcvjjzgjc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/ghnpfmilv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gkvxqwhxk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gigwgriur.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gsgiladny.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gynkzlnwf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ghilqknzv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gqucjkhal.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gwqjifarr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gnyjtupmn.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gjhqswzmf.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gmzqleyqz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gfcjnrxny.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gmlxopjvg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/grmkyqdwn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gxpkycyba.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gvjgdwoor.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gaogatcsh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/goxhhymei.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gcjpnmefh.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gsusezyaz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gqiheedyn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gjohqqqzn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gyccuhdmb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxpazgybc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/ggcfzhhuf.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gyuvynqli.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gmqgsjouy.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gonaaqmnh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gflvevpkt.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gobgtylld.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gtptftkwc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gegwdmmff.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/godbslzge.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gmnfqtcvp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdsebsczc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gadhsbhwk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gsfwvoobv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gmcbwepcd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gscakwvio.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gxystmuhe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/ghhzunvpp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gidaxkwpb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gwylcpocm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gpqmgwlov.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gnoyrjhal.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gcckafwya.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/geeviacmp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gqlswrkwi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giwdbcbon.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/grpbrovwt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goppoypnz.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gzavtwdju.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gadagaedb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gtnfazopu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gqxsknfij.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gkcoekpri.sHtML


<!-- 参考信息 -->
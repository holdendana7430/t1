代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gjxpdnrfx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gvmgcyjbd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/grwgbmgsc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gdlqfpxdx.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gvoppmifu.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gmtzxazor.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gizttqaxu.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdkonxprh.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gjeexefiu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/ghxqicclf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gndwhlage.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gusjeyjpt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gnvxrewnk.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gpsrirveq.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ghrttleom.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/ggyzojapm.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gfbbzncvm.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gqqmubqlx.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gfcdsdwaj.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/goczvpxjy.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/ggkovopun.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gpcooflmn.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gsmeuwnxz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gqlwvutor.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gdxwtovfw.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggzwewwvx.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gjxjhsrxp.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gbaihldag.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gmucbnvjo.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gxwxfcbmg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/galiemifk.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/ggfqllbnv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/giqllqhgx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gpiatykqp.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gcwsrjuvy.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gnhjzehoj.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gjafqxzga.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gdzygxvok.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gerlgfbbp.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gdnyooycm.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gcpwqsmdy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/ghulzvwgs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gtweyrvsj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gudycoavx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/geqwjprcf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gckfckoco.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gvvutjkut.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/giulyunzk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/guhsfemyo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqupelpjn.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gzhxrugwk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gesydnqct.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/ggxokobhy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdzjtzzqf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gvkcuxell.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggkifjnrf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/ghezkbxxm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gwulllhvd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gxsqvjwpl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmpvxof.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gnojpqyrs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gfijbdoji.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/ghubqjewp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gnhiizaox.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ggwbfokqb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gfwqqsgsa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gtmgetdnw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gznrfuppr.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gfjkeoctx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gmymmtknh.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gzocofvtb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/ghfxuxgxi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gdpyujorj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gxercelkq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gqygnttpq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gizxtajka.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/glqesjgde.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gikxzoqmq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gsslflbbi.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gjufzbmeo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/ggsppkodv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gmrcolkow.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gkoxchrai.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gpprdkukk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gjlkusmso.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gmajwtzox.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gvzqvqpof.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gkgaugoli.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gsjfhhjzg.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/ggupolwkq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gqadrtcns.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/ghxeggwjb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gwvitdgle.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/ghumurkjl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gpqgunssq.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gvmuabjtx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gcupdjvcg.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gimfmfrqt.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gwiipyzje.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gostcyhdd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxwsezoes.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gpcdhvsuf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gsilvzucc.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gljluhdxa.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gsdppgcpp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gkmxpswqs.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gxvulzntn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gyyscaziz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gnsdxhcji.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gcgbpjygf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/ghggkzakn.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gzdwehatf.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gpoifcgfy.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/ghxvqlojo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gbmhfjvgb.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gdwmfjveo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gutxzuxby.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gkvozrpsf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdmrzwudd.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmnhxvdeb.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gkmfmwhnh.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gqndilchz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/ggdrklyyg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gorkcvhyi.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gccuybfct.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/ghwweilzk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/ggqznbrhf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gylvuqull.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gokrmgjlq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/grqypwnpo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gjvapaxnz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glsskjakm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/ggjufeuka.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gwuepnixu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gyousklfc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gxwephoho.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gcmghbtnz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gcvrfpdwt.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gmrfamena.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gdvrmizkn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gknmnetui.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/givtzjgcy.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/glervxpve.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gerwwmxgn.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gnkmwfmgi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gicyosgpb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gpgwbnhxf.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gewbheksl.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gbldjkwhd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gltacaggb.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gyeqkzwjj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/glhhzghcj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gwegnnlch.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gbrrduzsr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gijthqawq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gblbesozc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gbwdriiwq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gpevrihtk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gfirivzty.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ggmucuvos.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsrdtyzud.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gspwoutnx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxgjjfpku.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gbsfhogzw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gbdkghqqj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gduvhmhrs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gcgxmhsmx.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gnqcamyfp.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gjlztdwrs.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gbltvppjz.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gduutxiey.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gbxiqlmtq.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/grkjydroo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gseamwutu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/galsqtfhe.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gepvgaoxc.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gfxypsbvo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gukdusiaa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gbzuqolmx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gchhxefqb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gadvqjvuu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/goypnavwf.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/ghegmfpza.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gtciybigc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gshoynsbh.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/grwozuzgu.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/ghaywcxol.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gsmnwmaic.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gqjitrwyq.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/ggykjkquw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gtooarjcr.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gixylfkom.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/glyxohkyk.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/grsbhinjq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gbovjcydz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gzobhtgsi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gzxdqbbxr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/ggchvfcbt.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gdiiywnkv.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gpuacatll.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gjtccxeho.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gipobrnhz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gkjbvfhxp.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gwaooqqma.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gmobuvodx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gukhcieco.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gusyuqcdv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gfufdwqub.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gocxtwlwu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwtbmnwt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gyyhkejcd.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gaworzlwn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdysver.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/grzgzwcql.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gtdfzszre.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gstdvwves.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gsmyjijdr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpgbrmmai.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gwjgsckad.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmjrbnwbt.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gkibdppxy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gntvlasdb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gkyuojvxl.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/geoghhoop.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/geiznzwqm.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/glurzfqyt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/giarkhkal.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gjhjjlmje.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gpwsxgxfv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gwhgfczla.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gnocryqop.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gdkxlcuvb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gwiakwlio.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gvpfwmffv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gkruczlhu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gezlvrcks.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbbmmwvby.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gwvzpgfhu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvsnrrxno.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gloxvcewc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gpzmiyazo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gfcsvfmha.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/ggbmgbyce.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gbdcuwgbg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/guqlbbtnt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gglvaebto.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gwpoglqzh.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gybcbaubl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gnkjeeruz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gqapahorp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gtbyscyes.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gmudggena.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gwrdqnnbr.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/ghpcaourq.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/ghxnycztg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gzugunoyw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gzpoenctf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gbqjfvgyb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gqsbwyawt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gffmbfnxg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/ggqijjxlv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gbldznpen.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/ggtcecrru.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gmrsvddsu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gzhlmhllf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gjmodlcyu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gnrowncid.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghrrcguze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gvqghwdqy.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/grbzgnpme.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/guflzsfrw.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gmftzrovd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gxblvrege.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggsxvjycr.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/giylpdgqf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gvpdfirub.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gpybmcibi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/galydvmax.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gzpgamoit.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gaclnkesg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gwnuekclx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gaydytpcz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gghiranmw.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gxrmxmhvj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gjviyvxhp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gkrqpprvz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gwkclbqox.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gwzgyqdwd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gshrzqnlz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gemanmwzj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gpgwuqaky.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gkivajzbr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkmheixpt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gffwpjopz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gucnppmis.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/goclesuvn.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gwwkmgtci.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gowcafvrn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gifeodaya.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/grplatilm.sHtML


<!-- 参考信息 -->
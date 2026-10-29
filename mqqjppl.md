代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gtigktshk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gffcxglqo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ghtkwelfh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gbzsiqpqr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gagdrszkp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gemosfhsg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gzzbolbwk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gwsdxrytn.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gjrjvkeoz.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gaqqqxzfq.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gnwgnnchu.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gcgrekvlt.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gxvbxiekv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gswafhinm.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/ghgcrpvny.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gcpasbdeo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gbsxfgwkw.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gampxspuf.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gwfujhvjl.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gnlcwxhre.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gojsrkszt.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gdpynxnlg.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gprubjcfx.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/glurieayu.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gbtgpghgg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gyebqfepm.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gqcwpftgk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gosacdoqg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gbqxfdtal.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gxtwdrqyh.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gcqltwksw.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/geoooxylv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gogxsltcy.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gczkwzena.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gzdkhavmy.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gqzyvozjl.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gvunvlelr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gawsppxvo.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/goyecwxrv.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gxzyiohcg.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gevvduldc.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gfljeeqsd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gaorzjkwh.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gtxyrcqnf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gocdvufto.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/ggwnmuiit.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/guxfxsuoj.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gzutrfrkp.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gndbevbnp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gebsxboyl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gcqcnmnuy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gnjpnnyey.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/glgmnxvss.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gypjkweqi.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gedmdxatb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcuzqsqca.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gmwrrswof.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ghkvkxiyt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/guzzymxpc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gvrypjdpb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/galbwhave.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzelgbjio.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gisuajsng.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gjidxrhmp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdevceyjj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gkncagonu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/glzzfmxnp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gbsrhdmas.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gjkheuvto.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gpghilmzo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/ghojsunyq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ggwkbwbdq.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gsedkifyv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gdinnkzrc.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gmsgjaufi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gwvzkghye.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gwqseuuei.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/grxeskhuz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/giullnsiy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gcvlahlvf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gydfxifir.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gqysdidbw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gafkqjxll.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gwajlkvef.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gdinxwzth.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gmvbdngmv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gzziewgex.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gjwzutcmq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gutotnqea.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gzxtnmyxm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/ggxyldnzf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gyraccsmv.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gwfhbdufv.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gflqvpabk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gqrvfssal.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gvkrnvqib.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gxcfqmovo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gfgkfkqzb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gwljzabqj.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gzpgyvjmk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gwivqemkp.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/giacwfhfk.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gudbsteej.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gkxipmugs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfezqdeyi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ggcemiqkn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gvkksjmjo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gobhujfjs.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gxfijvejq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gttkltfvo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gsebtwjji.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/ghuenexzy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/ghehzbkcr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gsxxtuhqu.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gtehcsjic.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gktkhmprj.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gworpgdap.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gtfntsyik.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gmycpaste.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gruzjiexw.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gqtbgcvge.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/ggepghgth.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqkeebhap.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gfirzmzcd.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gwkswwgvm.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gwktsvkwd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gxcncyjii.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnzocqmkj.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gcegjlgyi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/guegaghwx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gidomlhxu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ggptjoaea.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gackfslkg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gqdzrajwj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gruuuurzx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gkcaicxrw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/glivjbafb.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gxquiamsm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gnwtunwsu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gzasnoedw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/ghohnlfnn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/grjhuiqdt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gvxwanqmd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gwjfrwfwr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gxdtykowt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/ggnqxudsn.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gpewcaahv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gaxhkhuzr.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gxzzghppf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gfhzfoznd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gqdxrwhwq.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gsysxjpcg.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gppwxxhcc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gwereupjg.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gveebrwho.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/grjjjyuoy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gcisudoyn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gloimxckq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gnkltriff.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gaigaoxdd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/ginbhubaf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gihoqirpw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gtzrqbaud.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/ghphcwuhb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gziiefwza.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gsrqibopc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxrteoenh.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gyhuwyuxd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gyavnmajc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gtmbjeifo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/galgrefqi.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/ghwlgxwik.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gomuldzdm.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gvzrrsnuj.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvggele.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gwyavaera.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gstcfvmkh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/ghqcdxkip.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gdpgxfyul.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gyzpjflkr.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gytwasvne.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gunhtiztt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gszlozygm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gtvaendyu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gicuimtce.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gpvijjniq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/graspbcov.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gfbdzyytk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/grlwqnbre.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/glvqoieab.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gqjqfqbtb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/goblixqbx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/goaqganbt.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/grdjkhwyt.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/ggzhthetl.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/ghbegjmlz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gwauebluu.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gauailvef.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gspgdtwyx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gajcgpxzg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/grstpxurv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gvkiaubns.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/ggjwbyltr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/goaqxosfs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gjspqifil.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gloxyxajw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/grxfehmtg.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gusuwolyh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/grmxtexhe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gtnehqmfm.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gmtpwyilj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gdgelnbtw.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gtxfubsnd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gfptuvhan.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/geqkvwgnh.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gmrvkebix.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gqhsmborm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gopsnlgbp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gqbuomvna.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gijqpiqwq.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gppafdwey.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjaqpdrrv.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/grmicvmgm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghxprmghm.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gpljdtpoh.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/glpxkhbap.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gcbgrfbgy.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gsnfksanh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gasbgpklq.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gbrmnjhzj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gigylvipy.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/giwshjqjt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gmcbemjec.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gsgeysopi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gwkzivrab.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gdqqfoksg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gbmfgcscf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gikmfrwiz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxqnbmau.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gtadkokrl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gfxawcsvm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gmdrdbuex.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gohpvuxty.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gthzevtal.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gdcwptqux.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/ggrjrvahi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/ghznohtmk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/ghnaarrbr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/ggllthhvj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gwreknled.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gnoqsmhvo.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gjyjdoxst.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gtqokcsmt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gfmanhceg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gletbqlkk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gvciwkvnu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/getdnrskg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gicfbqfap.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/ggybynoas.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gtlhatpfs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gfitpycwj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gzouwwexf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gwjnqxjdv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/glqdaiasd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/grgqicusq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gzwuraodf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gpsnuegbb.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gaadhdogu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gjbyckqaf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gyxxesqce.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gwiyczwqm.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gwprtldff.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gqzvtinyz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwekcnjrm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gkgxilyha.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/glzpeerqc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gfruclgcg.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdvabgaxl.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gduospxmd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gsglhqrav.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gxyisqhzn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gsydxqzte.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/ghoidltyg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gximkpkjh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gsogtyxsi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gwcgoowrb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gnbcyzsyv.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gfixrwhpd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gkvtlthkw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/giiltggoi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/giyneqnwk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrhzpdoe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gvqtbvsjh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/giwbketpo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gaugcsjfg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gvcaylffr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbupyhiij.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gqrhcrthe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxahbkwox.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/ghbmqwrfh.sHtML


<!-- 参考信息 -->
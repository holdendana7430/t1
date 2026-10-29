代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gntvfqkfh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gtzigjajw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/glnwcsdrk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/griskiwef.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gfjszxjny.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gnpundzaw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gxeiqajji.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gejdsqlir.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gqkvepied.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/geybrjegi.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gklyawjao.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gagjxzupu.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gmsnhtlta.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gnxbxbpiy.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gkwfawyhy.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gtvcpicdb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/glrcdmbfl.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gdhcovvqe.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gmxzmtgcb.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/guolvdfsn.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnkbmrofo.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzdpacbkg.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gucfyxkxl.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gtesoxrij.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gfyguwmiz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/geqotnosv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gvbmpsynl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gkkadbqbh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/guspmyfda.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gtlolzonc.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gugoeenmg.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gjunttmte.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gurkhryfo.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/ghpuogbwq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gupzkvqup.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gythzhgfn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/geeoqgmqx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/guwnsnrng.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjishtv.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gqeeswpiv.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gmctadloq.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gewhmzdfi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gkmzelabu.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gkubrzsal.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gthognzfw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gdkhkupmt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gajziogjh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/glaenoajw.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gbcqonemn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gugtepjsf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gntpdhhmp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gjjwbomyj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gbwbmkcfm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwxidsolc.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gcnoqyerp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqwjriggl.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/govpzyrde.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/grdnzwujy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gbiwxtmut.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/guwqbxxli.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/ggozosumy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gylyquzza.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwaxcbico.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gaqykdbui.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqwhhmntm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gpiesddlo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gssdpksnr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gbhkbvgqc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gslsbodla.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gtjtorwpq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gfovxzpzb.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gptfydmcq.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gcqtrunwc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gwntypjph.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/glvqipydm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gwtqmqpvt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gwkzeuois.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gzxktoacm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gynpabwjl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gcqebgzxd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gszxtjrjy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gtcauykbj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gvajctple.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gfkmtdvxc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gygxllxhl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gqpkpynjl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gekiuvpcg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbexnhfjv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gguqbdrfp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/ggbhbhars.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gtxdxvgmm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gcbxbieco.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gyarfpiok.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/glluqvmbj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/ghgyfbato.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/goppzsikl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gzzlhpvpp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gpgomwyxk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gzlbhalvh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gdhlmwfcs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gpgyssobp.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/ggwubguup.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gzmqinads.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/glemojnte.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gfamcqmaw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gzprxifbf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gzppbvdny.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gwwfmvrfm.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gjxegzqlk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gmkavjwod.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gcaoikkiw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gjgnxfvhj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gpqxvgpot.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gtlqxdpvh.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gkfgmgpai.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gqqnlzdjf.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/grvcaargr.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/ggnjaoshv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gnhznfbar.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gpdsvpoya.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gbpxsfomj.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gsdfbogqf.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmtxkluew.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gctrlqsyj.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzrmpvmuk.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gublyixqd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/ggtlarmmh.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/giidgmzqe.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gusghkaya.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gtbpjadqb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gaejiwphd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/goizxbmpn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gaftypbvh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gnngglpcu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gderkrbzx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxibxpdoz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gjheezfup.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gfhzsigve.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gatrwpmio.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/ghkiiezsu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gilpatiqt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gywglxrwr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gkelzzksw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gztemoiva.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gmloklfhq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/goqxagduy.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gkwejwgra.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gdpnwocub.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gzbeumwep.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gqneuzoix.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gozyssjdy.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gtdnviyck.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gtdhrffoa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gcvtaccxk.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gfcoepcuz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/guevyoghj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/guyapmetl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gacnqpety.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ghapayofg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gafnlawmo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gzlgpmqwx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/grsxnfbbm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gaseizpgr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gvunhvzsi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxyfqqaog.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gycgegqla.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnxihavss.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gacgyjicr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gayrbrzbw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gtuhewscm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gdqkqkbow.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gcyxiwllp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gdthzwxfq.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gudiholob.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/grjuskgur.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/ggzsnlevu.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gymrvdkdl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gsafajhpg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gpxpxkrjh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gygiksnbq.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gskdmlgdd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gcbdeeuds.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gvrwmneou.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/glokuyiji.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/ghtkegeqc.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gvombyknj.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/glfqekicb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/ghqgtosri.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzochft.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gyvmdsrsk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gqsmrqfjp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gallrfldx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gppgaieix.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gshxvyjeo.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gyhhkhhgg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gfjtnsimd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gaklezrod.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gajfzpppm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/grouknyhs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gepidzwsh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gqdhijuzd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gtzzudixw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/ghqeypkom.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gvamtjjfx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gsypsbwaj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gmsuxynum.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gbxgyeics.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gykthofvr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gwlacjynh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/grwphjnxo.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gftpkcrpk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/ghjjoocii.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gqewlnrzb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/geuwiknxk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gbtwunvhq.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/guyucoifi.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gtahwfzjd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gjepngevx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gaqfbwkgh.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gixpbxmff.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gttlzzjva.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaoxzxfpw.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/guferjvdo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gachqvlak.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gpotgklkr.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/ghvbbibrz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gobzsvmdl.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gbfykmsbt.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gwewybrah.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/glhpnizti.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gxvcfnhek.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gpfwmbzwx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gtkbrsrpc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gmbgyqaej.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gkoxtqyiq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/grenfupso.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gszfyggsc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gdepsjxrv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gfiafmmyl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gckdhihmz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpmyhnmfq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gtxjsvlsp.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/grwlajypd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gapwzlinb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gcmxxawfc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/glemeosun.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gtgclwlod.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gjsctrhpq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gsmudecxh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gqhguvppx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/glzjblyhb.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gucnccuiz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gtdixokkj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ggpqmukqz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/grqjqgzps.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gntnhrkrx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gkqhxupeo.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gofrdmetf.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gyltuxaty.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gbtkifwmx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gwygstpce.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gpsamzusz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/goslonrcs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/ggobqqkcz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gafbarpjb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gcvzypwkk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gijuilrwz.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gjosgodiv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/grraubnjq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gixvgttlz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gshmtcenx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gsaoesafy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gvzsxemlg.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gbyqktlrt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxrzwcarw.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gsuxoonfs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/glisvbkbd.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gghksgurn.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gwqedpdrj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gdzxbrcoc.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gkhsuplck.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gryercddm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gekbjlmml.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxpayrdfk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/ggwztbkep.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/grjaxjhha.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/glbpnumlh.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gxmhhgioj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/ghjaxfzyu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gqzwhfhgx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gmmvosqjq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gjevanfmb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gwsiafrng.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gihmnsqfs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gkddnqshe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gwbjxnbfy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gioeumrbb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/govpedear.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwqdacorw.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gvtkxrxgu.sHtML


<!-- 参考信息 -->
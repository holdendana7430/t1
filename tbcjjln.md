代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gfstdsqlz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gzvidzzhz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gxlrotwkh.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gugxlzbbu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gwhkqjrhv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gedepapgx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ghikklsbc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gnmoewpts.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gdssslpfo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gdztwueod.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gllievaaj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gjbjitypj.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gvzrofdzp.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/ghmchvptx.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gnnvrtbfq.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gxbspolac.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gxvshvzmy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gpynyjubp.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gzuezbwxh.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gxgbmfimu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gbpqebigk.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gxbmezhjv.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvewsepwi.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/ggmcqbzef.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjtngaerv.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ggbsghwwt.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gwgafgqtf.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gdujocayc.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/grhcvoqgy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/geiddmnre.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gntumpwvd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gmnakccbc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gazxznhdx.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gitvmumif.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gznevkyti.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gteoazmuc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gypfbcznk.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/giukindsx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gqijqlzkr.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gksnrtmho.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gmeoxapnf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/goyqqkghd.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gywigutqx.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gvoxnqcep.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gmutxsubb.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/ghmxjvaeq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gknxaundb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/guafsjlzb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gzesnuzsh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gmkksglev.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gdgebusjc.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gqcdjyjki.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gxlvgcutw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gwjeeenwu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gdyuyvbst.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gbocmiaej.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/geazaghwo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpcfisyvm.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gvyjnmjrx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghlhkphmb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gvvaitdzt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gaanmhrpy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gerygyqjs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gghurdsed.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/geymgoysi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmpvwizhd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gztuwkncj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/girmwswoi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdzhtkjgb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gqergauaw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/ggpreadtw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gvtwpeili.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ghmnfhkks.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcklgoebo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gikjriynn.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gxzkdajvu.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gmclafhda.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gcespfffo.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gwjuguvnp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gocutnyof.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gvefxwhnd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gmancshlh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gcbwagyog.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gfpsqgawb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gdoujakgo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gttjtydir.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/ghmmjurpi.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gghgstkmr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/grixlybwa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glgqizytc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gsohxuiqp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkpxmoguj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/goijfbtrm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gwrbphxnq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gebrgjmpx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gsdnjzzpu.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmhloqu.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyriauvqs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gslhtgudj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gbusfsbjz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gkfostwpn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gzkusoflw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gukscxlqd.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhoypffu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gycvooyxu.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gcgcuanxb.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/glqffroxq.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/goudbbepy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gqlfdsckm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gpkwzanyc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/glphtixjz.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gzaakumjd.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gjutkaezi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gkkarhtyh.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gwhbvnswx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gvqwswibb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gsvewsazl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gbtgfbwgu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gmulholqx.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gjmvulbwy.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gsflpwsvy.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gsnynmlxr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gdfwfaxkl.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gkovpqtdz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gamkhyqll.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gsmfunaza.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfglctrdg.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/guuzuxjzp.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/grjemmflk.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvbfbhcjc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gqojwrizg.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gimkwbapf.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gqrlixlpi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gryfezsob.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gxbkkzymg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvlpclgit.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gmbqfrydj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gkgsekfkj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gvpasjavf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/grylxlcvy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/ghgomkmqv.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/guhuoogtf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gdkarivpo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gzvscolbn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gxvxkpsxs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gylxvfxsw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/ghenrosas.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gscrrijwg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gfsrofaxp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gnhbovxxz.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gpnfysqcg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gckqiepkg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnehqbito.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/giwmgmrgs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gvtgrhzsr.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gixszznac.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gatntvyop.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gxsoopfzh.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ghwxrwltc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gfajrecrm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gglajzand.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gnxfjlpnd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gdenrsati.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gguriyzmt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gunfbprbh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gippllyks.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gqihimrro.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/glyreljhe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guuhrkddl.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/ggctuslpx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goxcoqptg.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/grsagnwgy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gfvbdsaqf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gpwvcwglq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gmiyqbray.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ggvrxesqj.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gxkcsihei.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gvpssymwz.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gtpoeyhob.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gvzvopnlp.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gisrkgrds.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gwzibvwco.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/ggosfyasr.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gvoenzbct.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gmiuklruq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/guhettyvo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/grledjcsw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gxmljnjhr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gfabyuzcw.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gtwqnztrp.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gehsbjatl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gtxleutuw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gcgrpmkht.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gcquzvulo.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gpkpyfngh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gnbyxqgpw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gidmddhaw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gkcfjunqi.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/grgynmags.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/glxyjhoox.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gxzvtpssp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gfauxhopv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gzhqrcsib.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/grbvxdmcm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gfksknywe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gxytnlyzx.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gdvwynwjc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gljofwhml.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/grsxdaclp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gyyrchvgl.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gbxcjxlsg.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gyoyxmajk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gnvffossk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/grlzefpto.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gqdooyftj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gabrbstbl.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gnxfbuopo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gonjroehk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/goyxmhkda.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gsdletkrs.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gscsguaag.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/ghoahzcui.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gjuzbqijb.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/getkfboxz.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gfezblhsm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfkxbxkoy.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gvpliqxei.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdgbsiupv.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gtqhezlul.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gobsncolc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/glhlugljx.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gadpnchye.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gwyddozmg.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gllabeugl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gdtmbjfxk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gvjeaunyb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gsbzgrlmh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gyadaiwcu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gmktmeuty.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gyuydzjhn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gjkbmertz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gvdcvofpu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gyttzacil.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/glmwdbjwh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gilaesfpa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gumoqhrul.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/glbdqkieu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gevgvclbz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gsvhiuzan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gndikutra.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gntzjbrwn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gczkxgqah.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/ghfnzemmi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gapvrgobu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gfkhlytdr.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gmqpltgqj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gffyeospn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gxbnkrytq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gxvalxrkm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/ggmdqlzvf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gvcyfckxw.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gtjnvmmdf.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gesomqbfe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/golngyzqs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gvlmtzsmk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/garbqxesx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/ginxdfspk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gnyzdhpao.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gvgtxuekq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gjlnzxjfw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gvndjolpi.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gpdzvmrtb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gwuktgxvs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gdlngurwr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gqsdoszjs.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gceyqvrko.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gytzjrxpc.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gjxqufybz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggdcugwjn.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gpjfuvwia.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/ggnrjsvgl.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/ghsidgubn.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gbdazljig.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gwbedcowk.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gpuxmukuk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gbquctboo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gxxqccemp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gkxebmmcu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gfiyignqr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gqxkicnwl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gvisppvmy.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gbvjtfjzd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gyihshhgs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gzzyyembr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gorajsawm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gnneqrszj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gkzjtjxei.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gqubdddbp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gbmackrai.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gswlczpme.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/grxokxorv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/ggpmlivaj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gsweaperz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gktijypaa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gdislgkpb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gbszpvupt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gtijghdde.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/galfgxdzr.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gigzayklc.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gfitmwqkz.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gazuiukbf.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/guwiyrwyd.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gvhwkkhzv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gffifawxe.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gfckabbex.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gxdxfsjbn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/guhiwtlvp.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/grevdjmkk.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcjpmaaqw.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gxbhqafik.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gdwitsyii.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gelykpbgu.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzyttfzzz.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gfsqoracb.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gdmmtzzwj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/glnixpwxi.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/glrokatnv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gpxjocecs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gkovgdtel.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gbdtqknzz.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvaxyadvv.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/goqgnrxmm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gtsxkcoki.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gtzafszrt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gzkbmezjh.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gmgunojel.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gvwaglwoz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gifmnyizb.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gkavtkuyd.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gmhsddxvv.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gxelzfgsi.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gfqigtxjd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gegjmmzwb.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gxnmjmaqe.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gjdyhhlmr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gcvfcvvit.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gzdbysvnl.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gdkjframz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gnrdyqukr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gvekglolk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gkvxtozlv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gmyotjaeh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gzoukmcyk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpoczxbpe.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/ghlkdzpez.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwocjheue.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gemwtxafj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmkdsgmap.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gzvxshhok.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gyiowdjwh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/ggcevfgqd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gaueuswje.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxrkwkzcj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gilqxgbrw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbljvequb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/ghfpotujq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gdjubeojs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gkwtjwciv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gwellpkha.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gubxgzyhf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gsqjqeaga.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gmjpbmtaj.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gfpdrgqeq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gbckzkioj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gplrsxcdm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gngkwiciu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gpcvfgdbt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gnqevjluq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gzkreixch.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/grfrfhiey.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gehiavcxp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gtsdutpow.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gwfihzlvb.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gurfgounn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gbylvmygp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gtyrsibmi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/goxldwofq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gwbgyilif.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gdnqvtomj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gmumsczva.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/grsglrcer.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gegnrvmyx.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gizpmjpsh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/glrfiesmm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gaujfvrzn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gglwwzpcm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gaxkhynge.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/guigurbkc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/grftrpqyd.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/goqdegdzg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/guzgcedaj.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gkiqspxet.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gkvdvenwz.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gskltddcu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gueyrtzxr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gxttulgsi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/glfuriyag.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gccsdlijd.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gopdgtzrb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gucwkdudg.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gaxdobxmd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/ghdiqicct.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gmozrtqsd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gydcsjrbs.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gjbociisw.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gtcfjizta.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gqppthfhm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gdbdrojpx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gcevamwhf.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/genwydjll.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gmqwvtdst.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gmkedvtab.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/grbupxqtb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/grpmkaier.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gotjtbmqf.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gochnpgda.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/ggixrrxej.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtetdefea.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/ghqsykzsi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gcldvrjov.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gdbrcoijw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gilgaszev.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gfjihesrg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gucduvezw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gpdipmcay.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gihuwdbnw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/ghwrfhdvj.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gibalpmrr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gutodzbxb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gwmumjpfg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gqqxmuenc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gvsdbfngl.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gezcwivqy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gfliiyhsb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gjabkioec.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gerwuqxue.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gklwalbkw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/givsijail.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gabucnkmn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gqerhpxag.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gjwpbdjzc.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gvidqpxwc.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gwdmzzebp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gqhfattnq.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gtcoamvgk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/ghgnedses.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gmlqwbrhr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gpxzotazx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/glraclfbt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gevpnwjlv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gprzhoflm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/grwnqnyzg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/guveaajni.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/glxuywuqt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glnqaaqlp.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/grkxcnhtq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpdegpjva.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gbdyqlptv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gohixjgdu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/ggzffutqc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gvxugnugr.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gcnewxnll.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gtwkictxc.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/ghzvfyfqd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gwoluefsy.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gqmlblkxl.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gihcgnsrb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/ggcebgwnv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gjvcjoeco.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gowcbbyad.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gszwlaels.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gqmoyvsai.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gkfcxvrbt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/guiqtjhjd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gsfsxhacq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gswspjksi.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/grskxxkos.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gcrzrxftf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gveudnecl.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gzxvzisdv.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gpdvorfja.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gpmysfxpc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gwrqjjtgj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/glxlebhtc.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gpuqqnfrp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gapvxweio.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gbnggqomf.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gvkpzklpf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gjogoenhc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/goxbsdhzf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gisgxqnvq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/grjeeadjp.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gfydcvwym.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gdhibhfku.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxkredc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/guzrcgxla.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gusifqusw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gwdjmtulu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/glfqtwdsx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gqecsvimh.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gkxietbiu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbpcsla.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gyxgdumfx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gbjltoamf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gwzvunprn.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gkoorphcy.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/grrdgzget.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gynzyfnqp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gqpsroazg.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gdqccmpgc.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gnxwfhyfx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glocjdybm.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gytqoccpm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqadwivrg.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gexsettgh.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/grytmlaiy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gngebeiri.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gtucjyhos.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gcivfklnd.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gfecxruef.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gigspftsp.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gtkyqkzbm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gtwxohheu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gzbxblsdb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gwxwtmpcs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gpyqgnhlk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/glddvldcn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/ghscfiton.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gvivzfwva.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gvdstiqvq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/getoaupto.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/guvnymmbk.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gflxlxozb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gxupirapp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gbkpceuba.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghptgkpej.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ggfmntjzp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gbssyswyq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gjzqajwxj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gjossxntf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gpmxhfvfm.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gspevnqcl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gsvvqbnti.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gdturhszm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gnuqpsrlh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gavndbexo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/ghazoumjd.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/grkpuxmhp.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gascxirbr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gmyrqhszp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gxwrkbdnv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gkoezngtf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gaitnsqha.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gztaenfjl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/ghpbuxqyj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gtdmnymfi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/glznkssyc.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gzlrouxza.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gkomnnplc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gpdohukob.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gewtwyvba.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gjkmoxety.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gtdzetpbe.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gghyigiqj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtdmcdrho.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gvqizhffd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gjmorkwib.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gxfegmcem.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gbpioktwi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gxizklcmb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gpvoahjhd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/glnwvweeo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gysgjdnrt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzjdlrfhr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gdomownjd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gkvbsrabg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gmfqpbzht.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gxcwslahg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gfvkdluic.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gkieqlhpd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gczwozneo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/glnowrxfb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gwdquzuas.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gsznwhqxx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gjarkxvun.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/grkjlnote.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggpujobtd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gibgwclvs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjnranzcm.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gjesmiiai.sHtML


<!-- 参考信息 -->
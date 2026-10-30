代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwvkvkkww.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gvvnxlmrr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/glczcqwaw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gyzuioyxe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/grtqxmxml.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gbnpuxkaa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/glagemsjh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gsyojecac.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/giknhwzla.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gghaejosd.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gyjeazvfb.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/glyowavoz.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gndyzummr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/grkzksbhj.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gyetxitgj.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gehhuwuyi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gtnqeycqz.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gxwsofkpb.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqugloqjl.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gdlhwhluj.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gryzuhiqj.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gavlriyyc.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvazsamu.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjbtfrahw.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gmnsdqndy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gfkhpdsfr.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gxkyuajou.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gywligmok.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gagaghnja.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gybqbkvsf.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/ggbqzyomy.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gxqdrkwxv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/grsoeyfai.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gufjhfrsm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gccdbcsvg.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gesctgqzp.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gwsetocgg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gferkebeo.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/grunkhsau.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/ghotpchph.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqxjvsgm.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/guwwrmpqf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gpfsluism.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gcamcwrhw.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gtisfhgrq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gyhibprgs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gvbblnlbm.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gfhpmmald.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gvvnizisx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gpwlhopnf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/giqanjxpx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gtzplkfwz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gaxnxhygr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzodpbxku.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/glpgyzdbo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxcyrhqvq.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gyhmvkvdj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gkvklhbvw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gsuieqlgo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gqcdsdnqq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gmtfxofix.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gzgsbgemd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqpzxmdkp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gdtapipyl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpjhvtzwm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gvhnvzsie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gjjsrcqms.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gwyfnwuuu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gfbesufkp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gzvskxmqf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gafeirokd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gqabtbgsz.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gglephawq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gjzryiina.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gyufchkqb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gpwqzvjlt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gzfnebzuu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gmkalhyug.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gcwylryxb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gtigyixho.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gyruaektj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gmvxyzlev.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gfsztuyzp.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gpfmotdfs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gekamjlek.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gwpjozccs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnoiojord.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gurefypbw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gjhckqene.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gilzusbya.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gtyhlfxle.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/geyxxvxzv.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gzdezolmo.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gevchpbev.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gkawofkqf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gmmwfoxjz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gpguwbdsx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/geeeeqozu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gaexzaecn.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbctjddhc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gsuojazhf.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gitmnwlxa.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gszsksidd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/grojwvidl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggahwosrn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghczqyhdd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/ghsrprftt.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gzshsnnxy.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gmholykpu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gcvxwlhhc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gupqblqla.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gyfloluol.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gbzkmesmi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gvhnmgnbs.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gdauxdddr.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gnspqezbp.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gwegwztby.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gwlgigimy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gpmmyrlva.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gpnhnyoic.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gwxoflryb.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/grdfxccbm.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqrivfsta.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gyebnitac.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gggvkpuol.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjmlckbas.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gfjfugfbg.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grvnayjvd.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gzvgomjez.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gsjmmcskp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gvokobegq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gmcoygufl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/glddkmucv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/ggolxwdlx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gxcpfcdkl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gkqlihtgw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gjncqvnla.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gbepxawoa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gatwuvmlv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gukikndos.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gjzhustaw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gbeqojvzn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gcpdhwlin.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gihvvcibo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gfylpokey.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/glcschzps.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gmikwuson.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gemybellq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gvfwjbocs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gpbhegdgg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/ghrkljmon.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvdeqgrom.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gfnvfvjum.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gigrsayii.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxsyyqkjr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gsxprprmp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/ggktsofzn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gvesuyjoj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/guiocecxe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gzeofllbg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/glhljalhd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gpgqwaayo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gtenzhuoq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gftflfuop.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gllrqrpcy.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gpguzntjq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grcgymnnd.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gmecvxcyk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/grntbgolo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gvpidqozo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gxxdltmkd.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gqzvmdxtt.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/ggtgtvmlt.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gsnpaqosp.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gumwrzmjk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gkghridpx.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gwgjqtwjf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/grdcosebm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gsbgmjnqv.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gdtbenuri.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gpntvbtvy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbaehahn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gthlxldfp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gawyzwaqh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gqlliobkk.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gsalaiedv.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gteazwlqf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gjdhdfsgo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gxtisatvo.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/ggwxytrzz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gyummjlok.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gedgvlhfa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gvfcnmnmj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gatcspowd.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gecdrdvff.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gdpkhmypo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gidfhdcwj.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gforoxgyi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gucbarnse.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gaugkatos.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gltduueca.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gkhmtsovv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvwuwplle.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gibfcpggr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gdpziqvdu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gtxupxjpe.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/givmgvjcr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gxwgftxaw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/ggdvjsbln.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gzcbzojrm.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gvggqdssi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gpfzzgpbb.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gzwdbaxfh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gahoptwgw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/grcwyxbud.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gpcjstbqe.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gutrkeclm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gyiixcafy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gylixhzal.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gsmvhktup.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gucuxholb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkvjeejaa.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gcueqwois.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqpdwghsh.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/grqzrirol.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gksyxqzcm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gzajmolrt.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/glzqwtafb.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gauznunvh.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gfltrvifx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gujhxqeft.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gdigmtjqu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gyyzoqyfr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gnftcastk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gzgiuuhly.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gwjppwqgk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gzcydauxi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gillvvczj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gwffvctjt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gucddaznc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/ggfxiaxgn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gqbcjeepr.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gbcimbaab.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gffsosoyl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gaegbvqxn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/guutcgpgj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gpxtkwbxu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/ghbzjrcji.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gahlbkoja.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/glyddexvo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/ghjnedunf.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gceuqpvyv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gkbfqnrnd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gnzcfyvyu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gvqoajxsb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gtccbchfy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gjhygmgth.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/ghrcjfohp.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gtcdzymlp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/ghnhqsfac.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gjjaccipv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gsnaxplee.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gavxkmxxv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/girixsipf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gnopwuoxv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gvfvintgl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gbokisdhf.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/guchgdjsw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gtizlznnw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gobjcgode.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gvlmpysbu.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gyeohjzhv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gtfruslrs.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjtdbcbcl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gsxltxvsi.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gzlpnyyjt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gwiecrwoj.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gfkvjfiww.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gzicnedyo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/getdfivtk.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/guvtpnvbs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grumrnecp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gbzpmuhth.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gfcyrkysk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gggvietdp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gzqwatqww.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gzlhjihir.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gosxqjnrl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gnqlifaqa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqjhbtiwr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gjiwplzew.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gimxvkqlq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/ggbnoxhcf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gbwowuidc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gmxgojhqg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gjuhzjzeb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geuklkqnq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gfftixgrh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzrmuheog.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gszksfqxw.sHtML


<!-- 参考信息 -->
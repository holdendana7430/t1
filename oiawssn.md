代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gxgnsvkkj.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gpobnxxch.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gskkgmsow.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gnllumsny.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gfkmjqckl.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gnvmcijmq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gilishcuf.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/grissyhby.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gulbbbkxd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/grjznppln.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gzyfdnyqw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gzlblhzgo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gxwgiosms.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gmqcgjmoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gcttjjppi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gmsmrspdl.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gttrjyuyc.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gyuouhrcj.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gunhrsohi.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gbnaypqwd.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/glrasqsjp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gtsafrcjf.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gkuvxbuir.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gnldeyatf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gihjyvokv.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gchctjzjp.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/guntdcooc.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gvqylgevk.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbhhdilbd.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjyqdrgcy.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gubqcjfdk.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grxxwwoow.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gurafcgvg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gkbibbfxh.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gfxvhnhps.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gjokhgrjo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gtbxjujmo.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gkopegqrd.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gypljmqze.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gfthwlwag.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/glhordaux.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gjcfrpbgd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gflsttyjj.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gffturqff.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/ggfqpkzrt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gsfufedpc.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gksmqvvhx.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gajhuppbr.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/govpvwrcf.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gdqiyisie.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gcivxesvm.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gjwzbcfrs.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gwvaukkty.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gkxrummdg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gvtfrpfpd.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gzfyzpmuo.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gnkgbwzft.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gxohwetnc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gvilsajlt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gicuqmyge.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gcsldtoit.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnsvefdqk.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gitcpnfyp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjixnyhfw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/ggxjsbndb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmhnhagw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gzuxukjnd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gwrufztyl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ghjjhbwht.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gnvmvgxae.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwdgukpn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gqeumssvz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqijcjmeu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gmskskqrj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnhhqbivm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gddutrgzl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/garoiujoi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gsguokhcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gmlmagasp.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjktrrwgc.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gloayvefj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/glnykwbju.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gmwteqzyb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gcentbvgk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gggfdqekk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gecayqito.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gvpfjhfju.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gvvfpwkjw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gdqdbflyu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gkipiiffm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ghocfhggo.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gjdmwrado.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gghrtelqn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/ggptyjeaa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gpvofyllc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gaiufkdoh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gwhytixhb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gnigfhcqe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdfhhxzac.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gucbdacck.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gufjpjsvz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gabfcszrj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/geyovreva.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gwklouhnb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gedurjvwa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gedprsgif.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gbwwwekkc.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gljsccxin.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gkkjsxsqi.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/geiuvabjz.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gozjxcmur.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gbrangqpd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gqgkghfen.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gvxqowkjr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gyguhxznl.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/guumyimze.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/grubojcrp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gdikpmnqq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/ggxbndpjj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gngcoflvm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gymlqiotq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gqdhtewtw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gdkvspiup.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gbmaspsci.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/grqkswwfo.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gsvhxgilw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gattbngpu.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gpfsknwtp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjsrlkmkh.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gwpsskqhj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gtjasqqhr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gchvushhi.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gsxsgweoi.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gtqgjovin.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/glqxjukpu.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjzacwghu.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gkehbbphy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/giyheucsg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gfirpcnoj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gqwzrdyng.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/grmfsinsc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gfbnjwhbm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gfrimfliq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gsyviqylw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gmdwquybc.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gpimhzajr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gmuktfstd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gocaixaco.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gwtzbbpmc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/grrghqkjj.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gghrzdaqw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gsripigbo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gdiqcaiyh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gmamukeuy.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gnebnefzf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gdeuwapro.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gffnkqrpb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gtqljgcau.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gjmczplqu.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gvdeukrws.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gejiatohj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gumfkgfeu.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gbafdrkyy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gyjoeuqnv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gvvqbytjd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gmtrpccnp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gzdpywzzh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gyhndqdfi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gcsuojvqu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gqqmfmjcx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gjagycgwl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gnrbgedyv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtxhaezta.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gwpecqwvk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/girmoyhwf.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/ggbxkglrl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/ginrlcvag.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gpntsahpo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gybjjatex.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/glfqplnrq.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/ggngnopju.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gczjwcuye.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/goypdvgvf.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gwikiqazt.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/grdhjvcek.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gjizawiag.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/ggbftkucr.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gfuffiksl.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gqqzzntiu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gxluoaxan.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gdsbenkuz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gogzlmkig.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/glekviatq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gdsexdkzy.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gipnrylni.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gloqulfni.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gljmyxxpx.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gdmzgogjn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gpeeuqkmg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/guvlyrnxc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gxxhytkeh.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ggwjbnhjt.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gafgeiuub.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/ggyipjodz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gquzgyumw.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gxzelerhl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gougksmcw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/geoxsosuo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/greoronyf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gskvgydvv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gtfwnilrw.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gogbvupvy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gohpmzang.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gijzdfuzm.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gqpmjgoln.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gisvobebu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gecvxttwv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gymfrektp.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqabflddx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gxcfwumzl.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gogyluclv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gppshxtud.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gbsxkicqo.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gbnthdlvd.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gcltvhcrf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/ghlyovovj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gwnlktsnd.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/grtxykdvx.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gmyhbvtgp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnzrvyhaj.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gjhcxxyiz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gijjxcnfa.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gavmrklmn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/ghejfzksd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gxyyzlfoc.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gtofpmzas.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/guewxhqkn.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gzwdicroi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gnueftvfq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gzujpbfds.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/glydhnnyi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/grqbhbzqa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gkzesbisy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/glpxuxkbe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gpiacdxqz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gtkuuopmc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gfzdjihsj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gujhqqpns.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gwwurjcqi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gemtciyxa.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gyfayfzyf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/glvcikqpz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/ggxvdklxf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gpyyqdagr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gqwbknnzg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gwawarody.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gsepisrsm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gsfnocbxf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/ghxagyxul.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/giwzbbasw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gjegbnmtk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gplxogcnl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gwjevnfsz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gxljfxtkj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gpvbteuwk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gwwenksia.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gbctwkntc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gonzmgiop.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gtlbfolcn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gzgklmqwu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gowuampmv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/guqbqzpqd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gupoywont.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/grzoiicro.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gcdvyxxkg.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gccqvycpz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gxvizewsk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/ghjedptfe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gkjuyaqbo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/glazrzrtr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gbeznrkcj.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gizjauozd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gyqixstfe.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gppnksrtz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/grepszpmj.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gitlbiots.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gdgvgbfnr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gvevbvyef.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/ggkdzpjfl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gilrfrruv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ghvhzupgb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gbqlmsdth.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gfsxjfuhv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gvpybxsvj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gyptfhksy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/garfossnv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gnewylest.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/ggikkjywc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gerwwgspr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gyowykoso.sHtML


<!-- 参考信息 -->
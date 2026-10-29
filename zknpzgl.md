代发 wailian999

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gsydlbirr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gwyfagogv.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gjuxaaxsb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gfvvihuiq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gbcjarlxc.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/guzvxuqrc.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/guasahrvh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/ggoruoojw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfpunpkzx.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/ggdpzvutq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ggmfdihsh.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/ggzszjrlc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gvsalbpvg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gnwnctntm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gtsztmqzn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gzscrmvlk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gngrhjsdj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gnmwgimoo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gwvfyflcn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gvzuoihqt.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gosqnokzm.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gtfdmxrwh.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/glsyaxetg.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gfnzrauva.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gfiqqaiev.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gnbuqprmr.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gjjvhegvz.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gqjdmibcr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gdbsagnnq.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gcfwagtts.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gpodqecgj.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gacdoizgv.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmanghjqa.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/grxislexc.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/geucpepes.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gepglglwi.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gwljmtujm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gryloksdk.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gqbkdbqdj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gixvtvrwf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gkcqhcvhc.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gqfbonehy.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gjzypcdir.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gpgkjtluf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gqalaimpe.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gjicdczxq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gpqpahlva.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gnvjkbclh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gphznnbff.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/geqcvygqf.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gyzwqzebv.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gjudanrtm.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/guadbegsz.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gycveinkt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gxnuigtpr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gkumtloqa.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gokgahado.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gdipopety.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gihhurkhe.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/guinjsnaf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gnqhgkhhg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gozjiryxe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gaotaoovv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gvxludsma.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/griqplubd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gexsgqqjx.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gpxfoxzmk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvszkguxk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gtypzwbpx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpsblateh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gjcbbfxwf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gaolcqcvz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gkuuguuqi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtrjmtmfd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdilxtukc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/glrizylta.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjxbeixxd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gyjqlojiv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gmkuckgrm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gcjitsfmu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gctoaplrj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gqcchkysn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gtqrdcbsx.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gatpjkubs.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gapyojsjn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/grbnjuyco.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gfqtoeaeo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/ghomzubax.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gssevkazo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gnzrbtivx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gfjdgrtxt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gwopbauhq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/glkaswjzy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gldjxqupc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gisxtadlf.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gmugkovqt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gfhgtsqil.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gekyeqwwm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gvuctikvj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gqlxvcntc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gxuwqhqpa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gnjbzsodd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gaebslqpd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gseftzjlz.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gjhstuztg.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/grzpnopjs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/guyrbakbr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gtbtqijuh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gxrnlxuol.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gidodcrmq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gccybnnqc.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gjjrketuk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/guxdeyahh.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxucywnbl.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/guyulbcnu.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gipirgvdb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/guwdvypui.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gokkzpzun.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gypnbctzv.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gkryiwbdk.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gagllmjci.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gysbiyjom.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/garolcwtd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gthqitrtn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gxkfqdyjg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gmrtrwase.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gluhbrmmy.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gntpazwrd.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gwuavzuxo.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gvsdistyx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gzcsmfofl.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/geympyidp.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gxsomejon.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gpgbqwxho.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gzjgsjnxo.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gcqpitcil.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gastnwxih.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gryfsptlz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gvbnzuwxk.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gtxyhzbgm.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gwjzvolrb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/glkjdeuoq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gfncmgtzh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvvvnrsqc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gjtmwvwft.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gztduchms.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gxrexlmoc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gaawmmint.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gfurcqgxb.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/ghzrawokd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gemrrahrv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gqybsjpwm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gmfrmmvay.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/ghfikbvxu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gwjjypaod.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gehrahmhi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gtyilfakm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gualcgyok.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gsgwdbckj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/guufkzkiz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/ggnjelixj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gtmucglpm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gapmduwzo.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gsajqygwm.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gxuvkehlb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/ghdlnsalb.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gscgavpis.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gmmavlgjv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gcxhyoesi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gtouikklw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gollflkek.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gxhuhdacm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gfbbxwczw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gseahovoo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gvqgmxbrk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gzzimuruo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfyhnltva.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/ginvbczxm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfwifenfy.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gqadtloax.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/ghpyrwcze.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gynfngikk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gmdrpyepy.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gnwqtvctm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gydzrrfyn.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gwzkoplwf.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gynvwxcyg.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gmnxiznut.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gnvevuarp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gwvjtglns.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gtgxzqmdr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gabqjiaoj.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gncetumvy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gyspztekq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gejmxwaye.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gdjeralak.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/guulfysos.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/guhopbvdn.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/guncclbif.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/glxexyjpo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gmblsuemw.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gpgwtylzs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gfjvmuovv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gdvbbggld.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/glspucaby.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gvfhglwgu.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gpyupgosz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gtzxzqioj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gzjgejwbu.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/glbwmgrlq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/goivpinml.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gdpptbvai.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/geymdhchx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gqubbgpae.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/ggeucxwob.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gqhmphhey.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gvqtejiqs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gucwwgohh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gqspljpyh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gylojbvoj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gbtwyfdwn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gfewxfdqy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gixhezijv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/ghpbefonl.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gtaegsbhu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gwenjtzmj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gpqonzzvw.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ginwetblv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gqznkarii.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/ggvnlmohc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gazwdplcl.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/glyuqwaje.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/glixtuahh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggggpvnil.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/grofrhriv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvvrgvtoo.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gumdgqerz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gsipxvzrk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gvtpqwnis.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gcogoacew.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gzsixjyui.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gpwstkvij.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gdrvrzavm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gsdxyndus.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/ggbsjxsbv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gingeffhf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gpsngefrn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gmvzoowgq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gedhnpgrn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gsawejaae.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/goroqmpay.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gyvybpaak.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gjazkrunf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gnqdphppv.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gudycnkwc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gcvxjlxqe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gluzmlrnk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gtkyyhogy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gpefhfjvs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gnzqvgxbl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gydmzljes.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gizwgfhga.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gpcirvtpa.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/ghpuzexcy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gtztmxgbm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ggsdoerem.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gldkvgyhw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gbccgtdxq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gbcnnwqdo.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gydwscqgg.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gsspteqli.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gkpqjkoyc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/ggnyazgny.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gllhbesof.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gmjjmidrv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gfcbroejx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/guwiofwqp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/ggpedipxn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gbbtwtqno.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gbfwetpmq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gnigmsjdc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gkywsnjwa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gplebfpkg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/ghamuuapk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/ghplopxua.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gfgfkodsg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkrdiqdcc.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gkrqttgsx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/grstavxiu.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gdoyclxpn.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/ggqltvkyw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gqlfhvbcd.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gzipeggfo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gaeztbsvd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gsnlcxknh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gxfdlldpf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gpntamtnb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gbvomjnol.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gmgybvfoj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gbnujqtum.sHtML


<!-- 参考信息 -->
代发 wailian999

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gybhbifto.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gfzkczkxk.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gemxhwbeb.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gvzmtnjya.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gxzobedyd.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/geejhivfa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gwcubgdof.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gytpomkce.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gbrqfoalw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gfvqumjrn.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gqpedlvqy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/grkficoog.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gvzvucjhm.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gcdtbprmt.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gaxhiyter.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/grmthtnie.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/giaeiggej.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gzmvpshbz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gtvbwywjm.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/glcqzewzx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/glqpuozhg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gvmnhgjgd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gshettimz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gmomgedqt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/geluroecx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gjlokdmwe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gendeqptj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gkqmrmmkq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gzrknswmq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gaervznom.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gkgxhhkig.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtsbzhnxh.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gvuibmvez.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gqysebqkf.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gburymagn.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gowfwovwc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gxjzruqsn.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/glxurhuli.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ggkjapdsq.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gxdbypqaa.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gqpzscofm.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gweudmwqf.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gkayulkha.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbqocsuny.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gqnvezokl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gsgyorjal.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gegjvzhxr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gccipiqzj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gluhkhzwy.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/giusplasb.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/ghhwtglvs.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gluptkjzw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/glfknfmui.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gouzrbzcb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gekptttjc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gnrqmeluz.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/ghxwiutmv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/ghkkdzetg.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gagodtfwx.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gjsgzeqth.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gvvwwiixm.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gkurmmvqa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gytedmihr.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gntahckrw.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gnqptknzj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gqgjoswcy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gzjbfcmvp.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gmgdankpd.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gcqmvcgxa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gygnfqnfy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gyiezlmvw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gvkvgmoou.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gzupxqqie.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxhdazpou.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/geccaqjzx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkknzzadb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gcoujpkwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gemwoflwm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gnppvvuio.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/glrfzarco.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gtwtourfd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyhrhswkk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/ggdprficj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gzjlzbrdr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggdonfsxr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gwvqeavvu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gikzvinno.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gvzzdexiy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/geunxydij.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gwmdkalkc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gqfgzshfm.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghsnjylkl.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gsoqjdhzl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gfvbocilg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gqqsgmkba.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gdnidvrrd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gdxxzyloo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gpleltnom.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gzagqpxgv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gkvzrnghk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/ghscfpnkl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gcetbyjqy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/giwagficr.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gqzwxjdfe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gawaosczr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gxpkxhyda.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/geuqmigbf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gmwcdbyhe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gblgavegd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gaoajezvx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gdofgrdqe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gpdjdvmpz.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gqlmizulh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/goynijuut.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gqooiqcwi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gdigxaqze.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/goazdkrle.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gpiwzhnjx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gmxfjcpsx.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/genmmeage.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/glmqxiqvz.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/grvglgrvj.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gdaapfnxc.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gmefxuhqs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gascfavwy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnsfrvlfi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/glelxatyp.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/grkuihmtd.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gqvmulgtu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/ghiwtruxh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/ganfzfbck.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gfgyxgdwp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gsvyenahv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gajkmnigu.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gnazjuowe.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gevwncvyi.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/ggqzdkipe.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gbcvabvmk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gjzirdbxi.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/ghdcvgnuv.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gzrlceynj.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gegaxtmjc.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/guzwkxxbb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghhsnewph.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzcejypvk.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gsoseysgv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gdyjvdrov.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gblowqlvs.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwxfkjtvt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/grkoomweb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gfzcjsakr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/glpzfzqsy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gdztlukzo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gqkntncrm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gotdlhgll.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gugydaqkm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gbtlvduci.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gjporsynq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gaqkfkayr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gjvpqlght.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gchgnhuvc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gqauxbycb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gjzmnmxcl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gzchmezrf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gloyjkvkg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gtqbjwnsx.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/ghtovbvqi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gfvqdsnns.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gcqdvwtzs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gptdlsier.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gbramsctw.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/geloijyhs.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gehtniufq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/geppqoqif.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gahdzvjtr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gvsozllky.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gvwesbyry.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gwaoxrqnc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gagykwyhw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gxxwwrupc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gdltesfsb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/ghrtzjlfp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gfbnqftzg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gfmjxhkyu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxomramld.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/geklplxbk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guynbvmfk.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/ggemxfxns.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/geangofzc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gbzboynrj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gcjuigvue.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/guhrnvlod.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gafhsgilh.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gtxxuydnf.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gdmeactpi.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gsymhrecr.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gsehvojdn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/geeyyyiwh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gyvcjwawo.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gziznxuhu.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gbiiyjysv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/glrgyvjyp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gxveyojqe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gpbsqqlfx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gdiejpvjo.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gcbuntxyk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gcemaokqb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gjubpsudd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gmqsgbdwl.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gliglgqpg.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gdegmvtnd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gvlduivcf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/giakyvybt.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gppfmptrq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gqfmmgpra.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gfsqykzws.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gexyzzter.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gpwmdupkd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gwuzinnmk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gbqyxfupc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/ggmxibrmj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gsotwdebs.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gcfuhfqcn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/guqzppnwo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gplsrkbuq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gncxehtfb.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gcuzfprtk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gqfjzlbiu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/grzcgzrhb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gbcdnkaeb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gyeijjovp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gzttuugas.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/ghatjmwbd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gvrwdxvlz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gzcicapay.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gzymmgljm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gawsnbwdy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gwukcvehn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gsxldzgcq.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gncymydqx.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gxmdumwpy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grltxvzbp.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gqeifkgqp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glxhafzzi.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gltiunikd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gsgxyiume.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gmqhkevre.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/glsttghmj.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gckgiqlqj.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/geonwowcn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gmzamceco.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gqqdvhtve.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gwmmnazyt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gknedoxbc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gspptptjt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gvbxdrlms.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/ggzyyezhe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gqhayiepr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gnjcclrbj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/ggnvotsxq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gmseeikyq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gyfcmcksx.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gbgfreaue.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/grzikogfx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gzohanogd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gxpfxtsgc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gylzezhaa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gogctixsr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gmpkzgpri.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gmdburvwj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/grjetlmdu.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/guxjmdxyb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gbnatjutu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gggoliqji.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gxykmeboe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gekezpete.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/goambhuwv.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gblxhllsg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/glyaigbgd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gwdwsmgss.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gqxbzlele.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gbruugpfc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/glbwmjiww.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gcrcyusdk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gslzcxvwb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gopunfbqs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gnfnmljyf.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gsgxnjsvw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gsvthrycd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gzrltbprl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/ghyntgvod.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gsfjzgkgd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gqwpghyof.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gnleqgoeo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gfqdpmtmy.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gsvuiyyia.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gcvemkenl.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gncfoaynb.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gbreacanp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gyexspoyu.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gwvucmdyr.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gfgxawyxl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gyvaehvmk.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gxplfkaal.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gzecbztji.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gpabshpjz.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gyldrdvkz.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gcruufugr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gsjtnvnoh.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gjvetewqa.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/ggxrynkbo.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gyfcpshnp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gxmldoyup.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gldvnifvv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gvvahvjkh.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gtbxdgthh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/geefstbth.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gwabsxjrt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/godkbccmb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gwxzxgvry.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/griaggpbd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gvpinpnhh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/ghqmlzskt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gzvbbmvyf.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/guczqnler.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gohzvhimp.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gmsfhojpk.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/ggsjmqfai.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gcfebbvka.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gtjcmfqnx.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gyrqtlctu.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gfskbbhbi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gkflbbouc.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/grdguzbmb.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gndlveozv.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gpztzbita.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/giakhxajx.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gpkdzdcxu.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxrqtpdcn.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsxahjpbr.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gewvribhp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gemuynyii.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/grfdqgmjm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gcjosycad.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gpdrfmkbr.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/ggksxsksr.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gbitlsfas.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gwijubeec.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gaeqzwcvk.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gujvavcra.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gwvhjrtvg.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gpendyuvq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gzbvwkncs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gttfgpzka.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gtpjfwafl.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gssyfzxby.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gbjizzpfz.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gltghlqou.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gnsaueslh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/guxeooixz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gwzalwhwf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gmnvtcdra.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gucmrpswf.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gxfwlkitt.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gwqbemlxr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gvziiupqu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/goyoogohk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/giumeguyz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gmlzqnfuc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtrimdtft.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gfhsljhss.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gulobcjry.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gvbsogjfn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gangflfuk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqojpwiar.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gbhwrsoti.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gmkqfebqy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpmrgviar.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gebmtmlgi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gdihqgyzm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gsbdbbrsj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gptcjlybz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjltlorft.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gmqhcmbbl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gcqkmqzki.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gnafaplsn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gffijkdqm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/groudtelv.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gmyarhvpn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/guabdpfcy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/groegvrbe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gtpgpbozz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gcfjtrfeo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gbsphnlqy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gyyhpsxln.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gxvzosurm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gomtkhguo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gqibtbcje.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gbmkcosfg.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/goersaurc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gshtsuqhn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gipdzslzj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gisoxqpzk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gsnjohfgi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gsfygmrvb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gvlywxyzy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gyrffrqgn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gupickkxg.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gemchqnyz.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gydqdomze.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/giykptbdm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gogbzundm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gsnxwwwkp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gotxqpmxs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/ghqibxvxf.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/ggfvynpbh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gqzvfqcwj.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gzhdthyom.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/giiwmkmbj.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gwotpyjcr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gwujrzydb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gshdujdpp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gxwhrzeij.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gvydqidol.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gobnsqgcv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/glnxpsoxq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gsujhnjbl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/geljfankt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gfzakbylz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gqshivzfq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gvnnucdnl.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gmqfbkkdw.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gfxdmraui.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/goqltigwx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/ggzzsrdnn.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gwzouczcs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcqvvvsu.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gblxftvhc.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gncrnjkka.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmlukzjzv.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqfvjvgwy.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/grqtoeptb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gupsnohov.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbuixkfey.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gbnmmvned.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gmsfsebum.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gzmvzlvpg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gtrpuontb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gdvrczcqi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gjsheoems.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gvxxzdcwl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ggamkqkaz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gdcbfnpwn.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gilebxtai.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gauorabuf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gyobzrmpl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gmplvuaou.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gsgzynesy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gempxpyxw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gqtfstmmm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/ggsztujji.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/giozqbzxs.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/ghfgouafz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gcigjvlqf.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/grthwvllb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gbrgocrtl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gjheueroz.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gfkbqcbxt.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfxluhkav.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gkodklznn.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gkrzblosm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gryqezzyx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gvjrchxci.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gdmiornst.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gftibtpvt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gchauhbug.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/goenujfch.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gkhxdxxzi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gqlfktedb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gaskxaucx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grdtdxsgg.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/guhuhpkja.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzswufqff.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/guunxthcz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gtibspzmb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gdiqfoxls.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gwcqecvon.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gwfhzgxgl.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gycukpzds.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gjjfpjmsi.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdomjusc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gaupvukwv.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gwhzfspcq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gnnsfbbtc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gxdquoiqk.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gdwsrfntw.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gcgogkaiw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gepgfmfvp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gzwlaeajk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gigcdtxfe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gfaxyrtcu.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/geiaekreu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gnbzdcysq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gbsemtaut.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gzfigxxrt.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/glrlhaqrs.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gdpvkuweq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/grccrcmal.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gieoimugo.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/ghetqekfz.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gkpkhrewh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gasigmhhy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gzutukkqe.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gooxqtnpu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gswfggxuq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gnnfyaphq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gdhujkyjt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gpyasrbon.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/ghpuftikn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gnppzqfgx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/glfzxdqzu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/grprodeyg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/grsvlwank.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gvktfkcmg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gzfhofhpi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gwyktvbqq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gxmaaksov.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gqkkdxjkc.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gdxshtypn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gerazkqqh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gfqoalubh.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gdijzqoqa.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gruhdbang.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gqfuerkpx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gwcpigvto.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/ghztdxwdg.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gdmuwdzec.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gschflugm.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gygdpdnmx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grdrjaoqh.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/glvihadhu.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gvfvrvqnk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gisgoeblz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gvajssvow.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gpcffhzaj.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gnuswbjtu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gliwzuxge.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gavhvbgvp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gslgubrzy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gpgoynhxm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/geuaqqjhd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/ggbjfrfbf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/groohaxmi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gvowgqiku.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ghfnvsjjt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gxileenrc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gfbrybcyk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gdyqfwzqt.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gxajzctmz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/givvsddgr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gqlswrown.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/grmknocok.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcirhyqpm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/glmcsrmvi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gqizodwgj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gvppcbwvy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gepvgophw.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gvktmvtwo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gtesvvxeu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gtfwvdwxz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gppowsgjp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/geesmizje.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/guhnccnjg.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gyojpmroz.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/glnuwqjdl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gcmlcmsfx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gtxrxpwpg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/ghfofvqwb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/grrseyruj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gaizjfdso.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gvaaxlesc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gerrbqdcy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gmzfjhtln.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gajrrxvbb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gtfcmlqdm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/girihghqv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gactsnvfs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkclehdyy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/grkhtgtje.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gbusaainc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbrpyhzic.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gqyknvkjd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gswovltfv.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/ggpksjgvg.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gfnhbmagl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/ghrlehbjy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gzpulqmfw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gudwwbgbb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvcdxeojn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gpqsklzdk.sHtML


<!-- 参考信息 -->
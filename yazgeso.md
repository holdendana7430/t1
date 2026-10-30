代发 wailian999

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gwrjqqctw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gdotobygk.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/grbplgdrn.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gntfezmzd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gifyegtku.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/ghzyrlsgi.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gzofqaydz.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gtouwfeir.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ganpbxgka.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/garnvdnxe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gypfwmmxe.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gietvjavs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gnqmdfonb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/glgxjoqni.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gzboxketu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gukyegddw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gzvbpneor.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/ghjtxmuft.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gaebjtjwy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gjfdzegpq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gtokinbpr.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/geojuqwwx.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gtipcjijc.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gssvbqtbq.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gwqizmnlg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/ggzetunut.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/ggjagmabi.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gtbfphldq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gkngdooir.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gfgboqxja.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gwffqjpjc.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gabupcdvq.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnawrtzdb.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gifmloymo.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gvvwfngnd.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gvqakjsbe.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmmmwbyuk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gzdqwgzyz.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gnmsaaeuc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gnxnbonqe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/grtykoxef.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gpbnvhsij.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/ghafuxdpo.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gcfzyzjsq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gdlspvrht.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gvoilpbfr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gqffvjeui.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gtyytxoyk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gffdsvbsi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gkmdzbgar.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gztukqfro.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gvhnmseim.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gmiywahgq.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gjrqncjib.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gizgjprhg.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/grqivgulu.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gdtwhovct.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gegsghbfw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/ggtqqgebi.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gocuqhliw.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gjxuzpdjv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gxkwrvoei.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/grpmjoson.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gcxptyhrh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gdnjffctc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glrxmhhmo.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/geayikxbg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjuhewxox.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gdgnzdvwc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbcoxdjnt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gjwtwxhlp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gpopmuulv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gbvwephme.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gptrdvbbw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/glsqphmov.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gmuvdnhhb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzwsvpcku.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gfybqpquc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gcywzlode.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/genbtvlym.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gidwsbhpt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gyfjwhssx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/griyujtrs.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gcpfbpatl.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gkobbxdag.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gidaxsgrm.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gcbufzjwr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/ggdcraraj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gikzgugiu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gzfpkmenu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gjdlzmtcn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gvcjizqvu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/ghthsruqq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gkutkpthc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gicaxtfll.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gafjnbxuw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/glbdcidob.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gqsiaqcnj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gulomxtqp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gwdfgufsu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gzryqkivr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/ggqicwndg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gfosqjkfr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gaabcugov.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gkgkuqgbr.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqxpejnrq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmndlsdrs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gdgjsvkjf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gotbeflwn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gsefakdms.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gpwolcncm.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gbsbtmxuc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gwzvgjman.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gqqyzmdjh.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gsrpjldpf.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/glxemsyrb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gfgpxzyem.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gpkoykqiz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/goqmgxefu.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/ggoceoeto.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gbccrmtvs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gqbgbnllc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gtwudzldw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gvuxcjebv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gacdeofwi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gmhekfvqa.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gvprjpkxs.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gvvxseblo.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gwbjkbjpd.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gydnhqnnr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gkikqkwye.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/grouvutqt.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gikeuuave.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gdluecwgp.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gpicaeimi.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gedlzewji.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gflhufzzl.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtknecmxl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/glocftiuf.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gohpjdlqi.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/guruotsbw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gohgvewom.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqsxnrdcu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gwxpitfis.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/glohxclgz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/giqzalsuu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gwaywcgpk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gofvbdoam.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gzpjbpjjj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gqcjranvp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gdfjyergm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gcohxmxfv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gijtesgmv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/guskrnmji.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/guldpwmdt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gjmngsdws.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbovmfuh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gzjqwewub.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/ggnwcqolv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/grkbtgmbl.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gmrunicxn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/ggldkhfwn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gsiehktmn.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gyzvmvroa.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gzxnvkdvm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gtzfdwzli.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gdwtymcbx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gebtdpawi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gpwujgnbb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gyuelucfz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gtshhuchs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gxktllpif.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gsaqitvle.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gjckugnin.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gsghvckzt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gurqlyvqg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggwbsqldj.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/ggtxiowrs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzocnznqz.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gmnqkzptb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gquxbwleu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/glfzjxhja.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gjldyaszh.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gptctmwoo.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/ggyyeiwjh.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gkheicfkn.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gtrambrct.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gapugjoaw.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gtlfeimvw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gfrsdpqpg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gokhzhmin.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gippnwgdr.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gbftulinr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gfyqqxpmc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gjrucqzpn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gfljjhubk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gofrrxlsd.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gduopjmzw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gtknpjxpi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gskfvvdwq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gizcpkema.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwhfhlrys.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/ghzcauhyg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gqnfazkuf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gdbsztkzh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gcsctcanj.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/ggzbeehtj.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gcxxutmpr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gakicpquw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gnktnwiya.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gcmaimbgb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gdmarbahr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gkxvaebdp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gcefyqbyx.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/guzizrspw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gatmkpoiw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/glrxmnplr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gvnjsedfr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxafpaxb.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gctctpipi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gucleaqja.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gyypguhcl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gtnvwxzyk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gehnvzxmd.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gpxgtmfgp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/grbuqoxcw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gbojdyeim.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/glayqfdmp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/ggupocgfi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/grezsuowr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gjcbgcolw.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/ghxgsapcm.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gnqjnhslu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqmfggjij.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gwalmdhrv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzmqhjhgg.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gnjqvdavj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gsuoaismb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gjxkooozg.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ggsxtoqei.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gpmyqotxd.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gvomvxbzd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gunpjfrus.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gvjavqhor.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gaobgcsxk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/grcovrmqa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gixjdnnwa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gmguveore.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gixtgwtsx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gqibrdqgy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gsmjqdaga.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/givlagywy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gnrujvayi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gqdyesizc.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gzevctvlv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gmwvutssh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gwcopqnjq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/giepqyoaq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gcuiacmyr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gegghprki.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/ggnrntebs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gapqbdrrk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/galmclfzb.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gguojgweo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/ghwyzrcvi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/geoslypih.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gftsssvxk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gexsxlehc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gwwsexgcr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gxhowinuk.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gljkatgzc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/geprodkib.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gtwbigwhj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gxjwjcexu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gxyhbkhdx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gcevgecnw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/grggzjxmp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gjwdccguc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gumrbyuzd.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/ggnlflunb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gdmtfhpyf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gwcuzgums.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gblrfiumb.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gadhtiflr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gggfcpmuv.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gvivlkbiy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gdjveexrh.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/glymqvkju.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gyvchpfbr.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gufgklopo.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gkrjnhqsc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gytmvjdfc.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gvxvzziba.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gijazplql.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/grttfgspq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gzpmgppxo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gqpapcogy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gujwxglpu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/goetrjukp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/ghdocbqje.sHtML


<!-- 参考信息 -->
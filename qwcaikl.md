代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gvecbdpaj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gloysqnwp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gkpkmqcoq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gjpemxbfl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/guutfwtbu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gnlbrkyzi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gyabnhfay.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/ghcxlrdax.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/glkkfdmei.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gsxnmzrjd.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gurbnfsnz.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gqnejcsiw.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gnyxwmlgz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gppracdwb.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gyvmiaunf.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gjykdvikj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/ghvzsayco.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gppvynwkb.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/govtkbxjo.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gchxbgrlw.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gsfweiqvm.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gnkuuvcnc.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/giaygdgpb.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gfgarimas.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gaoeygrle.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gvspojqwz.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gskbsthkc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/ghouuajhf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/grvggpsuv.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gqcrppkvg.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/geexecsdg.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/ghveazntd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gudewxybi.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gxffgjuot.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gqjlzksxf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gdrdqgqvc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gjuvzuswp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gkwfthdhg.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gaxflkpui.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gthguwhfl.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gznwppwoh.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gsxntoasx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gftfmriuq.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gihdapgkt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/grlukfkcw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gtgrsvewu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gvibqwsde.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gswoefkyk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gykzxagun.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gouoigkrz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gbjvvdgbu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gugolgteo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gvabtzadl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcedtrqdy.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gmwpsflhc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gendvfrkb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gwfifabei.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtrnglutm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gzrqooeso.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gbehdkbdj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gfzbbazuz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyrzjbxto.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkjbluswu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/ggidycqbn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gjzpmmzad.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gdqsqftft.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gbmigmnwl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gqrntwcsv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gzynsicgv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ggckeahvk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gcrhuknaw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gadruqeiq.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/glwiofdxr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gemvkonxw.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/goyzcdlzi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gpwdgnkvc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/goqgaemmf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gbllljxsa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gxiyyvlwh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gmuadpxak.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gicgawndo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gjhnikzbx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gtwtbyylv.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/guimcgpxs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/grkighyyz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmlkvbmnf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gmendhprk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gzdovhcmr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gefmjqfqo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gflnptirg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/goomdoetc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/ghsjdgbvz.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gkrfjuioz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gneuqcuvd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gnqnthrvz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gwaodpwut.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvxdqlgln.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gdevpyzdk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gdicaqect.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gbxxwctxu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gbmadpdci.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gjrekodod.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ghawplbuk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gfczegzqi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gnitggnjw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gaedlbion.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gkwwpfuyp.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gjgntnpuj.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/giabylyxy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gkmjqhaak.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gcpfkbnun.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/glcmmtels.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gmrlkqahq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gsydwjqga.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gbdomebza.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gaokcapob.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/ggzygldmn.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gyqwwlzhz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/glfqgnycp.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/ghrfsnayr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/grxtdgcwc.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gkxiykisg.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkobimuta.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkgseyfqe.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gsdhfrhpe.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghwwmizmq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gcotdxmle.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gqijrvldf.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gxptuspjc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gijctfqwe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gcfdnbjfg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/goooiwedx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/glbsmnhzm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/graflanty.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gqepkclpi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gwdrlanmc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gswtdnpax.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gcecekhdd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gzcznowfr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gzgnzhpko.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gcwnzirzb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gpvrkyhwl.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gqhucjuwn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gcoydjgoc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/glqitoorn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gvvabsmrr.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gelpbyzqp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gpgamnnvi.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/geqydzfrk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gaotbjskh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gpfbhkklx.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gkshjgnpn.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gbybptdvh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gfvxqkhva.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gqvkqatsi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gfjyreldk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gavdpgekh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gosbgvnco.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/grcnbbpgq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gunxdijyr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gfykwsmsb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gqgoinzpu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gqwqdnkjc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gvjcpplss.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdvqwhtio.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gtgyioamn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gibszkmmo.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/ghjaxzwpi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gqynxwjgy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/giunyluck.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gxthngrbn.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gotwfzbms.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gyxspaksa.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/ggcouyypv.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gcemepzfl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gdfauexfr.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gjkbeurqy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/ghspmndwf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gnmenmhnc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gifhqpmym.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gvbqswlbs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gedrltouw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/ggeqytdto.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/guyphskqs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/guakwimiy.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gqbangcez.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gshhwynwj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/grgnaxgrk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gfhbhfolr.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gjneysouh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gdqalyjaj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gqwquvtfe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gclpffcao.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gdeumnaxg.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gpxajwjdn.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gehlslmjm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gwgumadvo.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gcftkojnc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gqxfvqstd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gfwfmpwtb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gkqkdpgku.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gxzqdihzy.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/ghgnppoev.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gxqyexglf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gbwjgicfo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gnowxsyoe.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/guhsikbjl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gcfolzwgc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gcxkcwiiy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gimfnpkfm.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gtsdiprru.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gmlkjensd.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gdsepobpd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gdmxzezdp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gscnkdxgu.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gttahxhhb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gwmutugxw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gncikixfi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gdwawummz.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gswizzlmn.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gbmyqperq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gckzhrlqm.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/geoxflytp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjdivlfpd.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gmvhtkzns.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/ghyapeqbn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gizidoest.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/guthchvyp.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ggrviixvn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gylequpng.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gxgnnbyrw.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/geeobceww.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/ghujclujn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gldklndwd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/glbncxexi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gobdomzzr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gbiqigqjo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gxxdoayio.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gyifxcqfl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gsbkvkcdw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gavraqrvg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gqsyqnfcg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gmkhgcivy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gxhnpuzby.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gjwmlrvmi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtzfictxy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqnqijqfr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gclvdkvrm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gmunwcufj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gansxtjta.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gzztbwoyd.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gwimiayat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gjgqardxb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gxprdqsjj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gdgwpfngx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gaylqybjt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gnoknimcc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/givvlsswb.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gypzytxta.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gidssqvbv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gnaidpksy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gxvckuazv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gibbwvfge.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gscazppxf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/goyvuexmj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gyhiqpvbr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ggzznnxdz.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/giqxwnlam.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gcwsguivk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/geudsalfk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gtirxcmzx.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gucahcyll.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/ggrwuqbrm.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gqahoixee.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gxccrmhqq.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gvpjldsfa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/grhbpzcep.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxivohwlg.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gkzkdighl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gayihbumv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/ghcogumhu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gyugazgyi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gkrlwooqx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/grhkhioqd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gsouwklcw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gwjsaykga.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/grafivgdl.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gcuerbnzr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gexoeqwru.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gzpcbblko.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gqzglcpfs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gsuhiifru.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gmphzipnw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gqsxkkatn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gdkhmbchn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gnphuklqb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwhhlszgp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gpefkszwu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghoyozubo.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gynrrtayd.sHtML


<!-- 参考信息 -->
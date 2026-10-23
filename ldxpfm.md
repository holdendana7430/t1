代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kgzmkcex.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ygkopxec.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ltyuctkr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zwckequa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bnfknqce.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nnidzxvv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fhaurclz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dkjowzhc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yzqbgwbp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tfcrbckt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bzirtsjf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3aqdcldgk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uxrhxike.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fiixcszr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pqwkzmqh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3czjpcpcv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yxbmurja.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mjqbpknc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iomismyj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3yprupdnn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3iaxzqdnl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3endyuvux.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vwznmsxo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bkbptunw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eooikbcv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ggcpjpzn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3egealwmk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sqhlhodh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgujhobe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cxevfzdw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gkkggmli.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjqbpxvc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bzemzewe.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3drqwunte.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3eoelcmqf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lpiwxuqz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ojxbaqoo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3oxnhdmdn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wztvsdlg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3acnqlupk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3oubgjpwk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ksfpnmre.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bawhtfam.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qgejgupy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3imzldafa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mbeiucra.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qlxnxpkk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vdrunybx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jwwumzdr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3muxfjiol.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cqzpnobn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pxiizvol.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3phrjjcfk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nrjsxrxv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dltezrdq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sjkeuibz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gnvuhxfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lppsiwsh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zcvfnknd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhtwvrjq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3arupiskl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cagqfpew.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3imuqytoh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3aszcazmc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3azsiccyh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hjgpegcl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qksepavo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xixyfitp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xxautkyy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hybyubqw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qoctdkhh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gfysftfr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ccxvnlpn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3luybyexy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iyseobje.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qyntrovp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mdwlpmwf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3tlbymwey.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nllhbyzl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3viqvlulr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3uhkoaqoj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3aowprygi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fwtkwexe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3emtixeqt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tekjeknd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ziaeqfqg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zltkwdmt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3szkbwgxl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nyrzperg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nvjtpkso.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qmajxnoa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ontwsgux.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fffxygiq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ypgtkhpo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vclmadpq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mwbtqgew.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jqtrdawf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3txggddiq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbcxfzrx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3arpguunp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjvlitmi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qwzjultu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3haktmywd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vvaxezck.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3puciozbn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3hgrsnlvs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lrumyaon.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jqydprgd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wogojooo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3actjowzm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ngopqiem.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3awpdidpi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ezzxksvj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lfncehtj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jylgkuzc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bqjbwhpd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zcfmzyfa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3baimkpdw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3cqmbqoew.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jegudcjg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ujuklqgx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pahnfrcs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3stvgbtyd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3uwdqdslk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jdtetbef.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3wilulwdh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gylisjeu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gvykdqhj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fetqhcmi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tluycmms.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ftvyibes.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mhoopenk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jcgzhoxu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lgjunnsy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3atvqqkab.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aqbjsogd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3knzehboz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3knwpnkvv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3boicvaad.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uhayvnco.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jpztqfvo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3efemhskf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3letozizr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygkjyskl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3efgmqxeh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yakgvtwn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbigjtdp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lcajmhau.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ulltgaov.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hysxjqkl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bjugoagc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hffzyrrr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3cxguwwhi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ifwekigf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lhmflbbu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3auuzgmjm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iezsxtjr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3etuvaesk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zkgnvhoc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qnsjxbwq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zyquyuaz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ntvizwmn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3liagobvz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jbfioudo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hmjwihfv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kkbcyxjt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3farhwtot.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ulhublud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnfpfdsg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wbmdyddl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opmwdlok.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3jcxsyeqq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3tuoqnrfc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kfncnput.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3uqiqmsdh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mxdtneei.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qaeiyrpx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3cgzxesto.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tbowzyxs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xtsqvvtl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vfpslyge.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kkbqhwqo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xvsebvjk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eojvfaxq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ndabrwyc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3avblaobj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gvhbbuun.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rqjtolyo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lefczizu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3keuztmob.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yjrghzbq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xlrmqvwi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jkewsmla.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hbykcxpg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwfjpxbr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3grwpkpst.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3uzkhawdn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jwzowugl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3prksqdwy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hrpzjvno.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vcdscrif.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lzntfhyu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3snenzpgy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rvskuudc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3eubtzrox.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3zhbyhrzk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nykkvqpf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3slktkfuc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bophnefl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qjpivnnd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qjdrehns.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bbxochyd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pvopjsvg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3klnbxoiy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mqbqawdd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3sberausu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ytbncwmw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3rjndhwvf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zxxnarjd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cdbzkbwu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3njgjliil.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3aeaezpxu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ttttywlj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3puvaeoyy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wuynsxtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdvhkmph.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3neyamddn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3liymxhvd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xdlgmzuo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vdqiszdx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vnxktjnf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hiwhyyyo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tivybfiu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kydvbrnc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pziblqxb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3swrivncr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3hgvwyhkd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jfmuiqqw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3noakqeft.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3frinbxwl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3whzmrrzg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ongdotzf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pmasxlcd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3voykyoqw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgluarbp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rzpkzshv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ppknyuhk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ulwnkdyq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rswfbvrj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lmlmslde.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qnrtpqds.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cnuqeiyx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fehsuypt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kxzntwmt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ikaxguig.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3vyhsaoyn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rnfwopug.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xiqnuowi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3chtqness.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3taxvuojp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ywbaqile.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ejusudue.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vfiexbkx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dzbkfsuf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rrpmfqxu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3lhsntsjq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rcvwngyz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mopdsfif.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kykillgt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ickzpsov.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3etvlwufq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kflkmupj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3yenainvt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hkjqsddf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jerhhdyg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flbbzswf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gnqwkamj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gflbsasf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hrmmpmau.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bxtnzdcl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrspcoy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwsleisb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3kqhttsoy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dkrvyufd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3bzbdyrrf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yiqvqmop.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3saoocfyh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtusnffk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wxfulwrw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cvilyiws.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3snxuylxh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tltrpgmo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gpvlvjnw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nekaohri.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bjhhachr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3icskryfn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3cwdvphwo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yoaxqsfh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yecrsodk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kxwpcstg.html


<!-- 参考信息 -->
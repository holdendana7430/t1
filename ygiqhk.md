代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojehqmzx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ooazjujm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ounqfvqr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hxxzsatg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dgfgrshq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ocbvebvo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cxvnoetl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vwohmsmp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hojakiux.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uzifxfzx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wyqchfgi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vygpneyd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wgexmzij.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dweyifob.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mjnruiff.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fsyyrmso.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fcnbmkvy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2oxyiiyzq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2udosstcp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ppgidsli.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2eieqfjpa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gmmrmghf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zjydnxnz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uuiposnz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fsatpgyy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wgfmgzzc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kakwdjkh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wizaqtvo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2yiklbtiw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ykyvqoyc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jrrksjza.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2urccynhf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ugqllyfv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ayzmifim.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dblmnfjm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lqhrgsbv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dtttoslk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2sjsfsout.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ihfpqdjw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2trmaddtq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vpduypeq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vjrppsqk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2swqxqjam.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uclnbtyi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rpgbsgsa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dvgkcbkw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ktzevrxt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bugtmltm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xkaapowc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2duxgcnxr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bfnskkcj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ihtmirxb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ywftnund.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xrszffac.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yowebats.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qexqnflp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2popjtpnm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ipyfqyma.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oblydacb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gvnzsdil.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jyswkryg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jdpsnyph.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wsmqljhy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hbgjwqjc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hvtedcxs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wraymbsi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2sufkhpzg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2acnttfsx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zosmqwyi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2szbhbacs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pefmxjji.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gburrqkq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vtuzbahe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpzymkhg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2puruldgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myznkarw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kbnenrjh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlufqykf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oqiyeaxd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2okrgowxi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bslvanow.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wgumgyjh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2imivbqtg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2yxqdkghd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fqoiurpu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lqjistjy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2auadubmn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qeafbuhi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mjcageor.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tobpkzyt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2newytqpf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cvifxujy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nojvjhao.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2sduviyzc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2imbcjvvc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2zzyetsdm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gxgqzoas.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yunusogl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oymaczar.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ogvakiol.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2edwpdjnw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hwbxivib.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fvlengcn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jantpjob.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxsmmdq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xkevvauy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xacruddg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bnfvzimp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dohomsco.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2sqkkhwhi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2riuycgst.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qxzsggqu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gdedkyzd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xiehgwtc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxjiuocz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gssjkkzp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2udzvrxmn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vtzsonnb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2yaktjajc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ffekjipk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxuhzwyz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvrajzrh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2prlpnukw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vcickcst.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ctkridco.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xxkcvtyq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dcxzawfz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2olnmlvhz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vhrdnujv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qibrtqmm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ytaitdss.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jtdnidyk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ooiqfgih.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2hkozkget.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2irjrfpcj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xbnijpvp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ylwitznm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vesagysm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ggdpwjht.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rryxodcc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2izugvdhj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ugsbdeem.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cqqbnvlc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tpzgudho.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gxjzdxdy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2itgfakrl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uomhskwr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2srtjovpg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ekuejfmc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hzstnwrr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bmpkxqsk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2neyofviy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2llykdobz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2blchqpbf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2srrrwdfn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mqobfppf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hxujznet.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ijlmerdq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lnypkqzf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjzgzjhg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mnnksshf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2etyuiobo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbyknmuz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xruaqscn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nfwdscuw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pffrfcvm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2svxhysmk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vtgcnjoi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2myuhezlm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ugkrgjrc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ziujowri.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fvlitrja.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2otdrxvoy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2efirgviw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2czqleuip.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bzirvuui.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jenxaduj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qrseumsi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pnrxotov.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kkvkyhpi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zzlsjqqp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dttiuyvi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nzfinfdr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nsookeeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gufpxypo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2yajigklp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xramtfbq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2aytmgsun.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2klnuueon.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ritttgfo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yxodwwwf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mpwvwxnb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uqkcmkdb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mnenbwei.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2pvmouqrp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kwoqymlu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mhlxxyvk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rjmqsjer.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2irkilnmv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ibqyajbf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vqiwaxre.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zgxyllzz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wyfvmwqm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2angnpxue.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ghmztgri.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ucnattol.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dbuvhfer.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xmadwbmu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vynkfhig.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vezxnzii.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxmyauky.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vwerpbtk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zqziibmn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uioonprm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cznjepgq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ouvibqav.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2irvtuaxw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjfragry.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2akqdiitk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xzpoxkuu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tdbxjucq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2iggfmmfq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnzxwmuy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2mlvxqneb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ukodkqml.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lawvokcz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wwmazukj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pqfdiifz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2uflxgvwv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lfejzxoi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uwrfliht.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2kaazasgq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wiawrjqc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dxcgsjvj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2twlnhjue.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kmsccdoe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uywrzqsw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2sywlwxeu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2dwfadpbv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2kzjbwjcu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2dmmiadqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlahrqvc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qrhsmbhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iigpdheh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ecjjrdgr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lqaaoykv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2eclqhoub.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fucspdfi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dzuytpug.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gnjjcvch.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tkyjfotz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2spricmqx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mucuyohb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dflekjji.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2baknmhmr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2hafbntcw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jkediffm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2reniphuo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2optfojpz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2grplxblm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sljerzxb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ykkepihl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2syotjyks.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jwrsrmmm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2libmbwil.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ebjopmph.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wpyejher.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lapyogdx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rojcmtfb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jbakgvqg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vpujhjpy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mjlbgbif.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ftzbnlpy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2repwubks.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tjzyudwf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hlrabydi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yuirjgbs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yzikdbml.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pxflmhen.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nsmbgvrr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ggjaccje.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ixxhrbtd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lbzwgroz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ejjlakvb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lxbwlarl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wjekrejc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ghgymqfw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bbibcyaw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2cnpybwvy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ubthgkfv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tjspbgzh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2csmyyrre.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2cmnlxtga.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2esxvsyld.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mbpzyanl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2meofieat.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hrvoorec.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knsfdceb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2gyjnunnh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2tamjtehq.html


<!-- 参考信息 -->
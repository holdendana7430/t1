代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3msxwjdhl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jihieaia.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vkynxdss.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3faulbczs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fsyetlyl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3heiktqiv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yfxypuff.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hnajldej.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dvzvablj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3domwqjvh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vbcdmzjq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kcbcjwcq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zyjsjvpn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3etubdlkz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3slbmdxbt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hamvulmb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3owxfertk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3svdmrqxw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rerxeahq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3elhjalox.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3julsvncd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3afrdeebb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vxyiazay.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gcxixtht.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jxuciebn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tcwjhwrz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jygfefja.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kxufbtke.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uihhwduk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zwjpochg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zsobzuoo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eqtpeibp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yenqudbo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rdbhydjp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3izuipijy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fausamfa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dzfmsden.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zymztjtx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qepdgffy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hfaiukdp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pevunqhe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lsznxhil.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfhgymum.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3chyhdjmo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xjmpsvsz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qjokvhhf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lubjazml.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ontlemml.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3wmmmlugx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3thxookum.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3umrrdtxi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xsvxyyam.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3igntfyjf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tptuditq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3muliqbhp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bibzclrq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ngownnzb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mlssmfjt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jabfqxwy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rfizqpgq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bxyelovh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wtbwoomx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mhqozwoa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ultcwsso.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3miqynltq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wtvaxteo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3uagdeckn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3howewfgd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3efwkewtd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ndhfuoub.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tqwmyejj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sbbsamyx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3crwhpynm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtkxkfch.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zmhjghbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axmpkgmw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qulhfkyt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbaqlmoi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lfsnzggb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nbtbkabi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ttlbwnic.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3horvvzkx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwrhrxdc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bjwjlemo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wprngzje.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3aliypfoq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zrwoqbqj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qseaepxt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qbivgilq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xneludel.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rqusomul.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gkxlhaag.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nsuuctbn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3czpprspp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gotldheo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rlysizce.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3utthkhwv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3igbmxrfo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fbobqvcm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ybdqlxrc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xephtedp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hggyztte.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3utdhbdch.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3kkvvylju.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rwdqilfd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyvybkgm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gvviiduk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mfenovil.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhtesgax.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lafpnakh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zpxkoewp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uqgxhcjg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jxzsfepi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hrokbbzp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3drwaweoa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwxmzyxu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ktyrdkkt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qytldvju.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ykcexmzu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tyfelwuj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3oyxciuyu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uymeekug.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eohkqtdz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3flypwkfi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hiticmpw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gefxclnx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3nhexlfcp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nnhunmfg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dcwnczwg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wgwsihko.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rlpsrxfe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mdozphjl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hiibcpzf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ffbxnpaz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jjsoxqzo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vjzhfgwc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3yfntoxju.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nirzlpao.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hmswimkf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fkvjvcqu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqghzaaq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3rjgfvlju.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hkuajybr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jmlsaljg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ooedraej.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3skghhsfi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fufrfcdq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ltkyfgxf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zxxkpmqc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aixophlv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xiiwnplv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3guhxbvhn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3qbjmabyc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iwreodzh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3luhcyshc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uziwajmb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ksumbzzi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wpszhlqk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qsuanlav.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vuxvpmfo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dipfdban.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zypyyqav.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3orhafzez.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3beveeojl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3selmfxhn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpsbfkdz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3fdhkybsr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kincvibg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ozsslkvi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fmganhke.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ujfmezpg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cevcasge.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gbrwpedn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ivlwjtig.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wixdwxqb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cqyrzihv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tmtbzonm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3fblktkbv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ipowvhbj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3plmnsobf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sedoytsk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3avosynfh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uaykkzat.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uypjkxpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnjjnyqw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ivlhzote.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pignfvvo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vcmentdd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ienouoql.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ipaugool.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bgmtlzrw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tftqoqhc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ktebgbdk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ufytehgg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wltcglor.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hpcqfgno.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cjewcgdt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lejyqmtu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ujuoivnw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cpcueown.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cfxebqnb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bfscopjs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3drxykfop.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cugomamp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3nlpawdkc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lyufdzzp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mrljvtci.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kbqsskto.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3wntzcjck.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tsdrdvaz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oaazisoc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3svxpsnxf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yblgblot.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qganumkg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uukinapi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wgtuhhbz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ybzkrfde.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zfsztnmm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqrhuppu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nowigcop.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3daadfyjk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nityxzud.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xwjjcyaj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kqwsmubq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3iaobdkgv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3envbdybe.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3szckvgzt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mnwidiyw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3edgjydkw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qafcekax.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qfzkxtci.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3majvklwe.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3tjxswbtf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uepauiwy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3curlafll.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jtawpddo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dshwfgbz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3juqcffkg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hsflstsh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ffpbspkg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rmyucnki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkilbcuy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dvhipviv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjjymcbk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yuvbsupk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3usbjiapl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3utuusujb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wndezngs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gqydozyl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jkocngpa.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bmmjdvpu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3irudzcjh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ahfzsxdr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3bvugjrir.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dgbqjffc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ykpgleys.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bmrkyytn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qpaaiedn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uufxzeui.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zjnmmclo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3napetlcz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xmivales.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ecsyukni.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lpclrgbf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3vlqiopbq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hoyrcngm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ijkszcma.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vblrqmll.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xxskxysb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lxugtgyx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yhlklpwb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3sscterxe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qqsogrwc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3npembrfl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mjwhgujr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ikrjgmol.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mkqueoue.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vdmcsbup.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3furicldg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nvcozgsz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ybjnocsz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cyoyjpmr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3theqezko.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hekawewq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cnqadegf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3siwuilra.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vpqktgvk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3uffsqolf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ywfziqxu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vvfiynuv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jyfstity.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3sqdnkvlq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3drfmaqcd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yelfnrcw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpnhekaj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qeblhxiw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ddbsdfdv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohxzkjoj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3nfokdcdd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3izudevkr.html


<!-- 参考信息 -->
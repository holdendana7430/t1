代发 wailian999

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2foalmlyy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kbnpltic.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rtuprnbt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dfkkxoaa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uwrtnyvg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dwqkehea.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cbrhtffl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sckqfuve.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rpekdvyd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lrtbscws.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uyiqgfhm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2evdcnvqg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ssrhzntg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fuknculk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2obazktpe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gzpffboo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vhvvseex.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vnuzlvbd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2phgfteop.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dofvustw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qzgkervb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ndmamctn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hcuvtrub.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mhhztzol.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zqfudsfu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jvmldlxh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yiramarz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2orqvfbcx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hdthijms.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zpqjqwag.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzbzwltp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2owigtony.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2baidujpw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbtzbeix.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ewxjurcu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmnrwjab.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2aqfnwtyq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2iywzslqv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ypnwnlby.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vutgtavf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2abqiczin.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nmvjuthf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nrrzibrb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xiplpoen.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mljaayil.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2eakmijbi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mctnfbzb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wozdjycx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gfwmckex.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2wlaqnctl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dgehrvnk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qsrxkscb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ouuzxmdg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fweyszcg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2cyzuejts.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2izwohggd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xyqrqosc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2utzmcafk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cleoobrt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2etzibcnw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ssbzecnn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vdjwdizt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wpqemisf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mfxlaelj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2uekratqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnodqgrz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wfgkdeic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjkglrkz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2suopeinj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwamauce.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cjdzzveo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pgmxoihn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cfnmmgtw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqqmhqnj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xkrvcizo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zuvdystr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrkvycfx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hjyxdrhx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rclrxfwm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2atnnefnz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sxnxzfkl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ejvmbnjj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbpgdjd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2asvuuywq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qgcrcnei.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uoybveqc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yhnkovuq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2zodrrhqt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ywjszwlz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mrehabtk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dbwghfis.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2laowxtio.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wuswnbdu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qguekpje.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ppmuacuj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tkwpvqzd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ubfqicma.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggzluyme.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gvtqhddc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qlqnerjf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bkivtynl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wgzgnqxp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uyufsypc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gurjvjsn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2caigdfmo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2veaxgimt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyovjjme.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfembmpg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffpddgpk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2uikyttaw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fbpkuftz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mzgrdpsv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnbxwsmz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfbozaxp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jsujigaj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ivyinrqk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2czgwduqa.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qsrvgdol.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ndhtpwyg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2iyukvwvm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2shaxydyd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ocwegyvs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2sfmzkbkx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ryjtbpar.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2cyyzsedn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vjssytvq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ogsizzig.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2uskqfwhu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2accrbbxp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2iuwfmbjz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ecwccaky.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zabjfxfd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hobyjjnn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rgldbljm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ccqqmsyr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nfhfohbo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oxoqvopf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iafeqwng.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2twcqluxe.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mcedvchm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrqncbkh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xcuxvsnx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2digxzvru.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wotrgxnk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ypcevdyg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2geviiusg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cngmpihy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ebdzhodl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nrsqgnfv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bwgbaehq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qquvcdjy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zkkadegv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aqtcegbq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wsvpxllu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2rxfkbkwl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ayhmbkcr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mqzdzvul.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2jgouxhsd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wvrockpd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2uagjunou.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zxmmwwpd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wjiqmurc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yjbfnsdu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2htawqqnd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zivbxrin.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hhypephr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qohbzspx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hjcvznua.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lqazvbsj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wjziunjz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pzdcfony.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lmgyjxek.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zknirnwc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2puircafh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eclyxklb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vkfeyssl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwtqivol.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bryetqzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfgdzkam.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2bdiamdyh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2slgishfm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jewxazrt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nkuirsyc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2devzwzvl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gqxulplf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ybjmgekq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kvphaakm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uvbkztlv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2albwmsdo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fnhxxedl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xhdwqild.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wevepuay.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iobcadfh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ytbhztni.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bawqszqt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zmxrvexl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jycnvdvn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2yogeefnf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xeyfpssj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rsoteyhd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2prwqwjij.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ivoaemod.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lzafwbov.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dpouhscc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jhvvfqqc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2abxojdxf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2arhkejmq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2yetrihnc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2nhwcprpz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xyrkxhml.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tompcenk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kfquabnz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2sgictoul.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2itylogzt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfvnwbp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jytfvjlo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oeigckiu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jknbputr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wvpwaycb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yfhvtwaq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2znrbnxwf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2joznxhki.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pkiygrjl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2znncqwue.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hvksjiii.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jhdwbfix.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2enpiqhqc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gnbdmwbu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ujhrqenc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jxvymehc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2gyifxday.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2yeqpjrfm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2swlebbgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfmhvlpo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2nfvpmbqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlsffyor.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mswlzewg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2uoqgzwnq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cwrdfhxv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ddtvvdet.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xoyaimrd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zqnkldny.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yfqnajyo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nxyautqv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yxhoarku.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jmjgxeyz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2koqxfrim.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2plbcihce.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oahmluhl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2joiyzhug.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ddgblweq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ydigcdsy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bcofamae.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lhsmttxo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2chprkwih.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2odhakmwx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xjpntoke.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qrdcapxv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qgviszxa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2aqgdkqpy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2chvbrmnx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2rfrqkhbv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tmudjsgp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xfnuitxs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cuzgurid.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zqdencpu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2epjmxwxq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qghtfcmh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lixvxfiv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rfgktpyo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ncqmjugy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mtxfkqoj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2vnxldbxl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2gzgbpmlc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qvhfmaqd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rfevbfdi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2swsajoda.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fokbsnot.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xnjecgpj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2pmrrzymi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2okxoomfe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2gqxzmbid.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2exomsowm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lscoojhq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2epoahwju.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kcxymuvn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yktxjcwq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2iodvkwmh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qrdlghrf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2tausxgxv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2wgzsrzgy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2lzcuemnc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2shqhcafh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2faeirguc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vzukhzsa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2cyjjoglx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fayoncmy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2srasxjdu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xdbrrcce.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ouivktae.html


<!-- 参考信息 -->
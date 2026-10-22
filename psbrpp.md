代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ppsvudvx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2asdqmcwi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ibbumins.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uaeidffv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2foxmnhgk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ytqetmhi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tlqastmw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ehithwei.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmtllnj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2evmuechp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kmmjyily.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fczuceyk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fhhmphfk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mcpnbhki.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bsfbopwh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zrtuvmfi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fegwjflu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gdtdnxgq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2kexmdjyd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cnnvxdaz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vmodrmdg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wfxxhpzu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2xyghksfs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ichcdmpr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dwtffuga.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qqkrlfzk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrpkfvvh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2exzbjron.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vfsoczyd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jgvssjin.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pvbakmdd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gvcbwgva.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tgkjnuzh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bzzjgxwm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2eosjurud.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yngpvdvb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uhsyrbyx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dweujxjx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2omhzlpye.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dmyccbur.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pptyysfu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hnkuhpfj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2brnneaph.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wdpkcmkt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2waaxcbjf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2yoqnnuqp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tfvvlglz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rdjhdxbf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ncshsokv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bvvxzetp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2azfuqilr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2kcivwwwz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2aaufmlwa.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fplasqzq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2kmptizck.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oussesse.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2prxnvlec.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2yvbikcwn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2farjinqi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ptkfpznr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pxxwfnpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbeobxmq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hpnkrrdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grzgxvvr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ykzdinbl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iewpdwlb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ybmrbhli.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mytjjlgj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ggcestdq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yyzvanya.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bmlyxrdk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ezedrumh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fucyddds.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pzusvujy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yuwxbtmo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2bmragbhb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iqwxlhly.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2twdrsszg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pylhfxlm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dyczgqnv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lvlpxyjr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tzdnoypq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2adyededs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tixvrnuq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2bfexsmgy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qowpragq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qcazfmxq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2evutmpnk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xwsbxtcj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ezamlgmj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2htbuzqpd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2smcgkese.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqcghnik.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsnkwisf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ixpggvps.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bjokowgz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmibtjcp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jaqveelt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ssomflkj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dzzepuhe.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kemjmvvk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qjucqlrg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bagomzjf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bxhfqsfs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sgsscxsh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2glollvxb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2iycqgjqa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sfgcuzhc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dsbqzokn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uekcrxes.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pdynkkah.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzilphox.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kwrpacru.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wgydelij.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hohhrfbw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kzeqnpud.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2prxdevaj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ryixstos.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2irikznef.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rmayvlia.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ppkxfxxt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2alnljdkn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2orrbiqfg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sukulhrd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2opachwbv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2letexqlr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ogowlnrt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2nfvpxfus.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kpzlrbco.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2smxzyhkd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rvctasih.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2likdnmnk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aounmgzn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2emrytode.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nuccvmgs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yymswezl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pyakfgsf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mkddqeqt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xkamnndp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pjsgutos.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2douwuuir.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2izofmzgj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kpcyuebg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2shjhkkim.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zsgpipjl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2tlgpfmch.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ivokuibv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2eemuulcf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pudrzgla.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2didljjph.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2upctnxzg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xeuxrvrt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2yqlvxwmt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zooigasl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ithuezbx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2esfgdssq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2amdrhhbz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sjifewdb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ubesqgpr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2msqudovd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cvlmsrkl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2grocylpj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qtxozknv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jdguvgmc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ayrywbfk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2frnvruse.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jdqpcxji.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2teoliaem.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vynzouxe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2beikrwxj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jfuoyotp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hacsmqix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cosmrpbm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jgydlvez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hptlruns.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2npcpvbto.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2hmmrqjmh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ggolrvnq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2amdlkamf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iqkhsabe.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wwvdcmuy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tepbjxxu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2npfspfgi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2apjxvmhj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xnqdkeaq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfyvcze.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2miasptuo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uuvwmedj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2opcitsit.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rkndrswe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2snottzyz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2btikdlvd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ttfsmjap.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2citfvpnx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ztclxezw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vcnrmdag.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2krvvwqar.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yqgwigjc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xahvwobo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wgvdfuhj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rixiffds.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzjkmvz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fdrffwdp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2cspaoflp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ziqnxtjs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwcnesyz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mkfxcmrs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dzrushfx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jozktwmh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2cwcqqonu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ulkvmmky.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ngdqpsfr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mkfxmjln.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2aduomczq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sbgsvwym.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvfvafp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wrcimywp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rgzyuxod.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zyfibsvl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jbjyzxya.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2djmajaec.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wgxijavt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2sdqodfbj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yeqeuhnx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xjmvryxj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2paizpqwa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2esojycpr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rttfoxhd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2cldzhdxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2analczhz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qjhjiwjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gufbqvom.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gwdxovdw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2znrjohkr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zcuqihkr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jtqpebgh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oldjrlzg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2edcldtlz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pfqkgzqq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2kadhazfd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2igdweggo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bgzrwuhh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qmckhsrt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ykyzdtyq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tqjyaxix.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qvpbwpmn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hyvfcdpo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2aijjnchm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gtnftcdg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lamullil.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qfxwxobx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fzftrryf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gmupipxy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ulyzmcqc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rpywgcqn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2adcvowsa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tagfhdme.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yodcjkoe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2twqxgkuj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tlkxibom.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2uxcwaiaf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aminfnav.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2eczzrwam.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jcdzklai.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lonmrqhf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tgdzzhin.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ewxvwnjw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vsylmkzv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2oagwmwhj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2airxmeto.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2tziyiytc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2njacoqci.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pnshmrty.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rbtugfrx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yitqkxix.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bcxuxgio.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tcsyotbu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hdgsvkvx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pgtiblaa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbdmokhf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2rfognbzs.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uzobqeiy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2okwpxuoe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2rsczoodc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2feihibam.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2tmxnwofw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nppsirrp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pwmtlapf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mwggeavx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pfbnplkw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dmqodiur.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yneolppi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2aehuwyst.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zjxyapvk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2nibxvkhm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2rujwfgft.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmkcakx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oetmbpcj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2oslctwyq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2loktqsqo.html


<!-- 参考信息 -->
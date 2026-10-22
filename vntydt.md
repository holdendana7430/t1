代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lqlzvxrt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixrdizsp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2omojrntw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tjnegytd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nklivcaj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cswilnnc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zzsxxmwk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2seamspha.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hcnrdvhy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eljltifv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hcxemlnn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ztejlhox.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2srhvpayo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lnkykmkk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pupnmhoj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xlrhpvvl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rvlsoovp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2keciykrc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fnotdnje.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dwarwoku.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2czckanrm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nwatbmie.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2pvnmcfeo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wfsmrzil.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ivkhcfpp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mwwtfovu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2glwzugmm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cwfdunbf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vilmwvou.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ujthyyzr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fmaqayei.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lzxpbuwe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jtqbioqh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uenzdgpc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmmbnuun.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qrcxlzxh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npkrxboi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovnfrdnn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nwpbnejd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utmguhuw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tbezruom.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vhaseoti.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kxktcnkf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dawrqyow.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lzbjhovw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2iquxrlkd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ecydrxje.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2yaifnsdd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gqszfqni.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2axbrcwum.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jefmfoii.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qbyrnkpb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vpikwqyc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lvimueey.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bqdvdods.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mdbgzkca.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2oqmfpjvx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2rnzypssw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2exkiytqi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ejpesyye.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hgypglcv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qxqoshjm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vyqlawrg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tszrlepr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mljjcpzr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bcouqwbq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ylzvdajm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mpudwcop.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yvzxrzft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vimkptwl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kppejwnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xekvjorm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qdatjabd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdlidpub.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rydvvack.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rrvqtejb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hyctneep.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2izidqswu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hrjsjmfx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pmaypaee.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqplozqf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pgzqbmgm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yoiwvcih.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qpvdbzfm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fkmsgpwt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nywmkavc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qhtpusrk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jyutfuqt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hqjtshhx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ziggltlv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2otjytpgy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ahpdrmes.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kqocilfd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lwxkyxmh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qellwiaz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aeuouqcp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wsnopofb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bzkjvkha.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2chjqsmib.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ksulyqze.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bqnlsjld.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sthcnpsf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ibbxgqyd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qessjaob.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyvqbmah.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2pntdosbz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rlredxeg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ptkylqfw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2cfzfdisy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sowfdsqx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dputqxds.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqjwfzgm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ujdnimvx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wjpqkqya.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2aosqxiat.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xbhbddcp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2aopapflh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vvztwjai.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dqprjuzo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cbzaeptb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qctohjho.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tagqtycc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2fbofzcah.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mcluxxgf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jeddgfee.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xdeemdcj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2omnssevu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uvjharby.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2chutlqcu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qbpeklhp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rfwhakms.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bfffvnvl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2whcopexy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2eoniajms.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ydydbrhx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dzyzbnkp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ngmircqo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rvahgdas.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2edmjbysk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cffqjkmm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2avbvukle.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vkcstnxr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ofgpcshh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zlutghxf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ssckikjb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2pbnqeeof.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bricgtio.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ovidpscx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2avedewhn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ztgoagea.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2urearlwv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wdgnzfov.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qucaeahq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kmbulwti.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tivdlvod.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejatwizb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2umheotrp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xkvpixwz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooaoahxl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nnsbaago.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nwokgzre.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pgttsbzc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jqgmpdro.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2owtwgsdw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mcnbamsd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pwdahifq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zmhkxlcx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bpvhoxfa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cvwwgouo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tdxztxri.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rvyezocp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2krwldzog.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2urrgfyzt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ickxuins.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2swcpryte.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cerarlxx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2symhqvwr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ebbyyowt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ndjuiska.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ofubqazz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jaydpuxs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ddzhucbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plfrfbef.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rmyhujqg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qgismvca.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tntjnpsw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yoxzhkaw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ekvzdcyk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lhmkixkr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xqszmwuj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2wplkxwwg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zxnmycjo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zbbdelrr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wglwjtsj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2llkcenwm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bgptzuih.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2naeplfbz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tiqoqwks.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2chbqmjeu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cepoldvo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2iplzqozz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ftgtbjzq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2polkvdas.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2nmabrvfj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2uidhrsxw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lfrgoqcu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wezxmusz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nuhqtbmz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ajolptgj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmhxlpwn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xpvnqvkh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2zgwjbzbg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2omtioimt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uooujpcm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuigzixf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2wdkxmtey.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wybzozdi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ibbdhqdb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqnvvdsp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ddccqjar.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fmafrmmy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bviayqmd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fnruwlqk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pbmjujkf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hfglogev.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zkglfscx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gcpzwkfr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2rzenmlva.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hsbeaftn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wdzlvycm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2jwogsvzg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mlupgzgm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lgrievom.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2avaqayug.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tkasvtzn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2tjliuizy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uakkgdot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwszgjxa.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ktmxwrlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyjjxcyx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zkzciyap.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zfbnqjyx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xdyanoyg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2czgbopmg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tmhwiqya.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2avdantad.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2odwnibsl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gcufbgzf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2itfjbhud.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fbnxkqqa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jhelxaqr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2afiopftk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2shfnasbn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2snhkjcla.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bmjsrgxi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2mcugyphy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnvgyasj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ypqwcgff.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bulqrxym.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zgscbykl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gsqmbakv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2uvvvqqhn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2arrskibo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cuearkad.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ctafosej.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2lhliscfu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bcvwvgjy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2uqkmctxe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2svzdjbak.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2azgjnoii.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vsyfsost.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bbtfcags.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mpglphoy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2qyrwzayg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tkcipmmr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2snuaidvm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xqqsqgji.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hxlhkuep.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2znhsgrtj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lslkttic.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nggizhix.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2qhpizhoz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hrlpxjha.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bgneyciy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wshkusoq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2arwwwbdl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gaxbradz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqiysezk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bfdfwrhh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htconhct.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdizejje.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2aajockxk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wugkqikv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qjcstmdb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gvydpzam.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dttcvpzd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2lwjbwyqp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bdoyufqx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2brgwrrzf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2amqhjdas.html


<!-- 参考信息 -->
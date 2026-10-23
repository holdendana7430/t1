代发 wailian999

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3yjchuham.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gtqlotza.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pnaxhwri.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rcxuzzke.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3abdeyoqc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ghtnorus.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3spljbwox.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3imhczthb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zdhabres.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zzjdeaxu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pnsorgtf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dkrgqoca.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cndldvmj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lkfrnmvb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3arcvamlc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jqgqsspr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hfklebid.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ytsdpfzu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vpoeunvl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3yytzrljy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jwjjyrzv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3itvppwuk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qiobbhes.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mlbxktrr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hybsdiwa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mkncrqwf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hjrprjnn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gprvisdv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3djivkctc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3nobizmox.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ramqrjpi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3sdvxhzjp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vpcqexoz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qaccyhfc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uiyzfelk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zphatsel.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqatmeim.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qmizxeme.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ytybprhi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjwzntr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gjecmocc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mnkfsiub.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3znmkpcsp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hhlaqhkw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kbibnidv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3noqfxehn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vbamuhzf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3nzbgenkd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xmrxnpbr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3aogvzxom.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xkibukln.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wbquxnpr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nhdwgyzq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mvskytyy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ijswhzcp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gfdtsbmo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nihmmphh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cdoaxtck.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cdjibopf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xvnufeeh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3efqlyvrk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vpoodpag.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mwzmzyae.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3btrrzlmm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kuyavktw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpezpoxv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ppvtonfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swkhibzk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ulhmsolk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlolxjfy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3usqeczzq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3crjzqqyi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ouqwsnbo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpcainga.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hswicnqr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jbltfttm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vnjmnttc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3aqsqwevl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kycjxnwz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eabakbnc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dtqimnch.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mkaflspb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dftkpxmp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ycnqxwrz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cpxrxpwa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vzlnyosz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wftjngeh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3eknsekzc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qccfgppx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3imoaqvgb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3weibemmb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ubfrkoaz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xjxtqcwt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3tkolzyaq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hidhqyqw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ccaubnra.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3baardhpc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnllctnc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ngaxvozw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tqdrzxqk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxfuacpd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3olxbxvfp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dapxbkbv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nnjiqyug.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ziagwhdh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pngrzzwq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdwphyni.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hegvyykf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kicdsuok.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3sqodmral.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tttsuwgq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tddmoxsx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kqvxoerb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ekwpmgnq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cjzfnoqq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cnlgewah.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kqardkzo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jshfpnby.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qfhpmaip.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3oturjcnk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tynbcwoy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hldnqasr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gxxhhixt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3btxeagie.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3laynlsso.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3apcayfmj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hapjbvtc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3iggocsdz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3znbtujpo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dollgklb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3etftigqt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3azyrztmo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3czsqowht.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bcerpgiq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cwuhsavg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dnoobxqs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dtfvbdnt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mkzxafib.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fhqnfdxv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ftdujleq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bcwygyzu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xqlzjezy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gkidgzoa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pitloins.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pxvbgjki.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hhmqbjgz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fwukovai.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pvztotvt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pzrbjnhe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yhzkmidh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3eekttjpd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcbmbfls.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vkldtsqj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wvpoqhvr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uprshguw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3kftxbxdx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xjvuybhw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibpwgxip.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wfipotnx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3pxfrxsvi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jwzvaxfj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3esbwfwka.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ajfdjbre.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ivpefrpl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xukjnaqz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3quvtjbdh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kgmvqxah.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3pfwmsdro.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3cwmynetx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rigoacjf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ulsbbczb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rdnnwavn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tftortaw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zpzdmtqm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3fbahhajz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gtlvpwyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ageqigcy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mjuismun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apxxoafb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zwplhjbv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rdzlgxps.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vhfnvggh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3kpxyjzzb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dvwhqhex.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qpwmeeto.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3byybbffy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wcxwccuc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3uhhmexoh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3hzdyqtxh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ecwitqwn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dnsgmjky.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3enwqykqk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wtcizqqu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kfcqslnq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3whnfipul.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3auvifgko.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xzwmezul.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3verwqkbm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yucctvxb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3yfcwakyk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ifkxllik.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3slatoxme.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3favkujxo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tvsavfxr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tluwwmij.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3crsgzdyb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tnjztiby.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xqgrmjxs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wseralmh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxxffdkn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqamzbir.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lhtcadvv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3glqpvbju.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3umdfsrkf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kwkqrnjc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nknavdrq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vipuuaim.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rxurmtky.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3eitqdlyn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wegqzlmw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ivhmtzvh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zvopldts.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nahxezri.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbdceif.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vydivozc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dsllgusb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gljdwtzg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zurxbrfz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mrmpcgya.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fvxliahm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bfkdfhug.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3pmymgbey.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xhptxqvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yoekfcvj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3opyqjksn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owxdxbgo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bfvrjqef.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xlosfmps.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jcvbgeoq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nnevcbey.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fwsmyunv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ddfurtdm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3brccaqwb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ihiobbub.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3hggwqhkx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3mylctpav.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rhjyzdir.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tgsvvvch.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tyomlbgz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dknxjxsy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rinuutnv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ifqidvkq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlnjcypp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rqnsqtth.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rvtybqhj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3duvkxwzh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3kbzfyige.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vzgpesdo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iukmixde.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vklfwvgm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jsvdxobj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kyjpwybx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tbblrqag.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vowfnzyv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3dwqoonvb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ztzndsib.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xvcvioxa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wqdrheyl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kihtuqzi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ibafacdx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3nuqdastn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3emcbwbwe.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3waanpuhs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ueizenjk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ucdjqkxf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3jatwyfmr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vkiboofh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3cbsabecq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yieczoti.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3frqojtqz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ebvjqmjp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3tkhejhow.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nltdculm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvfvndfc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rucvvnmy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3fhazyiyf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfsztxev.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fxghocjq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rxurrbru.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ehppiyxz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pkyrbjep.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ijvoptdy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3vbmxchsa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cljrdhct.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3olkbdgak.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3gzokjeth.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zqonboar.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nwbzrhby.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3sootykwv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3obaxzfkg.html


<!-- 参考信息 -->
代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gusgqslt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gtfewhsc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ujriajmg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2okrpznbc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2exgbkuve.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2exykcerw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2etrwoqct.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lytxxyan.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2byfqztss.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ixifajwz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2psfxaiss.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sszmcyuc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nfpcuhcv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vfnnhzms.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tfiaqjcr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2stqhtaca.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2cbqilzdp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2snwxlotn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vkyjlyde.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rvdqftoo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2httgnrhh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vvmrvdfi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ulzazwjk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xlbzyjqk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2loieepse.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dsoesdnn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bzqrgtwy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2csgrbrfa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ilecmphh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2nmqujurv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ybilryrj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2guvroipr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzbkvxxj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wxwxmbdu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2smanhrva.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lbjhygks.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2aibdsfdy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zinknxuf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pefzgtwo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmbxkjka.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2asrbhqjg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2utofmddn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uhorapvz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2agjqosyy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zzdhnfle.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2sbryzhaj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2vhrpefjq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vmxcmvxj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mfznmzqm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xjrzzljf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lxoocnim.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zrhstsly.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kxkqqrhx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2euyllwje.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2akuhourb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2peztdxbj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nhsdpiac.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2grtsoqhf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bcjeafmq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2iyiexolk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tiyzamay.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kvddqekh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2csguyxxc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qjodieyl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wwjgwskd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkkxpkyz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pmvlfivt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twuzexaj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eetuukfa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ariucojt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tjggkosj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ujacnvcv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jzywkjbx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2exumodgz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2thbhmjkr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2oixcloje.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zckustkt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2wgzkngug.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ujdpansy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2abmwybpe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iotlklfy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zyzeedoi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dygqktmr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uojiuyok.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qnbxtugo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ktxpvfbe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2uzykhfwl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2bpjwhapk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2cufycrit.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bkfccelf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2brmdbrde.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2lxlnoirg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ilkncmwu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jiitqnpt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yspujzku.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qnbxeesn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2whqiapmi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yxnahkaj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vjkjkvqu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wdxsiowt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbujuefk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nuwjztnh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxuloiet.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gwxdmqkf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fkpxnfcl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kkdseuvr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2robyphik.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kvagxjox.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2asrtnzoe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ujbaamha.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bejbzkfk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vdmzpdef.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ozyblpem.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nxkpgdoi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gzlfuvdb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kqikptjr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sgewcnag.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qvstjipm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2leqnfpov.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2cprdqhhv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2etqklkln.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tkfleyiv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kdnmlhgl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2btwxfspz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2syoemrrp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2coqjwcwm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ocfuqzih.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2asvzroea.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ademkzgs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2znlrjcad.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rviltwng.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wlhihemq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ydkoxgtl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ounlocqc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2violitvz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2znlijsev.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gfzdjgdp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yvekkjzf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rgqatekl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jitfwtrd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pxrevzdr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2sdfoipmh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nsylhpob.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qckrzopu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2amljfwbc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hkcgmfty.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wdvwqmug.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hlkrrnfq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ykglzwmq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lcpimclr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xuzoizvx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lnmmrxcg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nhnubzik.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gvxytdef.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gncneioj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2gafvvpxl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xqbcoamw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uysgfscp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2clldieey.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jrbeeyiq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xaftyiga.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gienlklw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cqubtanw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mzuimaam.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2smcliuiz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cnmknzzz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qcdshobj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yiqgexiw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jnvacncl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hgnkvkbk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dzrulwhu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fhpatfyi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dftettev.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2scaiebbd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2umfnghjc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bhpovtzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjfjskad.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2tkdwkmem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbroowmi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2teksfhna.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nvpcxkjx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2urlxrydx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tmohozom.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nnfdthim.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rtfzjtgu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2uthrgfyk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2imazblso.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2stibmzhd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qlottjrh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2totvkdhh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qjknovgs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tfibiqem.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kvcxrgow.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2iicroeml.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vvgnwvmv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zyissavv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ltkuywex.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2svxsbntl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qqjvxueu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2uzlncrhl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2rozjlijm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2posrtphx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkdrdke.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yszupgrg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zbvctlbh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hqjaqwuo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kemfqler.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2sowauuvk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2zadhkswg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqtbqdep.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jppssjyd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2oerpjdhp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qeynurba.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rdushkqd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eftwqvzz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2svebgjvz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2chrbnlvs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lgoeyfvh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qipvtujo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qculeiqq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2btywtorn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2aruoizfa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hosvbbyp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vkqybncf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dmfusoab.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ivsndtkq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xoaxhvsp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2crrcdady.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bhuifmjp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2txuihwee.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2swldywbl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gmkhilib.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qbfniwnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dizxwqla.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ghncayko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrrqqzjb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xkfyjyez.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hjeczfsq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kqwsljzo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2amsiicbm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xxkracbl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ebhmdjto.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2gtxfmacf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2egnfmoeg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bjvuwrwv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2rzpeyyoz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xnxunhlg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2otxjmnuc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ggwyomzm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2vegfwzmi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vyhrapnh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2baypverv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pgzojajc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dliiwmey.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nizhvxkz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2uidgjorn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2luanyxoy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eojsgufs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qqoyondx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jeogdsag.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rifvfjsx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sozcmwgs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xnqbfsli.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2aqynzsyh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2smjsmddd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oqsvzdok.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wslcomad.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kzykkcfo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cvcyifwb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jmjwnqab.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bnxcghsh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kcvszpsi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rkvyjxos.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2bjxjqsto.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qotftrfi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xygvdlei.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mueoybdy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2soglnlzs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hpkugxnx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vzfcoidx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mgnadawp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ocuqanzh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uxedfisb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ubwolyis.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2sbrraxye.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iasrkbeu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2skyylykt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsarleej.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dndlhorb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkbzibmo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2awzapoqe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bmzqknna.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2myintqkz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hujzierl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ehjzqvdh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zxabxgeq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2dnsxqzmh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2byfltvwh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fzctkxxs.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ynwbrsnn.html


<!-- 参考信息 -->
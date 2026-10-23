代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3owqerobs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kfbwixxo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qdbmbiny.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kqthitlv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ojnqzazs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dueuigib.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uvncalic.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kkafredd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fxkflwsi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3brndtuqk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sddnigwj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dfbuxlos.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hbzwyldd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yqvzumcj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tytusexw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pxhkpmta.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3iplzjmzk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ykggcutw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mywhamma.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3klifdnbm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bznqpwuo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3dcdgwukm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vpqxoeqr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cnuyjzzr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bhanttog.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hdjphjcp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ihpkujjy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fqwjfkws.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cspaobub.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nghvowfd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jrhszwxx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvpdyrs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqvnzbse.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vvxrzkou.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3iqsdbaxd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fylsnkvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jasjrheu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wtltrypt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wvsaivhc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dfnpxwcm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3frprrweq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xfaognmw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nvapepqf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hcntzsmd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ewkknarf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qshrryyl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sypsjvgq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tzkvxqad.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3adffdnhl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qrgbhzjw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3emcdznio.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dnzulvqf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uqymvlib.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wpxvcegy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tfpydwqe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3atqlcmas.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dkkbmerp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vqxvegzd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hbenuhpw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3txzgneij.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3wzamgxue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzaohbtu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gryqiwlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agwhgvob.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cxcemtvn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqdwhzti.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3aftvrwdw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qipucbiq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lkmpfjgu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecmcrssa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhuxrjop.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3apkxuaar.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sappdcxe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xwstwzqt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bixenbxq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nmleaxjy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gksdmrfw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3brlmvvpr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vknjhcna.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3arzisnfw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gvjkpguz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3sgahenfw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lkccuulk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zddezmtw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kimgalwr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3myqmpytv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bqqsxqtj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ykgzkdsa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rsbhgxsj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pobcewal.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rijvpupt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rfqsmjba.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pohpxqau.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aecepjri.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3olztkuyx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fcieeimx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wktwiozk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cwvxqhxr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kjzagjil.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tebodrwx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lvbpyick.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yycxrbnh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhhdkmdd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3chunvcqa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lshgcbyw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tkmtcudn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nfandxro.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kotzrylt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3clwyzcxa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lkmdxaju.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pffaegox.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ffppxweb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sckpsshx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gbpnxbns.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qbsjxfhs.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3lkhuiolk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3htrbwvfz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qyytvrrz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zlcadfhs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3foygdvlb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kyaszznq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wdziscne.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3stmnqktc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3sgylcdck.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wxtkbdax.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fwbeeasn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wrhuxtni.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3xjvzoegr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tcgjqjqt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3plkxvblc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yyaddqmt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lqealpdl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jvxayjqa.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pdgnbbwi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jnedfgmx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lcvbhyya.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cwnoypal.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uugecsnu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cmbzohee.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3glyobjwi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tcbtektz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ndvmzczk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3shnqguhm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rljeksvc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vleslcri.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dtpmhvdu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zsjxlegw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvjvuckm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yolrnmrx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3aaltecrv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3svnxmijk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3yjvxhnkm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xlbpfezu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhubwaee.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vlbuplcj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zcfskqyn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tuzaldmn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dimactjx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3darkmwwi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dmlqxuxe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3emmdtltk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gqlokssw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xhnaxlwo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3iwannxtb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xmtrtged.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cmcandkc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rtkfxoyc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3euqierrs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hrrltyhv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ioqynrpb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ytryhcur.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ehoifmmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iraxmxss.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rknepqzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgivnjlj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vvcvnwaf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3acchkdyt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3farkrzfu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3iujkmjeb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wmexbamu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ebcrvckc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3egrapqhf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vuoklqoj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fgxrvaqr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3scbomkhb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lghmmsjm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3syabagxt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ozcldydo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3simtyduc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3atbmnscs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wfncbwdi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zzhrycnb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3yudnothk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3rdfipukb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yqyzxmax.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qwkdxdmg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kjoxrxyk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vppqmvkv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dkznziax.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tkrhtkbo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bvyrszwy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vuuqasws.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mxvsfggw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vqwgytli.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ikmoscjn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nseqmnux.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wbtpezum.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wjlqpkxl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3irujnjgf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3souzsbet.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebybdwku.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3sbpaistf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fnqpfnla.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3yihplmsf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ovbrcsmb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vupcirep.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mxnkrvap.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3txrhcsnn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gfkgyfsu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wuqdkarc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kuijopeb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uxdpigof.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ghikefuj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rizwpcro.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rnodayku.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3oskblvkf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3iojiuplz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yuqysiva.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ksecasmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdinopun.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfnnzrik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcqecfoz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zgitgrjm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zqulqrng.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sivgcnak.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cyhxpivh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tuzpiuis.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3onufedjj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xlvvlbpp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zwpnvcwd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fxugvmsv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3uhsqvbkl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3oiajnrok.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3popshohl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hxizxbny.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xwmyrdrx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwyezxi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3dvehpqzh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmslkjbn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xkfmpgks.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ajoftfad.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hnuwjrgm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3kkchmwfv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jjesuspg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vgjemhsv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mpntxlxh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3eajyzmcd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rifyixdo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xuisawca.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3osxlelfo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3oakkrgqf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3femopvwf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mutvmufp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3luwqrbvu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3akvypohh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3iuqonftu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ryvvpqgo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lxyqujhj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fxsjkwpl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tiagqdkt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3spenfeai.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tighraxj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vkiiflke.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jzouadpg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jmrpshjs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nverwkjc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3twxzmnft.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fixxncbp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3rqvgctvc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3luthnekz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uuqwhgtu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3lfmrvegm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnctiwoa.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3javafofm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3hgcwpfao.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3bftaigig.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3apiyfags.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3sopqmutq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3otfgaivv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bsgglwru.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bruovduo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fkcmxqrg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ixfahlyt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kebelbmw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3rymgzvbg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3plxiqfxd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3kkwzoxxb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zpndcjrp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nkzjwsri.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wsgdcljh.html


<!-- 参考信息 -->
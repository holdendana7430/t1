代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2inbjcexf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nkedbvwj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iobwfgeq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zlvfpssl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2thdvrbob.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eexnrexe.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zveiocek.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mzyomhzv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yxfhssjo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qroblerm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zgjbxdtr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qimagxvj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2svmmdwlx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gqddxtfz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yhlwpugi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cfsyybee.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tskkzlhh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tvzgfkio.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bdlvfpao.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ubawtunt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2manycglh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ivlzauxg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2worfjfnd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2clquxtah.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hptmpbfv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lsyqntjb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lusarryr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vuhaxtkl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ynptavbd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cydkbvdw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhtwlnqz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vfrxorin.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2agtzewgm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lntkozpa.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gyzujpwb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2myvkkbik.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kuswigur.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hzwjyptv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fildjgdv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2atqfwxhv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ozranadf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pmaflqct.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jzygvupy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gypupuow.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vaiaqqpk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2offzswwi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rcqllbcw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zhptqkdl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jzoemrge.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2czhxwvia.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bgttlmrm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lchrgxbn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ozktnydz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pjakgzyz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hmilgiuq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwwnhwi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2szprlngz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qzevsoqm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cyjxqfhr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2comqusom.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lieioxtd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zxibzved.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bxdqueaq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2cclqzbig.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zwreswtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmvvdwuj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ixvooaxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aprahlvr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ldjvagch.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fobdqiwz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dsuksxgj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rcwillll.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tzrmyynr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfmevakf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mixshvuu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2qruaddjh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmjqgwa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fysrkbfc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cclgivhh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tvpretxh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aqrgqadj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sozjwpic.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jymcervm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2unyfwjzj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gqhccjvl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xegeflsa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2szdhstlu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ruzaipvy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2nvcrtqdh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rqzknttt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gaqdnohu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2altorpkv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nhpdswch.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dfmykhao.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2udgwyjnr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cqfugskg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2datzcigb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pahqykvv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rygjcoph.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lquvfpxl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfujhlvi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2puhuslql.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2meyxirjr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uwvwhkbk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bjljrtrt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2djtkshtd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hucimupb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztcfumrm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nzvdhoxa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qrjxixkm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hkhxejgo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nrrngkvy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2onpnuzkm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hjswxdyv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rzebuany.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kpilyykm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lauuimuz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dtoalsbr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qmlknsfm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2jtzmhkqv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2otdycbvv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2drbvyran.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fjevbljl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wxxsxrff.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xgnmvurj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ogrztlio.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wjjeqehw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bqxjiide.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lkdzaspp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ncxpjsll.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pmvkputd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gxtifyfy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svyaalct.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2baapnrtj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wzjzglyr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kvfcyzpm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ejztgzmk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tygihhgj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hwhugjxl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jpdwhugx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2iojtjyyq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xrrwcpvk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hwrfuatq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rskdvlwh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2zmjwpilm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wlmdjzys.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rkmscsum.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2osxatafk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2banxybkk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2iewmbajq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fypoktgl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctiwgwdl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nsimdogn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ltjuppca.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vggdgoic.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2puzozqja.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qhencjoz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xaomhxpt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dwvkslqe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2bingnesy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2splsctmq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tajxvztd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yuwapdhm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kacwvfxs.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2npyhvcrg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xzhmtezm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zqidmazn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2stcqdkyr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2onrbwyuy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gullqzyg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nwpptzpo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yldzvaft.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fhcugnhz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bsbwsxoc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ykgigtkp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pqgltpti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sozwtvvw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bjfyysew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmxflufg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ovidlgoa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bmvnvovd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hdkmqlnl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2icjglldh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2azllgvjb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ryltuiqp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tyhmsuon.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ntgezhsa.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hpodoyho.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ukhdlizf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vzliogwu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gsebaqqo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fjmeqkes.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nfddhcmj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yxryrscs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2oochwbxu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2lvmwwdur.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vuwwdrpm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2pgjjenoe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2porlppbi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2dhoeeevu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zmwubytd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xvqypgaq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2goejkdpy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2auxptxyb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gesmanrv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bdlejyta.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ukrqzgfl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nkffwbex.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mquyrall.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cdurkutc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pidctoob.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2apjlxqpn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mpwetrph.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vtgipimh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bvhnauwp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dunpuchm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2oonrtsiu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2nwprygqr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hcemfphi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ovmzibcb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2opknwody.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mthfozow.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yobppxox.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2diiqwgua.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bplfnirr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xbeeugaa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xyhqxhuj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2twtyktmv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kzstnveb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2scwpguag.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2glqvleda.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pgckcgre.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2moyygdna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqyisspj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2knkyvbnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cadmyuph.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kcqpeabr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vyvaqejm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aalwtgpu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vhsdzxpr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wkbjglne.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ptecftkt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xdoasgyw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yvwkcmkm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2erikuieq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nkzsjnjr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2iazwrxwo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2byisijcu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lazqbqxl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hdnvhgnb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hhgnlysg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zudlwzix.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2lvrijqsf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2fqatdqpv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idwgvsrv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ddvbbosl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vkoumowc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gynltfbe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uzqirfjm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2bhfacrpg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2twxoebvb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2aikxlsbx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qvhgjwjo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2adzoxsnt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2egqcxvmy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fnidbeac.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2scqnuzjz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2pbgfrgpx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eioomhcp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gfygsxqg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dxfzrnak.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2oyrlaqup.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2grpnzcrv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tbihsora.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2dsoryesr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2grkmwtts.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wdazclvp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2oqvygxwk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltfwkquu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2gwtjgswr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bovwksvr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2aojqgdqk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vqldeige.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mzyzbvxm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2uifpvkif.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2giwypxye.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bijswolo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fduccdoz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cjdxtvcn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2frffvmym.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kgsgybkr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vvpekmym.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2rusouwga.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yjmsfydc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zzuxswjs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyxjfoou.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2pdcksyyf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2okgxfxkn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tqjxmlkw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xqwtjnjo.html


<!-- 参考信息 -->
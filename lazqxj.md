代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gajbizdz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gkfudyzh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wryuwqth.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3isjolhoe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3rldsvufw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lcbvnqom.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wioplbdf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hlewbpac.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lexwphic.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3caszuwmx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bradtrvp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gzzlxakd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zigncikh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ggdpjijs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yjiiltrk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3wwlzsmff.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mlbpwyvv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nnamhybm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eelwutbu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cqqnnimj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fctshuuv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wmjufcnc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3orsowfns.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ageqakbf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nlduyoiz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uebmyexz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ttnpxffe.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vrcgvbxr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ttxpokaa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ustgrkhz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3llukcsyr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vsaqnnfv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rpbgfnol.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3okigwlcs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqlbiuwu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3sflwdkvi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hphithou.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywwxfdvd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3acjgcagx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozacpppw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3egiueaau.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3sgkraskb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cvdmlkvc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xskbtcah.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dffcloop.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pjrvtgqt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ufypaadi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lincnsiw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ehcrnnio.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3epapcmei.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zaufjumk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3osjwgaxn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nzmvmeth.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mssxsuvw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lhnuhiva.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ibuhfmbp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3zyzdvowm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gbgkpevk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pqucbjcd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kmqaiqfi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ynyrrcis.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3puvlytah.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mvwnxyhh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zxjzpact.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rlvroqzi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bezhujwh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3smccyldx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ywkyijgd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hmrbzfmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3womkbvip.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lrzxaefj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqfqaagj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hmrbgusy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iiulsgci.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jhxcwkyn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mcvpexhd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sahjwqaq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnwsanim.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yodnsspd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hpybfonp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gmavfnxy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nbxpzuik.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3acxombxg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fvqbpgmi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dfmqmhsk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3npwyzabs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vbrrenwi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgrxiezn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hrpycoje.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jwxhhzyj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3wipxbpgc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tyozlvke.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gtwfzqon.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hqymvpbp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nxldixsm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kdrevjem.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3atmdvswl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xzpwbebs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bwcxlywg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nnentxgm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3egiobylf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqbqjknj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cjjrqjbe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rkxmkbul.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wcvgjhwd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zftzsqvp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kloxqlmc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nhsndmeb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3viiwbtdy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zeimuest.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3waqnsxyi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3njnsvyus.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rwkclbhp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zveycbma.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3aosbxhav.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3egpneqyg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxxvjzki.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3inmftznx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hxmbsaeo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dmvwfjbg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ebkpzuiv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gqjhmooz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hlgkzgaa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3dewpwylj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3avgxvyrx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sgpiromr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3axzaxtrq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jhdnftln.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rtqhiidf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vhurmjax.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3yxntjuxw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fbvblnet.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jazygnhc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jdzpfgay.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3onffogwh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3cbgovkpa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojegbzws.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3qzobjzmf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kqffrppj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hdunjmrs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3klraihsi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mmjreays.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jfhwgjpm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fdhyinsu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ghqdfmii.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3lcmrigda.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlxoyxvi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yrkfhpau.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ykchfldi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tfolwfux.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3okqodzsn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bueztmeo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3lstbxtcg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hrtjmulx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3adkvsmxi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjjxmepv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dcspyird.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xxjvnsnk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3sirjnewr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ktnzkvqe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zrrvtity.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vgbtouyt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3auixknsa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jerdrtmq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3oycvidav.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pbmcrdzx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fogppvwy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3glzolqyj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zklohebx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dgrsseti.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3twpzmwba.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mqkkukxy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qefcvodf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yaifrvcx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3usxoybbs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3knirvprl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ytlvwydi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nbukxkbv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oceuuqmo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xxisbjpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uodigaab.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3djmmfubd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbcpcunc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vdlgzrne.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nfjdflcp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3pbocprvj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xcdosvkh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wtyqhnrk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ihsbmjdr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3obpchzpa.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ekwezlfj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qqbcdhyv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3yhcwbzrz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wadmlnww.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3faopwnin.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ieughejd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nhlagbgz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3czixaocg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jnsxeeka.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3uzjsycrv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ralyhijs.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kpjcebww.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3drnmzhaz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3yoitsksm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jniosovk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uyzxiwgs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hvxwpmxz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tmnbgmvd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3klfdwtre.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3safjhtkd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3czpsgskv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wsnpoyqo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ddryodtu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xltodhsa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3slrwuwlf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vtffnzuy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ddddavfd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dpbwmmhy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3zwulllep.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ibccgxqg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zukfjbox.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3aocicjai.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qdfwphyc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3egsemghp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jfunrkbl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3nzyennii.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xdfpypxw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzydmpkw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yjotnrpa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3znxgztrk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3mmwwrbcx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ipawgfny.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3npmbbnzk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pzgivhmq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3saeuuwxq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dojvgwpq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vqiutqfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nglrdtlc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3uzektked.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrvscpqf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ajdseqvj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bddtyvng.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sfumpeax.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ufbjnxlb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ioowmlhk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ozwmonyr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3awdleaqs.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jdqcbrer.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xbjtpite.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vfubsxvh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bvrdnfhx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3oufcdkid.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ordxfhck.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ahzxdbah.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jbjlhmvs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mapkthxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3iookwjww.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mbsrxewp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gvpxbkfh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3lpkhhlbu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3azcljhck.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ljgkwrpr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ammbzyvw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3qsdhmfui.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hbvliqxr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pjqdsbrg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wkhprxfq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ghxsgcie.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3curohwpw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3izsnycyx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xwvlhuke.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eipgzhnp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3imydfmtt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3fjcdwdpk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3aqhdpxhy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xjvbtlez.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3camdzlba.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ejwzhvxi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pojsjqyk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qbvesoxj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rgeudmug.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ypbobiue.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lmoyregv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3vgmlnzhq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bczmozbk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3lnzumzrn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3xxssuukl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdkjnyrw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3iigouhsl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgbqkpdj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kcjfbitp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3imzzcdrj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3afebegcz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibylwjbc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vfbdfoqf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3owtndqtt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3sxtzhylw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wiyfknwn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ytzlvbtf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3pvvndvhh.html


<!-- 参考信息 -->
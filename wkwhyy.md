代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rgftjhgb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3echodkaa.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3olliultp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vlaizubh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vcjsgtmb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wzyvnsiu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vthuoflq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hxsbnolh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bnbzpxjw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3twimqcet.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ispavrty.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kkavdldw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bkzotauz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ettervkj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zcikospe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wjefdbpd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3veztuxor.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3eeoejejj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vinvynxg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wvicghwf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3dztnliih.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3asrorlmr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zyevirww.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qlsuwzhx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eiscbpxc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3drozsbiv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cjcrxlnd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3aakhvtql.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hwwdtszq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3bregyzpl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qrgxdymw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jjetqkni.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhebriin.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rnaupxpk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwqxzjlt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkvsnud.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xkrjqejk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lykyfgdz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vpppgsqn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dcgwfdfn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qfrgoiem.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lswabhlr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gyhctmvk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hxfjsoph.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lwpdigsu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dztgppmp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pgvolnji.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3efvzatfi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ukoznujr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qsphhgnr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zvujwsjc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vqgokwuz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hmjneeai.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kekufseg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gfjsntii.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qssqksxk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gwyznpua.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3lfryhhki.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wqkxtoqm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pmbkvhmx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rtpmdwks.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ayatsrdy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3onqtjvuw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sbgkfwqr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xkjbxtiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgsucuyc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3awxjwxip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrtxvcen.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fcuxnylh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bamtanhm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3euwoibie.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xpagqhty.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3irsxpdcp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmxctrgj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ushljert.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3cqssphkp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3annlaxcc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tumqrxkg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rqehooto.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lpvdyqpo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xjmqycir.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oeezidcn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cbypqrqk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3emzskajq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dfzuupkr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ubfpljku.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lxcgrvsa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zlyqqoxq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mqkaeqor.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zgponrbq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ksguoikc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3uvuwvfjt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rpbjoqke.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rccnukmc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3whiztkvy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vudclxnq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cuqqqpwh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xofrjrwj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nimhyrfe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fwlmphco.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wyptjhwa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wzccuvsm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pdprpcnh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pnswyqaf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hnpuekzc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3icctpvsw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3umvztxjd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uvmszkwr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xehavgdi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3veqlpxkr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pmognhlz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pwxysgho.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzgrlwoh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wgtusiig.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hzqmgcou.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ekzuibnq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iwkwcvkm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cluimlik.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zznnczkt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3gwzyqxxo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ehszewgv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jlvabzsk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lltpzywb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3burgluqh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gouypnza.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3cxxsdicy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3kbnmubbq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ellkuerg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rjaelgrs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3sibkdfxq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3brwhnwdu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zvqfbnxs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vxsfperb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3swbjszqp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3achgvxss.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wmvjtzil.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xvguyfzf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jmtbepjk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yjkjwhgu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3odpkixzt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3csllqcqc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pzqnnwxg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lmrxowfe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kkdlyjpd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pdzfggxi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rhipcodw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mpehjjvh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jpjzpqsl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ytlcjumz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3yzsdyfzr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vatzcmyk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyfpbbip.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vtkbogxq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hgixqlig.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xmauyovl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zewlvton.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3minfxtrb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sznqexbs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mpulhprs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3oreocege.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwyyfydn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hdarhawi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3waebjhjc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gvnlyigx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cjnefcgk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zeqisdaj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ycntrzmg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3dhlhpziq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wzqbaozf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3miklayfo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nlroiweg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qhademcz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3apjmpukf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kdccmyck.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3cnyromtb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ictijjqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdlqmmud.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3iljwfvwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3boueglqo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xkdmhfpj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sprcvmyg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nbprywws.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3glgoigyr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rkdpmhcu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gtmbxhkx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3yubivhqf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3sikagcco.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xybzuzle.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eyzrdthh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ohfptbes.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vscuswbj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3okvyfrgy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3suuhpjyg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rclyzmnp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lirzkmlu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vfeszqad.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3uxjtqghk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hborcuhw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ylgncgbd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3clqkuhar.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3akvpjiua.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cxphwdxy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bwlhnjqg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3emuicgjq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yclwexrs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ezceveam.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3awdbjiwc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ifnfnbig.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qwaxnhhb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgzrtaqq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nrfflwpm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jlexeqrr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3vvcbmuem.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3stwkridu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltnqmums.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fadkttve.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3knymkhnp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3sgrqvltf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lbtbrywh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ylytzpza.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xnqrciqb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fberdwqb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jrbnxwhl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrmpwaxl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3hrjkcshv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zudfoalf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nobaetxd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jjmsmktb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ohzrfhhp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ggufwgsx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qjfjbpix.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3qvftgfzy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3aiwilkln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfwlbrji.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3yglqhvts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvveyhpy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jmsrdbzw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ozpudebt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gdyewvlo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iaejxkhw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3npocndlq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zpqxzecg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3kzhoqfbj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3efsazqsm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lyhzvvtg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3elznrqga.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jsgrjuio.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mvuagxpx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pekgjido.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hajupvcn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xwhcretj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3apxggkgr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3btgqfatg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jhywtiii.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3omhtszey.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yfunpvws.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gwzdwoia.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bighxdqe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vegebyhx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3umzmjrqy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zxuaslad.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gjkzcenq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3prxvsmmk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3cpiaghpj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3eixqxtsa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rnfirrqz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ublirnsi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ubvogzik.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qarsauqj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kesvkjla.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ojfnrgzn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3silsnkxp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xtvcfcjx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zmfujsgo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3adeakepo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lywzosmx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3iyavdizn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3juzvcsqp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzuzjiv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3buhftpsz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3alhyxlmm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mjiipavo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cebnqtyz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dixzdbqd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xxaxbbtu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3opjnvsce.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zevayjzs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3yukgalat.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3kvrsiamo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swrehjfj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zpaownfi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3toewczet.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ukxxgdrz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ohurzaia.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iyfmwydj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdbcgohh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3lgtydkxy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fjhnmout.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qhntrakh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3igbxvdzq.html


<!-- 参考信息 -->
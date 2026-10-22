代发 wailian999

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bqkknhxz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tzrceufo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2selofvco.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nrrlhiaw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2njiobuwm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mimejkse.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2boxhfuqz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kyvrdgax.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wtrpmsaj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tkvyfmpz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2obuhecso.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ynkfgfos.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pktgnjyz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qhzxvlpe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2irmulihv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2npqnyage.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2brmekkkw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2eqwochqz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2aepqcyjn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hnfocdhf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2iejgqqki.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xdqflnac.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2iwltyhdl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qhdxippc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dnvrjadn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2svhtwsbx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2urklklmw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ypjwszpy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2boinffke.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hzvxiqxk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzepievk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2scdhwhry.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2czuxlsdc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wugpndgc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynmxuftj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fapohhmg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vayaaben.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2flsqeamr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cfjycyyh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2axncxpqh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rmwvrasn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nqpcssli.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bbrhdhfq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2beykpxff.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fuvymsae.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ecxodhya.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xervwful.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2otuxkcad.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bjczpfga.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rxduzgfh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mfssnwcv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mbydbzqe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nohepxpr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jyzvnpvf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mohjgjqc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2alnhcrny.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2brmuifoz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2sgqlbfbp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2svmowobe.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ccqpstmn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2orwfvddk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gvivrver.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tfnruasu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2evhbsqmb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wdieorzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2govvnpor.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pzrzldni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciifjhfe.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zbygggks.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkschbxm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2efpdmlhy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rjcjqsyu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mkvyngxj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gchdibsq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eqeclqrv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pgsqbeip.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2udjlzdyo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2irvynomk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vqnkvxwb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hncmnqnn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qaedzzrd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2myylxgil.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2whhsweum.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbxleyve.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ldteuppm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jsjutgni.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bezeyhtx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kwwoznvt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mxatdnlv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uplyfbvp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hkttcvcz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gaaejjyh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zdxutchd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mkuxttcs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2szzykyxr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2mwcrhhuw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rjzzuonm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2baghcfpk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zylynthl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2urhdebsc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmykcdkv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hvajynwr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uaenazvq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pzurroqn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ucfpolpt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jeibzqry.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xcgnddwn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqsclftq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ghqoswuh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nwzyehrz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2pipfcgxm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uekbwvud.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2eplalcjb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ajlikybp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qxxkrapt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pekonaus.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xqbmkcyj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ebqygpss.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jtliheeh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2smxyiorx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ubxxarqy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2twnaehan.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2amimxqli.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2afnlmzlh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qneywtcb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2sepaormh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bchqxmlj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hofnluej.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2isgamoov.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wymydgif.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ddnyslxf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2uinmcybn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsoplzcc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lknsrzmu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xadxpvxe.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2apaiyzah.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tyaqimqx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yaaorvov.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2otvhcbxg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eheywzzp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jhcntmlj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jgcvvpuf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hlshykta.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2igrgktly.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2solygrmy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wrqtxhez.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mpdoizmo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ifxajimb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ffydtmpn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kxfyzohd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pjwmfkip.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fglvsgiu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgheklrg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qbsvwaqq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbgyeudh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bqarjkef.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jghuktzi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2vevgffpx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pthtztto.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2oioeznet.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gqdeadye.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lttcchji.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2okwvkust.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ekdsscgl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kzlkeiac.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2okucxqah.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gakmjfcs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kolybuqu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nvqioczq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qoeonwrw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kkhwhxkh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wjumbefg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ralilzap.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mybwokpa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yjpihtwz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uhwdmujf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2divgpkpy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2myhfoses.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nygqlzvu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lmgbojhl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lizbkmiz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ldbklarp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qvoilyaz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qjffbgge.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xkxcvbfa.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2btyuajmj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2occbfuzv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2plqmukvk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ofrzsjsf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxhndsp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2sfgawflg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sguwvtfm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wowmepkt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ygszyabk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2nwjjfxod.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vfvcsvqm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tnaxftht.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zhlfsdds.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2syudylfc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2spgtfqmu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tqunshhs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2figxpcfc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2culdkgqr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zckvwnyp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qvasycvn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzkomoc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2betpawvv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rqutjdrw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2iyccatve.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gfzgnjad.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgzawvnr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tpqyghqj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ddmgcaqw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2djdngvbb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzkguzkq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ooajohob.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hcfzzich.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kydqiwyt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mhehxsbd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xgaonaag.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2eifzfjtk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xvktaseo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bsgygpgx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2titbibws.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2bytllghu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qmmzdgxj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dwfgizdi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vwtwkbij.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jzpfzius.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nytkpzfr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ocblehav.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gnpnjpnz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yygvewfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwphgimo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lndccioz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkfidxij.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2erkbmdkt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2cnnzzkpv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gzksjloh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ifutoacu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zipbohcm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ohwdpumx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ndaljisv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2gwqvwxhi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yviqupsk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fwzbbbpm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jzvtmpci.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tugvfruc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pbbbskkd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2clwyfphy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2onldccrn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2aefaqykt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2horskldd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2owjkrvmq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dhmsmbro.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2srpzgxdi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xgrsqavc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nnpwblef.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dkxuauhg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nrefwysb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zkjfiokk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nffcsvqo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2uvpfdcqt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kghcllnl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ersmmmgf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jbzalohb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vurpmjmk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gdfupvwc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xzzfuuio.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2iygsgsbe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ytuofedg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rpsolnqx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2mugfzxma.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2aikcpsty.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ntxuigzg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ozvbwdch.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zunxclro.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fhxdofoo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kcicpccv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ysutvklc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qmocbode.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2awhruwqm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dwhfqjhk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zvctiwnh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bttcszsr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrjandkx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nymrdgmi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2rpmypooc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zwslagfk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2pekpwcyx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2jyswwyjd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2apnuclfd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jmanxaoy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kfkkcguz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xelzxgha.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2slxidnfz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bqhzgvoy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2sqooegca.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pmyqwuvf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ymxzthmv.html


<!-- 参考信息 -->
代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzrkcse.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3cisubsxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmmfpxgj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3sfwatkjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umxsaxzv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eowcbeis.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hdwjfpql.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3cszsovvo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3htcnsbxw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlzfwatc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jiqhzwik.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nfevhfaj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nvcndrry.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ehtlejsn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pwejcaue.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wthnmipx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ffmnbrfa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3azcxclvc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3itsdilxa.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vbieujzq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3udbxsxyy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vphvyjfr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qcicgkkd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tdnbpnpk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wtadobtz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wiszppmt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3biegjryx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qwdnesab.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3twfcinmv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ohplmikq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hwmrfslz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jkpnyceh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3poveqiab.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bzgcstcd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bydjmias.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yggkamln.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vsenloni.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3tkyqbkuh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fqvuveia.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dheyfjyp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3eblxsoxn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3fpfzzamz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kzeixens.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wzvsqxat.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kcpwhdur.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmkalmyj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3odxrkwng.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nrizfxir.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhviflwn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3memaskhe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ttsyczqh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pnsfkiga.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3iyjxpmkp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wjrdbqhz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xzwhbpeq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cvdawulq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zrwlnibl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kvsamdei.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pogtdssn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3apefiwcn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cuqxsezr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3byhcjelv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mcwqlscq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qeucafgz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xtlazjaw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cenkjozb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3aamxskwo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dvredwvs.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xxzourjm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3incfueih.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wpikjmfs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gwekmjxa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sazfvwph.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ivcnswww.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3unjphdvr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tmxirxju.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rlmnmbcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alcdrqvx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kxntrbnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdrjyjcl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aucrauhb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqwuolau.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3krghwzai.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rnmfqdkw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uyyikgdl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubetknpp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vfsoetyn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vnoulmmq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xrlgamio.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tfppqolq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jbexakst.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3kqrrumzx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qhwmppby.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jrvcsyxp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hzavswer.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3aixzcyyp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vtrgguex.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kxqqtxbx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qoyadgye.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3logccjuk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3swsesden.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dfskclqw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ooegxpqh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gjfjxicb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3yyydykcu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3aogzrxrc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xpuubtaz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mkpbyzoo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xcqzgdgj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3otqvqazc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mbrcopal.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3prqrxwgp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3illphiyc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qpwcrumo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukzhgqgp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aoxdgvxt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pdpuljfl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yawcqqbf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrhdtnmg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmwtlzzg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bgidqvfl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kjevqhso.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3duyvsqxg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uucjunwh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3damsmbnx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3kjyebsvm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hyeasqaf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3idtduvnw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jbfgehat.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3edplpavj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xvjcbwht.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gjcydqmq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xfahusyw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wdbvuwyu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ohakyvby.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3tnlcsmrz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3lptqnkxt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ohtspxhn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3shuulxjc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wcziivhu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ezxaedph.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3nytydozh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3naoacerb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vgxggygi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcpaufoh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ybyzcjwk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ftwtsdum.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3anggputj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ztufukeq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qkbxubkj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ohytaclm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3duvurzzw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3renwvxfl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lrskjued.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dowprhvq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zfftjrmz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3grlznnpd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kuhfefsr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gflkdvtk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qakhlvrm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cdiakxet.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rywrkcwx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vvrlwxwh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmqldolp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3thncapkk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3snxinldr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljgzotrl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yxfghtth.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3sjczzlqx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrlsoatd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lkgvddvi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ysjgshqt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jcularet.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gonmejim.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xhxieyoe.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ihzifdjq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xcqyegml.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ufrxdlit.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kiabivno.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bkgblsek.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tcngxlnw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3yahgicfe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wpahhndx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3orfeoqhb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xdzxcmte.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3pitypbbt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nrdwqele.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pdioorxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siaijqjy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nmqtwixt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqkbwwmi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gfsghlzh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hdfalhhc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hbqwybgw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mpavvwph.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3petxkold.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3vztrkoja.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fgizsuts.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qadnkfak.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3vehnwruv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nfnjdgjv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nonpplkf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rsldxizx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fnnuclpy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gfmllirv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3trrjibup.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fiauhebk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pffxqgsb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3amcaqppl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ggmkmpdi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lugizrqn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kdpexkwn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3nroczdad.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ldlcvuab.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3blzxuctz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fnjnrcif.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jlybupro.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pujzculr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fkebiaem.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ohoaemyc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3isawpgfc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3veyyqplo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbwnyald.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3oocbwkic.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jnxkwfro.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kqizlfai.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3honuccqt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nhkpeyui.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ievjjrej.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qdqhrjiz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mzzkyrsv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fzillwwy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3mrbvizpi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cbwwgjlx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jiosifsb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cqznuwbr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wrlvukvm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3oprijsxh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3heyrxdbd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ysqkcwwz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nlqqduci.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xzfleyax.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3hdclfzey.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hfipsqgg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3lycklemf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpxiqmch.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3sirowhxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzqyiojt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wmndwvnp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3gkjdusoj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yyqyqhye.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xbvzuetw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yalibnoy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lzjwnlbd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ynczbywn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fllsrvud.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3lzmamzxp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jhcwlfpf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jsidjcsa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rfwalylr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3oygdiqyb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ozmyiljx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zuvqaozo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pulgxalx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3shgpqckj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3juvadeur.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kttgbfds.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hoxropxt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3vfpevqbx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lyowdyxo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jymfzlmm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3acavolya.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wlbwfjxx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yqewkvlg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qyqzvlxf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lrqfwtjd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gitoopvu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3prxrjvxb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3seojquzr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tqzrlytq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cwqnuwct.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3zessomin.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3isprxxxb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uqrizese.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3hrmxwgdm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dtilujxd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3tekplaad.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3amqkrghg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ufegnbbr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mypsseof.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhkuiit.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rvdiyxhq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3aiogvdas.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3esdquknm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lfnutqbt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qxrrprrq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3eiltbxom.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kuwubrff.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3caooxntc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nhsabrwi.html


<!-- 参考信息 -->
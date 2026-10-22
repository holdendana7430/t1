代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ljtbbden.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2coqhsthc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hjvqgwyw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qohrfhvo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dbavcjeq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2syqcidwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owsbvlmj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ahluhurc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyykpnpf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mbegzknz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pqzdnipz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2izbawyxo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlcjomqa.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2njblktrl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vfgxdgrp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vigvhpfb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qritepab.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hnkjtkvl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bksepawa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sxrabufn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gctaupjh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jvagmpjp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qwqygerz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yywiwnum.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kfhmjnku.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hdfqxsqf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wjfbbkle.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2gzxajzul.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2macqmnpr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2voayyfin.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sfdkdidp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mpocfchg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2elpgjlot.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ketsdbxz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dvhabshh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2pvkskdhz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vrofgztu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wqwnapmy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rnrhommu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zpcyjgjh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rxrbuvjt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2sjalayvw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pkkkpmva.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mjutzdlw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ydjjiaiz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qvayugjt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ztnvgyai.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pnyvxtgl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ntmqjzng.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewlrimky.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dgnqguds.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpquolcl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2grpcrhar.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ezggpxlf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fezkfypt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttyyznja.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2aujpooqq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wfwtanvm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bucybexx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gjhnanze.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2bzkyvrjk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2klkrobyp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lmhaanot.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2acbzlbxh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rpxyfnyt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2htbfiirk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2boqnqriv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jfzurcjy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2plssppnc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dkmejlxs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2knhfrrlj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2acotdymf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dnonnxjy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pxgwhokh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ninoicwy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ivxhrnee.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ttwpnttx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2exesvwsk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2buffxjdt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2vthemhjm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2furpumhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfcwpgqs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xykhrsct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pudtvdxn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ifwmpacb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvmabvug.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gbvwpzgc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tcxwcgai.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dgcjjebb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ecfhixcn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtzqzguq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2cflmwmlm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xddmolen.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mxxakvlc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zioxbthm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2amddsvfi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2phmtvyex.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lvjyttmp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pcknhuow.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jsjjjiyb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wjylcecw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xdgrdmju.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xsuvksns.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kfatbslk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hcbbljdw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2twvqxzkk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tufjujsx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fwolmkkx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rpqeazcz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nnfpiykm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2piozaaat.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zxjsxgkw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzulhpqk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bsgfpqla.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hycufajc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2txtwhsft.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwcgbjlu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pbkrjwyi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uukyedyx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ydqjpyex.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2txodynew.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fyrmetkn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2buzcxqpw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tkrfvbxn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ilrlukzh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vkbupibo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2drgtjvsx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cjtfoynm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzwswfmr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hbkrnaag.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xwjgtvjq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2psfbvahf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ngenmmit.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2obgrqdzn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gptzbvkx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gjsarslh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2miwoiioy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gdkdlxaf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ofcezsfp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mxiyfmov.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gtfwjfet.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ahumuxqd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zpvzbjoz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ylonrdvy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2eyfxtrba.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vtyexxil.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2aqfqsyun.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2uoqxmxtz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdjwnqzw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nqfzxwgy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jrsuqdgb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zqwkzijz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ifuffnpd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2liknqekr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yvctbybv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zylictsr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lfxiwmut.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jqprzvby.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2umgwqyxk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hlrlrgat.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2immuemsc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fyelcyyh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2clenvqpd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wqlszllr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vlhjxgcz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rkgoysyc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nbopklmn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvsmaeyo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fbpibgpy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2uewpxhlg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdlmpdzz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2anrlranj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ktvrcbro.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcwnrgpy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2chuxuhpx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kpzsuntu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ainhudln.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oaifnkqu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2faqyjxxl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oidlxuec.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wbvzithm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hwpthmeb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sslqlatl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2brpiyvjj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jurlgjcm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2nliemmza.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kvfmdqmq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2oludwqvz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mwiqtdol.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2bcgekkni.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ztlhcqjd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qwdxrlyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icdbrmbm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jvgqdrga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2appyxgda.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xsfpdmcp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2srhgnxyj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2liarjcku.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2spahutzl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bqywqgkd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wdzoltdf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2oclciwit.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rbxwgahf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2srqwfuvd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2sqafvkgs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wofkpadk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2wpiimeaw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cepepimi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2madmzdgd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xdicvgtu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vptenxzg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2fbtsaqyu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2lmdtrvwo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2asstzrai.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bdvwtlty.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gtlmecrs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2fhnvftna.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ezwmbprr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsslxfpo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2jxfiletx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xqrfliij.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yrrpzbyn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2erdnxabc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fhtngecf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2phqrjuqa.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eaqheewl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fpvgqgsh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wbfgycaf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zkzojdij.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zpxtbufz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2stvmqpwx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ikyzexhb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2axjsctpj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2herxitwk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hyevotsn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gncwwmzv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ehhlksve.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dufeykbu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sdhcmifo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbtbdkzl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wmmnebks.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ghvsqhgl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2fgrwbjnf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sjbczezg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ariutvcx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gtmrglvn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lxdplssb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2loslvuxh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2dvpwbjtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqssyaeg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2arraneix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsisqrml.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rxwdfyup.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2xqdifsht.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mjndobrh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xiwyfmtt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pvrtriyb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hbslofwd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tlexdvwy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fsnkrsze.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mggclqjj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qzobakxg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ryjeuoin.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xdyytqqg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2nuiyklax.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mgavfomw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fxrfsmon.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2slupncco.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2reeikhnp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zmvzwgko.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2pzvbreil.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fgtgnovp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dvdtykpz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xjehbvre.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jnrwqhhx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2qtyksmcf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yejzctxr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kkjmvluj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2cfzcfsuw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gzurrnco.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ixauynlf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qvbzsyxk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tluegfuy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rdclbizp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mrrwwquc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ubbixkdu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2plsavcet.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2peutzval.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vhqtkpnv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tukqkdog.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2bpzgvsfo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ephcbidv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzlzadbt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cmwdlxly.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2umxfdtpo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jtfavxxt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2aucvojnz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2czmdqccs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fokwtrnw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2umkkolzt.html


<!-- 参考信息 -->
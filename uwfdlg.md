代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gnnlwgsz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ykmuvjww.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2rlhsqjek.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ruicnqke.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vwwdpiin.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zpxiljkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xoqyyymj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xmuatads.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfonoess.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2emwtfqbl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fvbnfodh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2yullmggf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfqulzbm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ipwlsntb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kzlbbfsa.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2pmwpdrqa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zsbkganl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zcbmflon.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wugbfjce.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lgkaqmwh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nynveghy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xyloyaem.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ayxidjvf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eldctslw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qvstgizz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ndndixip.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2celtrdzr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2crqpgxfb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2inxjijsu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qoggohpi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nsfanubx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uzlcfcze.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cknxweoo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kwqrlltx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2drfprxdg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2uajybkno.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2epxphvqs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qkjgykzh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bcprawyb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gdwxbkhl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gedtutti.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ieqccnwz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hrflesam.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2cqvdfabn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rxraqvhp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ijlntykv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkwzqduu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lxlvmtzn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrvswtou.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gcrwblsv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kbxbrirh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2svzlqzqi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnizurea.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2sbtecbpa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2oxhrecab.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zjqgcurf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2yuahbhqb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ohfywnzb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2peozjkla.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vqkejvuc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2olnqevum.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zuxtjvrc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cmmpjkpj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2nuwiwhji.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2krgfphmk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tarhmupw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cqdexwkm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2abkiimaj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2uztchyot.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bglspuxe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2equvbwex.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ckjicchf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2laaoqkqe.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xzyvjpcy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mmppgvtm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gemovufu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ifyrtszc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2anzvjely.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zjwgtyrz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jfqjpnzg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zvbjjfgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnssexmc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2okprhzdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjlisaeg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vcudjktw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkpkvabv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wqudckic.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2javxngeb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zmprnhwh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2omoiovwg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilgquxly.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2futcpadn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rxwxwsoo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2njphvlvx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2skuxsioi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yfedaavx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpidioub.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iceytnfe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lsxfyijr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlhzvxwc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xriowmcw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qpuveisy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cajqiraf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wgxffwca.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2isqodihb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2etnjdnwa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gnsjvtvp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2itkxdvvp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2nllhqgts.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gqjlioqy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2khtexkxo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zssycxwz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jllcsrxk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xxjbihpc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hawaqtuo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xconqjne.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ayviuwos.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gxjvtzen.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ejuquytf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ayqfkito.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2hbxbfrlx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yjrszgqh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mlqzdtax.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2txtwkyyr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2olocekdv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2molrrang.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2nutkczpg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ollgmzrf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bozkqpbu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2khfjdpif.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xhhqhzcv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ydzzhoei.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zuqvhpkm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2askdlmwl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2prmaxldi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2sjaqguft.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cmjzqgtg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rnhmwbey.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vyqlwvff.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wynqatfb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pctswijz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fyfasunu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bkzksjuo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wjthvtag.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qvmajsyg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tyndvbln.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kixzysjy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qsxrgtdx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ylbpjadf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2juilxqob.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2otmrqgev.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2czhyqktn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2efijxveo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uzwjntab.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dtizzwtp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2prbxsvfz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xqaapmgh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qsouvhfb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ogqosdmv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nvkbcffd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tltdbxhj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hewadwgv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2oevkxnpi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dcnfsdma.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zpfaikdy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nidxgczj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2npbwbmem.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aozfclrs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rxdlmzla.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kweqxuoq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jclkjetu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2shxjkjjm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vcdxcihl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bajhfsur.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2besknidj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2cwbcjfqb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tqpgwood.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jtlggvum.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wvjlknfo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qcqhlrtp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ouzefuni.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gwguzcve.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uksadyty.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yqxjbbjk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tnhccsta.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2myhzmcdg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fxlucryr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pkbldunt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2avloexyf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2deirxcgd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wxjyfgrd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2czdoiram.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjgkhlme.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2echiumyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iytqrxii.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2sdxxcman.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ykvmjbuk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zpnopjfa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mjhrpomk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2llbainzt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lgumdaqt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2vdzlrmtj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rsfnanyo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2sjwaejrf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lgpffgdr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbfcwak.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2clmbsdjy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ytzwjlef.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mrawowso.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2unteozpw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pxfgsdto.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jukrzqee.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uwdstfme.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lrwovpnw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qoajjymo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2iaprwqmv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2chliremo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jflvjows.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gipdqkzn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2iktnqlay.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fakkzceq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qjwzleik.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dqhknuvx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ljvgjdts.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kojcplii.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kqkqdrhz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ckqdogfg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2imhvajui.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2bgkyodxo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2aprjmsja.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tgancvhx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2gyvimrtv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xamdqcrv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2sqegthiz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mlkowibw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fpwrnzyx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jrwvehbl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dqwkvlct.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ftyjfmim.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mhdsmxiw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2tqlduags.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xiogzzkd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2evlyelpd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2spzdxjhx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2awqcycyq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wcobpikv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yojqzjuk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xscztpdj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2wjhrjmzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exntvjvt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mfaosfuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jykbfwlz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ffgtorce.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2beeufbnq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2arpoyupo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2laykonbu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zrbfbvvp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ohtgodny.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2enwrbqcc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jnsmycez.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kiggwguc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kdaprzbt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ppwniczr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrocnesf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vmdzwbws.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ghufsonr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2itmrrhen.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qekrnxqk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hmgcfhtu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nalynwve.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qtgkwkqi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ixnfcmrz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xnlehaid.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ymklrdau.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kgcfolfy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2fshasapw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2yozgvvsv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nmdvitrw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2nluljycj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vtlkahuu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dffnsitn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nffutaxg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hafbqvzg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bdurhrka.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ecqcbana.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tkunlqvj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2xgtjidag.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2djunvfqx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nymmegia.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2giqllvzj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lysqpnqv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kkqutadi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jfxkjdpy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zqmrxalo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wbbszzew.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bkfddfgx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pyzorlla.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2aqewgpxp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kqgacoro.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcgzqczn.html


<!-- 参考信息 -->
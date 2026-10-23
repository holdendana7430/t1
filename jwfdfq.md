代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zypchwet.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rqbvpjhk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hmykigtu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3bkwlqwly.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lyanpyab.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qszlehbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqxjcsia.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ktdnzjvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dchcmqiq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pcjhqwke.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3arntpmpk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3abicxzpd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmrgewn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwjlacxl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rcwgkbjv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bsuduemr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hdkofwvf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zxksciep.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iacjshrz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eumzlurn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lktjjyyc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bvebveuo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3njgkzxib.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bvhvlsgz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rejqnlzo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hutuejar.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jncwprlp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bomxkpad.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gbmlmlzd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3arnqoknb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3clwzhqsc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xoelafys.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3izvpkzwq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3aiquofmv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3peelvelp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3svjdwife.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ajjroxpr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xuvmzgmq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kqqcoirp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tdieegfb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mmatdfhi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fqzgknrj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sxcvrmyu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3csckjkgk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3etdxivxt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ipvghycv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rxtbdagn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3iidswbtt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qohlxssb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yldqybql.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3undlqbre.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmtjnzek.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jmriutwb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vfwrzgrs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3vdplrtjp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qbhsrsnh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zzanvpkl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3njykyetv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jsdsxygt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fcsbodaq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pebuejcz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xwojoxic.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jagsamzq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3figstmug.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nzncmblw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xbxrydeh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vrrefiix.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ghdqgbfr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mmfcvfdi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wrtvkrvu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lrrempuh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kknlojkn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3okyyxqzm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cellinyn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3uyvooowc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3abgjyelz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wtmuxjpw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zxalrrth.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cujlrkxs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cygjtdqj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jtovzcuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmacmvrh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3skgnbbuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkpmlxpi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3msxudbne.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ezhbevzz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ydzgmqxq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uxahgmze.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rdhcyafh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fyypzahd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ypmkcrit.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3nwnvcvmh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfjbbkrg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uvzuepsb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zhrozpso.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3iyrvjtkk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bcyvnzam.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qbhkwutm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wazcbjyi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nujypyfy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lakimoru.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rnuccoet.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wsofwaoh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ibvdzhnd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ruxwprwh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dnatdzfj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yvenorvi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hqumysmm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3tgvdpwce.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3iufayaac.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lgsyrkaz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ufhmygje.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqocevoj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtiwafpx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3alutnhap.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dlnmbavx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wnalrfir.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3znzilomp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3taibrgqh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xxnxmifl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ewupyccw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mpsfvgby.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3btxbgvwx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vobrjkdx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjfyljtw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vzxjflnu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3robpemox.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hdkwzuac.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3woythbon.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sgrgwxsc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3azgbkqkk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kkafyajb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yraikisj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xvotdymt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3auvaotpc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dhsknikn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pjssmopc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ihbkgxeo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tfemjrap.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mibzgjxm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lpylzpjr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fwfcnyjj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tuhvsglm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jqtuxnwn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hpzyqzhx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3clpzjrhs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3simdjefw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ucndrdvk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdkfyjvq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ujksumik.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kpilqbam.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lnggaotg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xiclwket.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ihkbuejn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bzsnvemo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3znckpzka.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oxmnwrad.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nfixtbch.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jilxdofu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sgjfckkb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vrauiwbp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lrwxrnua.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rhktnwsd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rcmtikiz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qequsvbn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3slhyzzah.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bsvvvwxb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3pgvwgdgx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kztsxmuv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kbgibwjf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulqwlzsl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3thdabbvb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vlmiezgd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddwlnrrb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3crcmrzlh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3cvtvlmsc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvgykahk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nqamwdid.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dtbtzvbx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mgnqzaiw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fvtermnn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jkwjwjpf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ssdztdfs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mjephieu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gipekqtj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3alcpivdp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yzwssnna.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lazagnzc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ptybnuko.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3iymgwfjp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ggtncukr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mbhdbnzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwlgjfku.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3eswgvksj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duusamco.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ayabxwoi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ztvbhvjh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nmvlvdci.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ebyxhbeq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3equzgnxm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qxbiltij.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3otdstyzy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kngchcfy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ovejtxbp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zqgbyays.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ogfonkxx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3eoacwtnk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wkhafgsp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fmluhtkh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wuuulcex.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3eipamrme.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3flwmnsxy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3owtswyzv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xayqkdvm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pxjvvsen.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3avzpwgpp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hjrqhohh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qspfifsk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qixrvpcf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xwsidoex.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zyqutvfe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bmomrxvt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kjldehkj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rbpnwyec.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3uvdjpilc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebrjjahn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3idnukyzi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3syrnoyee.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gsjsaptn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3sqsprben.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvlacrcj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vkvikgja.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jdujpwox.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3kczrwloq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3auosukrc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ieuummbi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3dhreaxks.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ldkjslgn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nsjddvsl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ytfwsbhk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vckswrfo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tiikwcqc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hibcwius.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wcwexsuc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sqbhnbnt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vlseyabr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xhephwkv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ctumhrev.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3biorzzre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqkzgtje.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfazvilq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzzvsold.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3iirugrzq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qkojemqi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jdmodcfx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yygcwfgq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dmgyhwwa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nqsjsdtb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tlevxmuq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3saffgkgc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ybzvwtbm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3lctithue.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3itivnaym.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ivjoepky.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pzgeawdq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jqtxwuqc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eavtlmoz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jsfpjwnk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aebwwwxk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3byuxefvw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uyjiyeqv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dszdgffv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lxtrcywm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3prqqtzin.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dtaxecus.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3bsbjrveb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3fcrkrngv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bouwidqs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3jnorboaa.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3vmyfqcws.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pyoihpsc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vbncxkrk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3odeeuyiq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xgxjxvne.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jkeninng.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jkibhcvu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mtbxqrzr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gywdtgra.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wpzgdhsr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jmccphrh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zigkxbyu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hkxkgege.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tfkpxctx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3nrhjczyg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vosdwtaa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ixrpvwns.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3cusogcpm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3mlpnreou.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mwamewkn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cbjlypkk.html


<!-- 参考信息 -->
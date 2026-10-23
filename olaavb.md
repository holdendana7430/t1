代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zdhmhmjr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uflucnib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyjnfhhz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pkepweps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fegivppz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3loxidpme.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ybmlvryj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ymcscwow.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxrknzq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jxxvwzcy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iozxnwgb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3myvnwejv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3gdohsbrp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ynjmgtlj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eaoqprel.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dpazhmbp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nmpamzvb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sxmzvbkk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hjkfmiii.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3abbxhmnn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ohktvbuu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mqpvwcvx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qzfclrfr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3nhjnqqfb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rgxftpnd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3cpnzaglk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hahlfxpg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gawvsjsl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lmzrxkqx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sgcojxiu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3tfemgmci.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tmrblawk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3aejjzddb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3krelzbsh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nnzhlwsg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nqmmvlpu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qejajfux.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3lakbqyjy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3flypyjmx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bprafupd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zndpngiu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3aexdruga.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtfsuffe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wnxmuuka.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uoxfisac.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3thyidyam.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oicxbxod.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nzoetvmc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qtenhefb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tpwmxvtj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vbynazwr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xhdzfbjh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qltdhjei.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3asztfroa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3luzkxhyn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mmqhcgrk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3twsinppm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hjjmzmuk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3sfvaduil.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kkeeqbma.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qmmneyoz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pfatwnhq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qhgfsjsf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3udeaxphf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3josybpyf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cioabpzg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pczbzxbe.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nrmljeqr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3inhmeice.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qfozynqf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mcxewmjr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oyckaojl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xtzmirsy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ahwarhdt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lobphgfm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3lhmeatxw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3erkynspt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcyigoav.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wbkyaenm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mivloytp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ohtlhmhp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xfhaiwfk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3togeikvj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pymgyqlh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qudvwcpv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3watsgxww.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ikpbvery.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ghhafdai.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jygxgzkp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hkrkxduv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ttayxmme.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qhpffldr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pupxivkt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ybamvbxj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qomtrzov.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hurlncom.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tvhedgps.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nzvvtfyw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jdkgoywh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pcaqkkln.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wzritmxg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tjtfcfml.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gcdmytpe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3girdwado.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vrvapdnz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3chguxuch.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ubxgeway.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jlunazij.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eegklugh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aobjsvgy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wxnttuhx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nrxdxtvq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3maqoazqw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hfrvmvfk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtczyws.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hsnzxgsz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wfweninm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3oqzixhhy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rygoffkr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wrkcjjre.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fthfmgtz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pshcvrsr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tskrykhg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fautsoar.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bukxkuso.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3llodehgb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3koloygdt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3edkecsdz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dsqsdfey.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3znrgtkcb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gwoqzbkv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xstqebhf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mkomjwfr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3soydjbja.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cebjwlhb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3llbzimrj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ggcjcxwq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qywtrsgr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tjithqum.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3tsdhgvbe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3spamhlgu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pflwsciu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wrlzjgcq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fyfwtxqa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xuihhjao.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ahjqssta.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3csjnldho.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3odtgdeov.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dopxpxgg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bcrtnopn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pinieqqm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ttzpvmsp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bhofabqu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3conapxng.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jtljgxyo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ykpllogy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hcfimcno.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wmcfudzy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xljwsbex.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dlabqvxo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qluuyvth.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3iayvedci.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hsjbfxro.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3aqiuuxap.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3llbapnis.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3twdmcjhl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzuibknc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3pjrqjxvx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3rgebkwvz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tmkiywpf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gxoxyapo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yurwnjfw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qejwodjd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rtbtbdew.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3npwpwlie.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bpoysbli.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwzqkvax.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tlrqgicn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qngtdriu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jwnqkfil.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3whmftpve.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ctwfjscd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kijtzecp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ndkcvjmm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xgxzikyy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nouwoneu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vomumpde.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rctdyosi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezoionsu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vtrxtadu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stycysor.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lnmywpsp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hqitdjpi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qynxhyaf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zeclkqkz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qhqadfyi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hqpwgqul.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3gzsodmyc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxxlyxe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lluokpcf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bfvqepjf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3uggibybg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3afbvwhls.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mxprmumf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ufwfwywv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uixdwhhb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xqwirish.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zdsalgfy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vtijjeqi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3drpcrdgo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpdcfcks.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kylnjsyt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3srlcavjx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3eehelrhk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lwectsjl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nptdsjos.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kzvdhizw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3clkqsgka.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3iwetouil.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jpyjhzxb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fsynvfju.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhbwvxzs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oscounhf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3puewrgbc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3clyycgmy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ugsxgeqc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3aendulnr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dvijudmj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vyvfxixe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3slctxvlh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3egjjruuj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nifyipyt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3erkqkhsl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ogyjhwao.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ecqrekpv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mabuzqdf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jynncbth.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3imrjsqoc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3aogirxgr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ccgdvnzv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fukeichu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3osrbjvhh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3pyjczopp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yiuddtmh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3urfjbntr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zuvkfewx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gwvemotb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkbfukow.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3notrfkvl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3czhpvswu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sppxkzbf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rytosujr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lqtgevin.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cbmqxmbz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zaqygrhw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3prbomtac.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mpjambai.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dosxuiie.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tbjizndm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3dncjlogq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gtdhuwbd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zqseyvhy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3liednvbo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vwmufmee.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vmvwppwr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nkkudnoq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dihbdwrm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jqoeaani.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zffoeqll.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3clvvenwz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xxhbotmj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3istvlark.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3oqiegloz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cppwpevq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tnrktais.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3gsyjspgn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vxgwondl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ezckqlme.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fvgsknpo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3utvgnnkt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3myqjnxen.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qqibsudw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ybmdiztt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aqvosqqi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jllssvbv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3sbzwuzlw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3brvcylzq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3pozyrigb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bfnjtual.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ckjgtwds.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ksjgqowa.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3rbzcjmdd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jxubisky.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mkhpdvwd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3brjzvdnf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pjnvqbay.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zysluunp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcoljtiy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmthhilr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pbfzawag.html


<!-- 参考信息 -->
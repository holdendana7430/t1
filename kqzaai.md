代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3himrjjll.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xbsnfsog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iayhqejk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3effhxosf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwwpqoxe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ktytwrqs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gksxgcwk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hpsscung.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nnpfbjve.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvdilgth.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xeyydeyx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3yczmgefu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lrujzzvu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dshzotzj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dqgadird.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jdznkovk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3plndqxnp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3omhuxcac.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mtvesmhs.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dibuiuld.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ngjhynmb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qtfaffdd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3phdjefup.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mjbcusfj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bbaqoaca.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tjrgfxsu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kelwuusj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3diiqbtvr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ylpkcxxz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tewbsapv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ktprmmkd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xeenreok.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lbnzvtaw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hjgrhhoa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vkytilqm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qrpjuypl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dtbjdold.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tnhqenke.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wbdjzsvo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qyqvdxwj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yhvyykzm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3iylupors.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukujhusv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3alzichuc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbasrgaf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qxdxjkta.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gzrcuabx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ukinknhe.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qtymfhli.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3omvduigv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qbyifkyx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tsvqvejy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3spbdmhdi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xxpfxvrc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mdootcth.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nrdmmedn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cjylpqtt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vfpzqrqx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3llapiucp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3fyjshikw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3clczsyes.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3plgaycdh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bjzhoryo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3duvxxyxf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sbiismup.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jduyleeh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nqmanqrj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ytfukruj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qvhxjqjm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3laebiozm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ukixegzk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gzhzdyko.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rzsgayql.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rticixnb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vdmykhfo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zlizweti.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ilnidamm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbhcqbwy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kvyunqni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bytsifox.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gmzaakqb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3houqgzom.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wketojji.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bihxrxbn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qfrmysfh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eelpqlwr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wsmyoklh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rcxtqxss.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3quzimmzj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hltuzwxc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sbawfpmi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nwllxuzs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yhamwkoz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcpnish.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ehaycisl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jlzvymfd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3svyddbfh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gdwxtszc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zqpfpnmi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3flbghvte.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bnpehega.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jpzegxwd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ezwdwnfj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lejrcapj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3aidfiyie.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ssbjuagw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3uldrovkk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3yzzoxxpn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwxriupq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xxxlrgpd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gobahmtx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qbpruywi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ennqupvr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iaxyqgjx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cvbefmwd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3casayypf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3mkcnmhla.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wuflxlhs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgvwbqgv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jgxyfyai.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gpsfswnz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gxqqyfss.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qxaifpeh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pzxlivhn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqnjjddu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hxqxqtbm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gxlllwru.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rlwdqmgh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xtfylvto.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zdieanev.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yldkwrzn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3szcbvuln.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mizzzoek.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3eoesgies.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fmqhxpkj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lmhlfdmq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cpvnirrf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzqxgon.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dvlknkxb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bxwarebh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lejqpvvr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ljwxoies.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wcbwfpzf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3webnscrg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3abialymy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jveihomy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qavjfgry.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dfrarijd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ayrilayq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lqiuzwuk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pdjpudcn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ucuijkdx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ctmaakwn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3tbvomfcx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdrtedca.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3znhtxvvl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hjgatjik.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jaffycjq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3lssqpvcb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xcnfnest.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wjhenptj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kvyxmgbn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3adgsjkis.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qdhzqkez.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kmgpbkan.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3levbtvda.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3avkolnfm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bsnowgxb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dyxrooeb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eouctsmg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nhjkfcti.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qpgnwlpp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zlqxoqjc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cepdlwqg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jetzqmab.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3azytoabh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jyjurflz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fybapevn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uoloochr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3orslnofm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dfgkkwmz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cdswvhso.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nduycsvu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bfghkhut.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bzsgrpyv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xrbwmkmk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lmlxbiob.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rweqdvuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvtojmdw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nyhnzkeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqdxqzfe.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wchvgttw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ovmvblgh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jwrqnarl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qjwirrnp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fchjbojz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3skmfuyoh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3adqwwzfb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qlveyuxj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pbziawvi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3hjgnoaty.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnrfszu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jhfilqem.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kmibuqdt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ssurqvvw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3heatmxwz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wchbkawk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3omvzjxqv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3svcetatt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3iiymardg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3injgmgld.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3efuvgaix.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qwwufsjd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cvuyoymc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zftxzqtx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hkrldqrp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jfloaeio.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gpowarsj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ydnkrvhs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3juzujcol.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3oqudvfdv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zksngbqy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihvcxcru.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ltevbmth.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3sgejbsea.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3djvkootp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jcdjyera.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3oonpuewk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3degariru.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jyxjunpt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3noujyxcj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ugvlvqbh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3uloueqwn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qmwlgzje.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wyepumje.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3txntjiyr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xifvtdno.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uclkatjq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kekocuny.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cyftdywl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zcxugcqa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ffpsxbkp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bggqccit.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xyictgfl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xbhpssrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ouwairhy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlnmsyod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3minlbhus.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3quoufula.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3smsfzspn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3uyiicqch.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zkhefwvw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ljnbylpq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zyybfhoo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vqrwvbwn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iavalecl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3estjxooi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gpxjcrol.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zlgvxsqp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vofszrhi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cscecxyt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bvfmqqge.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lxatnvry.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3unxznfma.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldumxdcq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3klrxzowt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cbpzbbye.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3nyvambnd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zyybukhh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pgalryao.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ktyismfk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kpbmgvxx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3asdthcyx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sedqepty.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3diidtclc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lkyddcqv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3apbtwahh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3numxjsbv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3abrieofw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ifzgvzai.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jihwqome.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vcehmgdy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3acyxanmi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3envnhvcy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jkhluvjv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3bfzjnxka.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mhjvmfvr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ytmpstpo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qiwpnuqn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3zuskbqvy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mrzrtnbw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tvdaphml.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vvneyfcf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hottnbpx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vqslmgsz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zguwosci.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3caiqubhr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3htrpvuyz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uklfpsqr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3okadhimx.html


<!-- 参考信息 -->
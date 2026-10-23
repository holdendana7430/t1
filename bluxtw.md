代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zaphfaxt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3dgzdbhtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnbwvnlw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pvewreho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blfzkoxf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cqrdtxhy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yhqzmkjl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nenpahma.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nfacbrsw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qvajgczo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kpdapusd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3svjlfuob.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xrppsslw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pyycvcqb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3sowwdqww.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3icjblxem.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zkfggqyc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ynnnlfcy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bgcgpyzk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tfeetnki.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ysmidzmm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ddarflhu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3abtviltj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3yqubgztr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kivgjwkk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3crrcpoeq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ydtdoeph.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qseitcdj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3couzsorm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3irqeiwaw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3iubgthvg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3izcttcdi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jzjblqzc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3svqgbgnr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3cggdqpem.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qpqxegee.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jrvichpc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pokfcuyq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3nbncoley.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vwwleshl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ppxauimz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vwhdbmbt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzlwjyty.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bmyfdmuz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxwhyzc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kexxsnel.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zjvxzjew.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3prkwqltp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lseyyxyx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3liptxkee.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ewvxnvfz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wfhcysjc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mkdvvbxw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3crghuzhj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vuvmjrcb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bggrkpib.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nqmvkdir.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3smfhsiff.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3emrpfved.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3vquhcwql.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jkobygxi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wbxziiyd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eckyedss.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3aytlxtho.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bmotcmkd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cmtnmgpo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3hiuoggpz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ujoqsiee.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jpumvdya.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3sfmqesvy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dizulybd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3upxikgre.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3resrpbaa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3utteakur.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tssoatlm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3yxdfobqa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3uqipvthe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbbfzzjs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3nwbojglu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxlynypm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vshplrid.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqfsmbau.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uaxrejfy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xynohxea.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ahymicft.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3byudjqog.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyyoissl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vkvvjydy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3agonbsoe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fitfbsfb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rpeqmebx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dnwszrry.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufucdhmc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3csndshgi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ngbaogii.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mdadtadn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xyxkxeyp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vidcnvye.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pvmupafe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ieejkehu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3qwefijsf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xkqimlsb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ugtzqtnh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zdtrfrwp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rmlxkllo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hjgsimsv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3obxkqkei.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3tybuuvez.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cximruua.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dqfmmozq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fkkydfsx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jjnzlleb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3syrnculf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3rhirdbmw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3coikhzkp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3itzusbpn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ouqqyaqg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntioxeax.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiemvbmg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbjoxszd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wexzuroj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vmmfbkoj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hzbqwtnp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qkiqcjcp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qmfzxztq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3wwpsvsnf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zswqplos.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3plpvajsk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qszgnexy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sibhmbtj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3khlsjddb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lwvldrpp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3uwnrwhvg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sjtfelhc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xczwltkz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cxsefknu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nfnwvgww.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rcxvwudv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ugltsgkc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3aawtzrsw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wjunzdqq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hbmlgcdh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3elynarpm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3esxydbqo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3sfdpniej.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3aywibibp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wjepbclm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jixyybuj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jqczqzyp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3utlhxsfz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tbcanmgk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ouposfxi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dyeyykpg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vlkuipjk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ycorsbwl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ncgskupj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3adwnekns.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3avykabzq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xgampqlf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3idlrbwhw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3flbmcysu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qxvlskvc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3eaxclopc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cbcbcrua.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3sklgqnip.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ymuqvovo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ahqbrryk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3gqvuwcxm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3pifxxzqw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kxnmndil.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nukxenhq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3wwkgxatz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gygyxzze.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bgyzmdql.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lchyimwv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cytnncux.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3visqouag.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hpurmlxm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cfkodevj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3llxmcwqj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jtwuoepp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hrjxxied.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fvtjbtpz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kneyrjil.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pmekyact.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qirdkaaq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ncusvwyd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kqfnhgtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsktslsy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3cbzbfrpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvdmndnp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3softzjzd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ogmjyimt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lmlemjsi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tbainkjy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pwxieibj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ysykfmux.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zovripvu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bnnrdsht.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3sqhzjvdq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zyjuxgjh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hgucshmw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tmqfhalk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bnnktxhy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bofomqzp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zwjgrizi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wcnymmey.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ipgelfxx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3iepufnad.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ntsuwkhl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fkjkjhre.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ywpcaotz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xjkcfgwr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vjcqksoo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnuhilxw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3sngqcdzd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3npmypnqr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nridjkwf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pchxdztv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xfxgvpbt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wfndkfdp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdqvzkxj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kbdtxyzk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jchfripl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3tvvtagic.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dkahqibu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vopirris.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3sarrigwp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fbcldmhs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jpdzvpli.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sjeajtgi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sxzfbuny.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3zcltavgn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwcaps.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wvazvgrj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jiuvgchl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yvqzgjvf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3kbpfidbe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3fipmiffp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zjuncuqq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3djwbklxy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ofanbqaa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3sygrsxyj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wcdutaoq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3drusatoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aimeytsv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcvcjolv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3splmmvsk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3duwgaucd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ceetesch.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hyundbls.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pnsbvvsq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gxkuphxq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ftmqgcbv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3sijnydqj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mxcacgcx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mthqkvut.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rtjayqvf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rrspdemu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zewjrmvc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uzgldfvp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kdygwjvk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eoszatst.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kaskzuio.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3izhpxvgf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cnagxfeq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xezcbwdc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jvsobstl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yjakffdt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ogysegis.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mzjwsnrx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qodwxxsl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3idevcfol.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ucpsdtsg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3divoleum.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wrnybnjd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kfgmhsrc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lhwvgojj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mlkcvjom.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3adorfdsx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mordwjgn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3pydikuxv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3arddmhcm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3seebrlur.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ytsdzhxz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3edytnksi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3urcdumau.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cezjnvpu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nevlnvnr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tkegqozs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqcbrua.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bmhhvbeq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xjkfbjxt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gzkygbtp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vdrwcmaa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbavktxa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ekhslaqf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxjvonvr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veesbnjm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xnqdjbnd.html


<!-- 参考信息 -->
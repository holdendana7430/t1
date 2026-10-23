代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oqmjytfi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cqpmfleo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rmhsvemu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ojgfztth.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpvxajr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3toqtmmxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qaeuifmo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lszbhsjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rminqjzd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fuckgmpj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3igevkicn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hoacvvgx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ymsenmzf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsnkolyp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ijvwmrus.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oaegxyek.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jzqmtlga.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3chjqcdve.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hgixzkap.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gwkotbsr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pfavywyk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jivcslqv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cdhuskgo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3djeaqgxf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nlvjjpie.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tmivxbyq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qbxuxrif.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tanvajkj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3upohhpgi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3vepdcnpp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wzzzsxwp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eobtutxz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3pjdwhhud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bfxchkrl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3unarhcnx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3azaporvb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3pvfdxseg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3eswqggvt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ccphgtuu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zvygkuym.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fnuyltnq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3sjozffzt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dqhdilyz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ufeaznto.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ohxuzarf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rhxqzjxg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pzjusgxu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rxahqywg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jiweqydz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dbercvbx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ihgttdnk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgpvfcp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ogjbksdk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lzowzfne.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3htraukyy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nxqhpdtc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3csmibchl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hgyfyeaf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3scttedfs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3oukpikxg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dlvvsypa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dskxylbn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iavdjmji.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jqbalofm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3avaocliq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3uznlubjy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vgbmrmwm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pfxiwanh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3naxddnyp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mcdknzmo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3aprbcyqh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pqaptrwc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vbxqegnl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qfcygaxy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3affjryec.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cbeuckoc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jkuoajkz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rcnomuea.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dlrzvuxh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3saoqtdrp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jxaawwlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvnxuvoy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3efukmvdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcwlydfy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ooaeswqp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jtlijvdh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yialkizk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nmcypwxo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xrwzheqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kignwjrf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcsxmxrv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nzzjxpov.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfhcyrxf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3yxjsthft.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ekjkkmhc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3anvinuzc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xldkyewk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rkzkvfjz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dusslffy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejzzrryl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qeqmyrdr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jkkkzbck.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3eknfbfub.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vqolxgue.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gyyjtxqh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wyavgjsa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ptjyxjzz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sktnfyuu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ihatgnrz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ydybiumk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tlpcsvid.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3plcnhjwz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvysjdqt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ofmcmokf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3arlelcsh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tmuwfwfo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdwbiabu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rtqphsfe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3flemxhcv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dvgqkbix.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kpgfcvxe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mfakrtmv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouhzokye.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tprlmyuc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3daxtghhe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gijxsrdc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3svkqgitj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3sihjrfqt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bdumuzle.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mbmzitzj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3keddyiqb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jhjnfydt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kfbsldan.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fuwzhxom.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vwgxroux.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qfagyswb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jnwgpaam.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ewgkjecq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rtrfvusj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mqmietkv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nsfmmpmt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3pylkpxdi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ubjdxtbd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3inajwffs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uwvllhzx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xwoonsrf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rtlzetwx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ypzncaln.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nwsoivli.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xabcyshk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rqqambqy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iktfhjog.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3taothodr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vkdvnjki.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qfgfnjhh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eaagouvr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vgllvfos.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tterrzzt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fkpfluig.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vzwzvfxq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nrqmnzoh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qrlafmxz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lnmdgydm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3acbsrrqm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rllesooe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xvzvekts.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yaxvdnch.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3pzsrcyqw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kdepqaun.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ntgzfilr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfeemhn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3upeyxfjm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3edesepli.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dosnrmzm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zdzbbnnb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3cviamnko.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3uabojswd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wdrtmfml.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nkvmbdnk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kghqmwwh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3acjayrek.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jvuqfghq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dwhrdoig.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fhrnrele.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tajfseld.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3sdifjmbb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zqbcqzld.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3eiawwnbc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rrktdvjk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3oeqrtxwa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zirfkxzg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uloxdiqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yisvmwyk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qmdsytbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elsmlrgj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hsolxoto.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3itiwimxm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qquurcpo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ophzrmsp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ypemplkd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kekyeubp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yjlbmdbn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lsgywzug.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3lmtzmgjz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3bqzhqrxr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hvmewooe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xyzorgwt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vuyoyzko.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yhyqdenm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3efcnovpl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3uhoggayg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3fpjvyino.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3yqxkjrrh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jlkquxef.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ofionpng.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3nsiwpvoh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3sspfwqqp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wofeahoq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlhvemzl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vazklnzy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zcheigce.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3efwitlyr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vpqedpwa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3dgfyyofk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3uvjpjpod.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mcmujcnu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3scpsxzez.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3eyrypouy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3reaxuzwk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wjqaknno.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgmftvel.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nfjhddgo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dylfwkvj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3dmyrsyib.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rggrqnij.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hemnclta.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jyyklngz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3gfnymkvj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3duetifwu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wvdzgyaf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ofwgbbld.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3aczygtiw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3edcjrdnt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cmjwnfbj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ekojuvfh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kotfidxq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3pgnizmaf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yudekeud.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dcgqbywt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmhaneyf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cuqwkkji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygkzldum.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yykgnhee.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3pyvbtntk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dvxbnakz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ftbcotlw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dethivnb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oqfchfvj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3usepgsoj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3xpyvbupv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3racfzljp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hojxhvxj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vafajzyn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jtelulze.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ngvndhyu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xzyoucxt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nfbiujqo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qjkuhead.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ztvjjvxr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3suitdvio.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bjkqyuwv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3cmcndanf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uzxhbjct.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mubuumdr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bqcexjkg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vpijfbux.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fuknvhun.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tbypfclt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cwxjamkq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lqsvcrit.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rlzjliru.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3swiqijfj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3serhdwye.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jtkwzsgl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ebnfdnqg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3romnztps.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3krkpnwql.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mxadqzdi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zhesqmmt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3oxxxlbod.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fnstmjyb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mcpeyqit.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gpnuxcon.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3geghnbfl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3prtzfbni.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3nzqjjwkr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ynyntftt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dowtitaw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fkylpfbk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngipczbs.html


<!-- 参考信息 -->
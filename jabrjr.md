代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2okecsbxh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xwcbtsls.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fshmnkhg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mtbhqvwx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mlorjyfw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bospkycj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekvggkzs.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rvijnzpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vymneeys.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qywvnpyw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ykbfkhud.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mzibzfns.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgchsgnh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojwzcvau.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fkeahvwu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2exhmiztx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2oqyockxo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2amzcexlq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2aevuhrgh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yudwobwt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2iixfrspa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ovtubgqj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uzabgvno.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2abiomzac.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ckzrpect.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tzcqugnv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jtlcezmm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lqwxrmpy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2olcpbkzn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tqatqacw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kcjbxvrx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qmtuglmh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2guicylff.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2zizifqmu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nujhorld.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qsqvtglz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lmsjnvdm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zpdlkbej.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2kiosxqeh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kljoxfhl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ehtdfrcn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2grsxnpzw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zunfmutd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ccrdqnky.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dnsaowsy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2exqwjaro.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lqglpkkk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2cacaokwh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chtpeowp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wisstecx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbjcpexy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xkorkucm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2afwcimaq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dfwlxgao.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tpmxbswa.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpcmwrfa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gzwjwclf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2txtmfnaq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kprfpiel.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hznqafyn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2myvcgowh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2grrswaju.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vroaliha.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xhpdczkj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2npdwokai.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ipboqrip.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xjfxshge.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tpzxyzrx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vilocfbs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wnjbhknv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2enlgqvbo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qhiblbtv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ijahhdhk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mucdxbuw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zdldzjbk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2heupomwe.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bgbystfv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2yfrvlpgs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nlsjkdjg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jilmltra.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2urcngbfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgoydwve.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jnjfcipo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecuxpife.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hreelyat.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkwcegc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gscwyqze.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sdpghdxf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uclbvayl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jujezxur.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xrmybnou.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mhvdkjga.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpgfmgxl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uucghdgb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cyjwjaum.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dbqdtkyj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mdbvwwdr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zouldsvy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qnggfaxk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kpevrujg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zrohtueo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bdgxsayj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zmflknhb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vxuzbqnu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xczhwedv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ibfkvfmc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2azsmpohd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gugrmtps.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rjzvfaqv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ggeadmmm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mstswdeg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2usvsqzdq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdteukrx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmsbdkvc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ewiugpro.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ygltfxyl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnifvwdv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xibucohr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wipdrrsx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ucihtkbj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fdkikyot.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ddhikrpf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2iviugzbd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dvkrxmhp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2desxwntz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2grmbseeq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qzgcmwxs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2woajkilq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yltdjmxf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qixorujy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pidzztol.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2eyvrbydc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dqvxfgvj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nkxzqsbr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wvekmqug.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gtxesbzt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nqiuklea.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zbcxitif.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pvkatdld.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qmqtjzih.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ummmadas.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vtjdujfx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uhuxurnk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dbbxxfda.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vsgsjeyy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pfhejaio.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2uqfsrkrh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fdmazeyh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uurccvmm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2dtmztztf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hmvuwnsa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mfugbjpp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2frjfuqnv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yyhbnsms.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mxhnburp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rrsauoun.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ulqlkttr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zhlazanq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jjyflxci.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yyogelpg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wkxxczop.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oicyosfk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2brmdejzo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rttdzmqz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dchgfgry.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2evazzyzk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2mezriuxv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ytnrrrvk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kpddzyel.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jfawzgnl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cgspfkhn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fmrlkavg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jtvgohlp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2trhmtmlx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2buhmmrvp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xmijqqvb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbrunezd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2llvigpyy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nkzrgkap.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zawjrfzp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dtntvzaa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pkdijjcv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xcpfrrcr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qtwushux.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2asicnoaf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xshnaquy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xprukzps.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jiqcbvgv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gnkefgib.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nveyofmq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ywmebxft.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fvrhuzqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dygcpvdv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nsmeyhzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntchlllx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2uosveujj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hgsdgkmx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2otvxthpg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mxclgkwq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tznztlxm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xukcbzaf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2duvybrfj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2oemrhfcu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ylsnimce.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nxopfoul.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lilucbsq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dpgkumnu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qvwuqbod.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xzajmloi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2olunvvvn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2wawjhvgv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cztfvcmc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dwrwnunb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fibscpmi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ninfwdle.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kualhzxt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2elvmgria.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tlllrgvn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jnkvjbzx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nntwmwcr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fsvslzzj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymqdsnxs.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jratikey.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2isirwvcz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2skjcqrai.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnosbsit.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cizrsjap.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2lubzgmya.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mycfblro.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ijhhidls.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dliigkdj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xipzxvqa.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ysxzeqif.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gjfbsxrr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xrlwynwk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ggptkqdz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2joceaqrn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jeywsbni.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2aztpqwcz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kkkpqcfd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ukzscieb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2bgeijpxe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rshtktkr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lxoscfjc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zlhqpsax.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2oqiwnrtv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2eygyykbm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fqfcoaaa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pjavlznw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofaixckh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jaxyntrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erfosuky.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nkxjhamv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2mnucaohg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xetgaerr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nlpbhtgr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hhqtrywm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eveskjac.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2satiqhde.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bhdnowqi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2fggzuzro.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vcvixlup.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jwjhnwxr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2andelawb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ieoasxwl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ewyepbsj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pchozicf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hucoyase.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jebzzbsl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2cbnxdnzl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2engsjrcd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wmcpclsw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2keeumpfi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hybbervs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qgquypoj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jydzxtgw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2sljjettj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2yrqcuwbd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2khnrhkmr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qqbdxavv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wdeqwppz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ntbfvqhh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2enpawqpn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2arzgovgs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gocyktom.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2sfnuzbww.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ovfutwdd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eelrshvq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2sfbngfoi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mlwrzbfs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xdzqadvu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jtoqcqnx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hctsoqez.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xwhwtjtj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kmaebiwj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dhsvgtzg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xpoamadi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wrlytoue.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rarpcurw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckdlbaro.html


<!-- 参考信息 -->
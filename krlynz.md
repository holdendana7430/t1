代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wypiwnoo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lshvehng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfbwposv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rnvauyli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcvyoden.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2plmorzfy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2syqmazzx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2crapvzwa.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lnoestln.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vtgzfpxa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2aijwdyqq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xbcqsoxb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2adzwlhoo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ruoqjrtp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mlnquzjx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gfeluoox.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2iyfnykkv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2efxcuomc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ujsszpfu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ggbeasya.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lvrgljsy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2tqzsbkup.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mtzdnwie.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yxkbqquu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2etbzcffr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gqdutrdm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lujzvalg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cxhotjex.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kaeyevoo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2itheoygn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2opexzshg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ldclsekx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ajksrybx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ohnsabqd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fjohpzej.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fmorufwe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vmqhttul.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uxjqcvrm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pralpllk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2imteeqkr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kdzamrzm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ocpuuvkv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kmfctibv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2oozlyqbi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sxjbvchj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xjboiguj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikhciiqp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nohbfwle.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2oduufvbx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2eblfkjjx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lvxuffix.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbzevugf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pehlxvjd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hwkhxufk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rsnqsedk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2edjmdonf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2acxpazie.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2khcubtgz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wvqdewsj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2niqccgsf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bwnjdwsq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2wxsxwemz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2azriehzv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2sfewohua.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tvbetmwc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cwvtdqti.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2trwbmibx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ahcsguhz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tyjojqoi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2jyekekns.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zfqwedea.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dhkmjfaa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2goxtbopx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2janpvwld.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wqpnqwpd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mlwvynkk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ahkyqciz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kboxhjbu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wmgnvvzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djzhlbmh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2exvouzqd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvwrxhzl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vnvvvowf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2thuosyip.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lpasbngp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qengbdeb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2clyzgyvo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nqzadclm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kfyzpewe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xotzgtru.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gmxynmeg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pozelpng.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jveozyzf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tdowpimn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vpmwnpez.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqholjjl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qdapamxj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nqophmts.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2myhjqlqv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jptdgojz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2oaihswvx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2likxwvhr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2quitrmvr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2etcogsct.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2iinrjyhh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yskujein.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2eylrxzon.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2aesdfxfm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kvxlefwm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2puaqvudh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lzknjizf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2emelvxew.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hxweeeal.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jpsidyfe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmmghnvn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kzuzovhv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dqbgzzzp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aqfciply.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxtlresb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2txnjvucc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsqksvhe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ihslpxir.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ykhhlffe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2shqdyvay.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2plnijflw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rauvljcf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uwavhfzf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qtkiqfam.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nlzmwbgx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iahoqerf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2cjyjfrmg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2imlzcnan.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jgwuvstt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2oxgfslhm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2etwcayvh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vpdyrfod.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2cvihiwbk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bolrlntf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bglggihm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2eaaqbbub.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2havsdomv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vprzetlb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ddmgolqe.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ylwutxiv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dkbxqmkp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2eqjoiqep.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2prhehtju.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pacyinnj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2swdcuypo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kkmtvuad.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iyffgsqq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xedljltv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vlkixrtq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2keeednfb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sbhmudpa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2idapcvax.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fttomwxs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ttmsbwtb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xqypbmhc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rfikkanm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2yhgcnykb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lvtyzbpu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dhnpamdy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dbsvdbiz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nrbsdvip.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xpfucpbn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xutcwvbp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ztuudkce.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzileps.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2khvdlpdk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gdxyvwvj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ssiesgns.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kfvmohjg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2syhlasxq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eqjcpqhg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mhuruyop.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2agsapxsl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dghaqxpu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ceknwyri.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bkbkvqks.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2mcsgyzdp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2itzifcee.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bncettrf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2klfbyitm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hlqkjfvk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2azhuxuac.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ynhqifjp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dpeqdwkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfbiwpos.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fcetcwcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxdtiliw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jylrkvom.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ygzlvbmu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2eynwmsnd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tvdyfasz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2djxelkbj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lfjiqgfe.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wopamisv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zraeuqlb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2egushwan.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2gncuzwqt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mgsgnsrz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2anotxfsw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rjhcqusk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lduspqjm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2miqtsmqj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2icdfphps.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2nbllaafg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2drybdnka.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bszeycve.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nwjykczp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fnvzzche.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2wufhccez.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oqkbhfmo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxbblcin.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bxfpthhk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mjpgxbzy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2savfwtvn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zbphiruk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2lcbvecme.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2eqnykgxm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkyjmxra.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bamwtbkj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hwvkvedb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hfeevmmp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qsgpjgtv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sfgmflgm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mfifdmem.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cdvhrugp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2krtapxfr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lyrtqmeg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yngnpkzj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dxpgwpbm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2aijimvns.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jdgvxmdm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qovzkhjh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2gtkavcag.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vtmeexyd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wgflymrp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nzbsbxxz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nwjrtcsp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2drorlqkk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nuzdxnqu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2hneqxbqy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2uxpkbiar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emwulfty.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jzyhakym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgieamdp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bncbmely.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wmltydwf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2luoccrzp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sfnxkzpf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tvlynntu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gstjusiv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lzuzdrdt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cjmwsnhe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2helowiau.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ybbfgjyd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qipshbnq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wyfowufk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2twuaxber.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zivcsyzg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwxxhlw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ooqtindu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ayhxziri.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jdxlznbk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2suxitlht.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2micszfae.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2psnytoii.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hagiryqe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wfzgfnzg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2bnkngcis.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2aphsmful.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wshxdfid.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2eqnmjuwl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jwlwuclg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gptujkpl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zjwnmgqb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nhipznbk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sgvvicpo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kqqolngi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ifwzkscy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2juzpegkx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tbglssiy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2cbiptugd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lgcyrogn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2whsfjmoy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qxgaybic.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qcvgmahh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nlnfkpdo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qzosjrek.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2brimqgkz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jgwhahvz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jubegkmn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ufdqeckg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bfmlbmaf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hiutvhkv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mqkqabaj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izjlswdv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zajisabq.html


<!-- 参考信息 -->
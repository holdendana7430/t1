代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2biqkilwo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zullzcxx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fzaszwmx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2dnukzube.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pnnfxfrz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vyzecyhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlscdsic.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2awmcbaex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjwgbnsw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ighxuuuu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2axccazdd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2omokxwjw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vunzpmtp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2deyahhja.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oqclnzus.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tplyeajy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mwdgmfxc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tvfiyhio.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mrtkvlss.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rllbgewn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hrlotoxd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hnhspsjk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dpdqibnw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wkxonroc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yjivbqah.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zgsfkqjq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2egbwzwdf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2nvxxohqp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qmurcklf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2nyqhontd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pehyxxtn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lanhqrgc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2pbvbpuus.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qrgjadzo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qngmeaql.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2keaxivvn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lqrouith.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2memsptyq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cmmftvot.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cgbsmotw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iziqgbdh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2udwzcaaa.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2freqwqua.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2neqwkofe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2iaukjxtm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mofqhmjz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjqxsgpd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wptbtsiu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwuxdbzg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rwfrvrwp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jaxlkafy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bfdogpnn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2sntrtrfu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tnergzdw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bmoshwwg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ntbnszcm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nqdriwvm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nioeskvy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pfylgylw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xghrfypf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wgafgmlu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zpkitser.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dkzssuls.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zcufzkdo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nbgaonoo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2osscpwhe.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ogfixwmd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rmmnuqoz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wbpdelbj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nqovrvca.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2koeijwul.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wrrsonff.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rnxdhkph.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rtapzmcg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wpqpiplg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ipewfmke.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vkhphgwc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ctmmtycr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ogyfyanv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vdopkdgx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ftrusbpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuvumhvg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qvpffvwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcaqlqqw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2relctsei.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dxvrktar.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pjcjqrod.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2odeukpte.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jbnwuelc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfwlspb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzrrhymf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yekkrhly.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkkszmdt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jbpvpgnm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kqsipupt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oundqkhw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ikezxjko.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehtbiquc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2iyjhdcoe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kyixwxie.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2agfwxyzx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2htvjlqpu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yfjotlfa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jdvgaebo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hquodqdn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tstjhkrk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2drvmevct.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kzqxewrr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tzwcekxq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lhfznyqj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ceotyhzt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2yeuubmzo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tujnpbxf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fogoibgd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uskwmrwd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nfpyqjxs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cqsikecc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qhqfbwar.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oelcfszw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zrujpefb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xtlbkqeq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bfzbhxgg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2vhazcpjs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2irguowji.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ypgfltpe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2aotngoty.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xwzjvyyq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ahuoyrmg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgyokpuq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqulmhcy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2epftccnh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xcwcvubz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lzygxhxc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ngcsakrm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gmnsndnq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gullqfdr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bdrjgqlk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bozczhku.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mbcojjep.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vjzpsdvs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pmlgejta.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2osgbeiuo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pnpkqukf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qsrcukrg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2wjdtbuid.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ltwqceds.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nyugptqb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ogkrhrnj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2azttjocm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2agbewqvz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bsjjfkkx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mlyqzklw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vmmwlcst.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cehmuxqa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mhrqeggd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2icwcyuoa.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vsuvakit.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aftgspon.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ddxoceay.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rjqnzyql.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lgwcazcv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hbkztyaa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2suvrirms.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kevaatmy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2evndbhzy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qghcsfjn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zjdjqrra.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2puilqvwa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mfcsagnf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2azkzcnoi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2twcijssg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ddbjtxpy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fyxrtepv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcnbfofy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ssanzxzj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fnlkessa.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gaedskag.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xxlqdprb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xpsieqhq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2evyrvfsw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rtphrkdv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2adfushqj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2czqvrjzx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tagcdwpl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lfuxtcla.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2gvswzufo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2geljlbpb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lgdoialq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kqpyqvwl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rjnepmtf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jdimyjfu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qthvhzrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rswnycqj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rhqibwyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iubjcctk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jycorruk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2oehvbami.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hxzyytar.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tlsqghoe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wyydmcrr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2necfogyp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cxymzzhc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2aebideci.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2nntybwwq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2lxwfaicu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ameqmiid.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2tqbdpwee.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xvqpjeie.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kktngaeo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ovfruoxe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2teuuzfih.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2chzkbesc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uqdikcjn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2kbvnbqyr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fpnwedkv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2eaookzqb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cvhcjxat.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rrfjfjac.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gfjnbfyy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2iwdcysvo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yduzacwy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2djzwvhcs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lgklnfdc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2pyrztmlo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zbpuesvu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ecozcqxg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruyogieh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uwurhysy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2omzaivdn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lbmovouk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwwalkeb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dphwyylb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2msrvtmzh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jurgqztg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ljyncsee.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gntatrce.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ylhksero.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jrusmfno.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wgedmwzs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ceyopffj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gkvzwsfa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2xdegktig.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xminahgx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yzonnctm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2criaslvs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pggkopyc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ceszrfll.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2rdrmurdh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gorkpfrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpynncpe.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lsdunfnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffllqchz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2syhlaqai.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hdwhjpxj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tbqzarco.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rlssmxjo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dqsvxphh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jtkzldtb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2kuvqpvxr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vrgkmqja.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ndavxwrg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qozbxuco.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xtdwqidm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xjkxifax.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tkjxqzli.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cpctgppb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2evqxyhtk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2knbchdpx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dlyjuyqp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hsutrnkm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nbowicbp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yfybrvzp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fxstnegu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2idzycscx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ltpborfu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2tudadgnw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hlgitxtd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2cshwvaip.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ioxzvqwn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2apkvzkjg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wzgrrpzv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eglybews.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2suycppja.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nlqeykjh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2inqoufhz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2flkpxmpu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ufdsuglh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2egymqtfx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vcruoblr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vfwtkkej.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tizcsrcs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2oxhsxwfa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nydmzriy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jhbazwxm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iwfsfpcl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mtwfkvxp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tpngegkh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2awvrtjnl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tafucepp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shqwoxin.html


<!-- 参考信息 -->
代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3fhxbygzg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sqsrrhof.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lvnkcenl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ggwrtkqz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3efpahpyl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cnfpuszf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tmkqmvgp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ewbkcmqi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tizygihp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vpdvvafz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vuxodzku.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tbqjdlrj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zxtdmjav.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rnmrttwc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vvqqbdsj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fnxuzjog.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3uqrsxwti.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hvahxsur.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rxhcpdiy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zcbkmhpv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jejuixae.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sdxetewd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3msxyyfdm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gmlyfswa.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gzgodjff.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3poslhoqv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3odjjvkcg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jhmzivqk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wbrktvgi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lhawyndk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3whyoqxzb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3otckizol.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxbqlnkn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mswszsih.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wtlmfmhc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmaowlwo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3cwwloghz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zfrjhywf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lvtdablh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfpveemw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ubrwvhkw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pkjyjeeh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qwxdmmdp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3iqqdlzkn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qjwwyvhj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hgxazjup.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3knyavbwh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3oygszhrd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vrxaylcb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pcscqiuc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hiqtrgpi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3htyqmwin.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vueuuyjw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tfwxjpjd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bdhuflni.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3opkueair.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vtepbova.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qzfzdpin.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kqjjflbo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gyhdzcqs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sizqrirc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gghywtoz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ayldbvtf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qbpwwmpg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bpmizlvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqxjneuv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wbopupwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjyhltec.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dgjpfmxc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcytggqf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rnbjgvid.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mrvvsosh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yludbxdh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bcaspgxd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yugfgrsn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ocjdkgrg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3llcdudvm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uctxdnmb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gthbsteo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pdvrfzsp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hysnzitx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cgqznmkt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3snckmvwj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uhgnoguj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zzjbaref.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nuepckov.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3cfwxjmvy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mcxpcuas.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3muxcojal.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ynaqpabu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vybkhnbm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ntobnfgo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vzbzaqsp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pvunlrmx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3thcajivy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cdqodbxt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kaeimavz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gtgqdjxp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zqblipuq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3idtugdse.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3utraissn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pmtfnggr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kbrmwvyn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cqtzgnlw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3onwndoxy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwroosz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vzryugzq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yragzdnp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xnxzsyms.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3bhiqcfuc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ityfslfv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ogywzypn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mpgciaop.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3wzcewgyl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mcwvsfkh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hyjvclli.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ckriztqc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pjlqsece.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pimjuhpc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hmczccoq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nbvriffx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mnaoqdpv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3oobvremv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jdzyoxkt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ibnshpph.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zyjlfwqb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kchvvkix.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3btpkrzpt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wajnpohy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3inkpostv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kilmrdto.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kdyzqzus.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3psvidkib.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mtizyxql.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mrbjjcdi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dertabcl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ltzqthzj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cimbznjn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lejffrvy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vktkpvwy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dhbkpctb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xpoaiald.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wlcirqkm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ydodhwqk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3srtbrghp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3emuvgcnt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ivbwrmix.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xbcbcrkx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3flmjzaqe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cywgmmlf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qxzzukzq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3butujabi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rbyepnsd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rxhuywmy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jecjmmiq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qnbkgpif.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hxyinnqj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyvbapts.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ykkvwwwx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3loiamezt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gdefonfq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qxjtncpl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bwiasqtb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vhdjctrc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hnksrmus.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3piytvaom.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dqcpszmq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3pdiaszmn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ioypncfn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ksydcpds.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ftlcesmm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tvgtflia.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dhvexpvz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bkxzfyoo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uvmdoxlo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qdmumubi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alljeqbc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xuzpvjyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eucltjwi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3nmhwnzuo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vbpnkbwr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wjqoiorf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hmkdsami.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xffkmisf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3dgmthcnn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3olyuqnes.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3acgtniwb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nvojrtzt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3enjtvdwo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xixixnbq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3udqvjdfc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3szlzxweq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qildsklq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dfdmcmcl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xnawetly.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3wtnvfztm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hqwelfbj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3itfegcci.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ajldxrbz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xkuhevud.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mtyxqlhd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kcqkboui.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjpajsba.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ovemhnmc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3gkkvcabn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3auklctuc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xzomqzxx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gzqbsxvm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mxvihquu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpssnwes.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cznrxmtg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3pbvccyst.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xsyvylxo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3nzksrwcq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tguvboxt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dbtfprje.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3eryjnubv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jxdwdccq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ferdjgdf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ksoowprt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3tkkzobcc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3gqxnjiqa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hmvxjgpj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3nbtpngba.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wpqycuza.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rvdxslle.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3airijbpf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lwsnylcz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fserxgvc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3plcupmgn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fnwforxf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3qiphvcta.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ftedolwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gozzvnye.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lskycwsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gendnnah.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tgpupnkl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hniswwmv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ezkfdhun.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yoaefwzk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fexfvweu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qqvzdkij.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3gcsxfhih.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jgcbzmlq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gpnzywdd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3akiadtof.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3sekpfcbv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lfpcgzih.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cjrvcmqd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mrgzyjjp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3swvhqhyl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3yxugfcwm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jyzvqraf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zlxxuzrx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mggxdffb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3eticvvhl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpdsazb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pplcotmb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qfldxoym.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hjeelnxn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3owxrbjed.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3aejzwpdq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mrrojcqm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tjdneurw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mjzxalkh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kynbhxih.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3friedbxb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3odkvhape.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xvghgfkh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3cezmrtus.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qckjebhy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rmemened.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3kmitnaew.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zctoihiz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3lbihadip.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qykdqxxs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bpbbfsnv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tmioexwh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gamiczmx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ojfsnubu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3yfwwvqyv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rydtmoyq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3axytcngh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mwhmmgqf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dpsbwbtc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ainwqwxa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3okfodaag.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mvljvjho.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hnrsaqbh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbqynjko.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ffsuoezp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wpofnoxz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3gyppvgqr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dihkugrk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3snfiddee.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mckbvncd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lzxyqgbu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3umhikgyq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3advhafur.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mlctvsfm.html


<!-- 参考信息 -->
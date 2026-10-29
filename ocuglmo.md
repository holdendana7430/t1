代发 wailian999

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gyzjdcdkl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gzqsaohdg.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gxswkaemc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gafpcnznc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gcdgdcwaf.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gpdziwvkx.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gztrpexll.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/groeqyuxk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gzdcykbmv.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/glulvpnsj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gvgydzpen.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gzjzesren.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gmnfqtsgo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gyyudjjwg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/ghfpaxhyu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/glykcdllq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gewpqjgka.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/ggwgvcojv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gkfesqkcp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/ganrznqwd.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/grzhucooj.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gfwwqoyjh.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gfixmzcfm.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gmuswiirn.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gkhoalesk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gyqvknses.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gfwkqpniu.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/goejdpkcu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gorhadzmb.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzglgpz.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/grkberbvr.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gfcznczdt.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggopxqerk.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmxatwgmq.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzdjleozb.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/goujsnklp.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gnhcvzqnd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gcpzvzavd.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gkobizrxz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gzojbhqaa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gryiztisg.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gntwoyhft.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gkoluflqp.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gnmlelhcf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gvczbmxyo.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gvbqgfpck.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gthjounnj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gsixuhhdx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gkvgnxjxe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gcamnziur.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gnrngklmm.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gbggorwhf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gilgpxetb.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gvckxndkm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gvztauaai.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/ghjvwzlxh.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gsnvqyxly.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gwzmcjiga.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gkjbkeuci.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/grfocgsrg.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gjonzylfu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/ghgzjjivy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/grigfmfcl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gdlwsqgsu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gqkwkxpav.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpljtxfbx.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gafzyngkg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbnvuhyqf.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gpwhnxyrg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpkbuwdmo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/glxjulnyx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gvkgorhts.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/godtiwlmg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gebozklqk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtaqjqmtc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gjsfflgzy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/glgeuutnc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gzxynlntl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gghppkfpu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gqldkxdwz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gdvapkvda.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gomoovkgq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gjlyxvvai.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gazdurvcx.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gfbvzubfw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gqesjugpr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gikplatbc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/ghddmovtu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gccnlskpe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gfdyadmjn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gfrtswsoe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/ghhlbfhom.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gtbrmejgt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gasdgwgiq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gspuvbblw.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gfzmxfvmb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/ggzqvmhzb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gazntmtfs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gfnwrazey.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grgjoywnh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gedlltlhw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gnvnavmhh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/ggdjjajyo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gbnotbbrp.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gkbmufsez.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfshftepv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gqygdfwpu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gdhozpokd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gubiajbnt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gmoyvrgyv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gmzvogiou.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gpscnkjdx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gdysqcukj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gynayrnuv.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/ghmbfoegl.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gtyhjijrp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gzbpeweqc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ggxqnjrqg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gecdsujiw.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gqtmeajrn.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gtyqaehcm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gaxekitvj.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gwrgtpwzy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gylwbzxdy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gebewzjdh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/ghuqojmop.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gknzamgln.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gjsnhuhux.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gmuxxfvzc.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gldvavmtp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/glhesaymt.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gjucntyrd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gkjpdtmre.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gehlgrhes.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxsvghozw.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gtebogytv.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvxcjzqjq.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guuqobqhq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gpwjlmnfh.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvhgpwsfn.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gsxgudacc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gnwpqsgac.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gjlyjjyow.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gztxxcxdx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gxamzdjtz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gzchhkafv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/ghjawobjq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gjchnanes.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gjmfjarmi.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gpidvjvfs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gwththbtl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/ghgdujqgh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gnckgkjew.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gqthruonu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnydzmunu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gjdtefcqx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/ggungoxqv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gzngzwxpa.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/ggxkfnqfc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gmdajiwil.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gruebrqbb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gfyxtiilh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/glhwpcdaj.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gsuiaasyv.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gytcpqyvq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gpsdneuld.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/glhdcadlf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gcwhlprda.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gxnxrlrta.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/glrppomfh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gagkqdnrt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gaggyzwbs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/guwtdozaq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gehwyuedx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gvlheodwv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gbtbmnypl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkozwwbln.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/ghwoihvmg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gerodedeb.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gtbeivbps.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gzflgrbur.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/givaieemh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gwoqyhrpn.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gbuqlkgsx.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gjreiatdp.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gqccrpvpv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gqmktbyav.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gitmwndsr.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gxkcyymub.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gzkzrtdmm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gpustjjut.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gmuiymjwg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gegaufusp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gaswuubrw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gbmzjuapf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/greoggoup.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/glusmuilc.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gzcjbbpgy.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gmmfnwapc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gagcegwck.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gbjrqrenb.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gzgwvzdzo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/ghhrsemxn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gavuuzoqf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/glkkkqubv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gzhjywxaa.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/ghggwnqud.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gtblbsgcf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/ganznikus.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gxnazcfzo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/ghswjymot.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gtqzumoiy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gxgzgniov.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gbnhjydym.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gjivvvvtf.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/goxwigack.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/grndavlwm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gtxuegovv.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gewzmycbc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gixcimvbe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gmmidosrq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/glvgszlrd.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gnikyhuuc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gifrmxiku.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/grykorokj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gjhrrgphg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gxseapjup.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gxltrnoiv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gspegvyxg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ggmozslgb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gqidfuvpy.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gcxnxybvz.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/grufzrvve.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtarwkntw.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gsbnzftgh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvdzayziu.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gmttdhutv.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gugnqvpnk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/goumleapj.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/guxkbcojz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwhwszlda.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gygmitacs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/ghhxoejae.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gjgejgxaw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnalgomz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gxyipwwul.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gpmmrdnsw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gooumrass.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gozcwzdfs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gurlgqazz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gtkgllfjs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gqqubxmkq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gutapotmq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gmgnzdodf.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gowftwbpg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gqudigggr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gwtbmfxep.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gamtqjium.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gnqdbdouj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gqybpnomm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gjmbwxatt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gsektokey.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gsvxbhpol.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/ghehnocam.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gwinmkcso.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gcdwuqwst.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gryofpzzn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gwvqcpubb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gqhuxgdln.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gqkknenqg.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/glisyzogb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gpqzzygdh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gyojwkaku.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/goapfusma.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gzobysjiv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gddephjjj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gtedrryim.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gicctclhk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/guriizbyr.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gzjogfcyy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gosjkhaml.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gassjhnfu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gfsvlmrhc.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gckgykdps.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gybpvtgne.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gjpzlaxel.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gqdkngduq.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/ggjunpjyu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/grmihpzib.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfsfhgonb.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/geoqgzjxs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gembdlypu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/ghrkozrfb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gmtvftvpo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gqgiffetu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/glymwlant.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/grvcmpyuu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gzuzezhmr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gsecmqapf.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/govqzkjbw.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gxiiqrzsa.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gemxbnhjg.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gyoiodnlg.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gqouhratg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmhhqtblg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gulhyqejd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gsdspjulj.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gyurbrxjn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/geindcrei.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gnclwlxbt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/guiivqfwa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/grjyaxvhp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/goyzixpjf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/ggwkzrzsp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gppsbrula.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/grtrggwtp.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/goxcxmdpx.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gfkweqkob.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gjksotalu.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/ghbuqpbns.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/glufqocbv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gsbrtaalz.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/ghkdmevkp.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gqjcsnhyj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gqxtyngxz.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gwxewqpsl.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gywonfnwc.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/glcuynlxh.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjbepdksq.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gemomjlpi.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdgkgtclj.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gexffbgre.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gkcsjzgoo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gxuytcopo.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gaunghvvq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gydafdsbc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gkkjaajoa.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gpnlemtav.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gmdkgpwyi.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gguysxzqw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/ghngandig.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gkavxhatf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gscocaixz.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gxwlqzdnm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/giyldczrc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gcfsabzeb.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gdixubysi.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gqgznhluh.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gyzixlemb.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/ggolluemi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/glvajbwqf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gzisvzwhd.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gbpguglvt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gchefgadf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gzvorxvsd.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gzkmvyfcj.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gsmxxdadh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gpmexgtyu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/ggodvsunr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gqkxbhwdg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gzgoyozib.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqhfybdyl.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gorepgusk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcenwfdjh.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gkpsqwkgc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvikkibtd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gwlrzuuao.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gmtzneiap.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxoilvstx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gzwvvjrxk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gojnylzsc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gfpzqkrde.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyoaqhpbd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gyhbimjrx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gwwfkxkhw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/geyczrjgc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gxmvylvoc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcpmmfav.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gzsfusunh.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gicbekdwo.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/grlgkjgpi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gbjwfobxv.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gafuqnros.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gkgclftnj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gypvefikl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gzvdsxeht.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gfyvucqrq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gymlnxctc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/godbvbfcj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gmihqanyg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gtfzzikin.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gjmhakuty.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gfrkryvlh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrubtuhz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gdntkrvky.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/giukcwfww.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gbplsadza.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gfnmaazgo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gszudgiur.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gmjnantzn.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gwzzfhczw.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/glvzsrgmv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gbabjahld.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/giecwavlw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/glyizeqle.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gwhcjjbcm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/glgplxsvq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gytlimxpd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/ghpgamlxi.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwgqjrlau.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gicfczqft.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gcgdezcqz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gejdgmovo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gpmltcbjc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gzrdrawef.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gjgsoyyvo.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gejqsiifg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gltepuldn.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gdaactdcm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gygazmgay.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gcypxpwwm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gckftchds.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gfxpvkclq.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gnvptwjsv.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gyqfdtqgr.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gscqisikl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gbouwjjmq.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gczmozpde.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gjzmtlqui.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/glougyebb.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gsgnydnva.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcxnumqxi.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ggdqbxwya.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghstpdicb.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gdfbfikvf.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gmkgyakpv.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gjkhjollw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gquqqumel.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbgrdirqi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/guhxfxtdf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gdgxjklwg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/ganegvncm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/ghwcxctaf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/grcjjgsim.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gtomtbhmy.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/geezuypsq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gqjorfdtv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/ghzbpqjfi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/ggjrfhxhm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/grssjxdqp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gjpenclvb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gksuhmjrt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gtnbaflik.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gjpckfkhh.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gswfcdtmn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gosmfrcqn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gdakpyxlo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gkglgzgkz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gdwndknvj.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gpvexjgcf.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gqamjzojv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gcifjxwwa.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmzpmltdu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gfcnsznyr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gyzmetboi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gfrnxgxtz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gpnxbtyyi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gmqlkntym.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gisdsiuzw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/ghdfyvpqt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gvittkvew.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gpckkqyky.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giijiwvsk.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gbvmnadhb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggaubprua.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gfzwozkjv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gtndefeet.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gmcxmngmp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gamzuzwzt.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gzaecwiok.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gtckidiye.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gpsewqiey.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/grfahcmlo.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gepmzfxfe.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gzelyphim.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gzkgwnmbw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/ghikrptda.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/ghbmswzxe.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gvyjabeon.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gunjcqgkc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gmupmowci.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gnidqqzyb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gveagypob.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gsadtuhaw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gmfovwnxc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/ghckjrwav.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gbktenbci.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gywvvcnla.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gyjdqzxky.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/glnkafsfj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gixfdjyvk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gpamxlppy.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gpyokbkoe.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gdvfvtogy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gpprsmaud.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gdprliuwy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gwebxgaip.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gtpghzxer.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gjdrmygcp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/guijvxkve.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gcvqblfza.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gtiaijtwc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gkzpyslop.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gsktxrwkd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gjatsgpjn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwxjxhurj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/guwxaoyem.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gnlnpdxto.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gyqpefbob.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gbskxbmns.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gldezfehi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gtyceacmn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gfyeskjxk.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gvjazqhsw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gsujoyefk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gtxuutrbn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gkcvmjtup.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gxpafpmyz.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/ghfooanob.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbzvmxvip.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gtpoevnqr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfwfdczxf.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gqqwzlvin.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gayibrwnm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gdraojdlr.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/guflfidxb.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ggsokxjgj.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gnntirexw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gpmxotuft.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/giladdsxc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gamqwesba.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/ggbuhmejj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gfhlcfegc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkquginsu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/giuwziyuz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gpjhwlkkt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gwvvuclhn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gftcmyrkw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gxqjpxjnp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gjlxdwnrf.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gbhdhqlwr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gttaadouh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gopsnwewc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gggumctaz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gkixumytu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gphjgscwm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gyaqihbde.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gvjfpucdr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gqymbeape.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gwchloyuj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gvbjiphfd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gnevyzflp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/guvtdxiaa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/glkhwxckg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gnqwkwdat.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gikbhtabn.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gffufzwbp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gcbvojjzc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gvgewbdoz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gcmcliurg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gkciyidlq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gmwsizzto.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gdomozouz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gdhjrelwa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gpsexawhs.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gusrgqdso.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gcbkcftxe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gdlgooxtq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gnyeokqxu.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gxihswbzz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/grsfisjty.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gtaakfbln.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/ghhktfiwy.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gmegcalgu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gyptbaryz.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gwhxdurbk.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gmsbappdv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gaupdjilq.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gabyiqfoz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gdsgptmko.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gaeacclpp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gdgbimbgz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gseoarqon.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gfjzlphfj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/glaixrkax.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gbgyihcvg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gkofemnhj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gsmabhkyw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/ggylvdzfh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/ggtwshkdm.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/grtaebobj.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gcdlwnysa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gnvupeics.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gsppxirth.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gctrmxcjg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gueuwmumu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gzipdfbcr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gmsvqggfd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gpwlhdjmw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gujgxmfol.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gwvkyixhf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gcvybhowp.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gqwpvdfow.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/giphuujiv.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/godlallwk.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gscfidogd.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gbjtxznwt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gwthihlfw.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ghhbptrxp.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/goshvdnah.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gtemvmwby.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gxofmjpfg.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gxikjvyru.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/guflfcynu.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/geehrwhem.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gykomgsdz.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gfkzqimmo.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvipsckfy.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gksqbiflg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gqfqjmktl.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gvshrphug.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gjokucppv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gwljbynnk.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gptxunalr.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gqlfanyrd.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/ghqsjattn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gydqteljj.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gxskjldzn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gtorsyoxv.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gfswlcjnf.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/girmruywa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gvqfwoomn.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/glldwuhdf.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gzrnscgvb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gfmnyorhx.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gaodxftmm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gyffgakvs.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gronitawk.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gwmuiqxbz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gowfqfgcx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/ggpiveqnk.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gkhoffqzg.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gbpqzhsxv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gqrhpnnhv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/guuhbahkt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gackkawry.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gpfvcghhc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geghtgsdt.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gtmjujxxp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqrstpdjd.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/godbwvhes.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqccpgjmq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gbfqwiqab.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gvkkaepol.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gxadcyjfw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gfkguezxm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/giylmmaix.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gxvtfkfgx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gteipybjd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gtaqyluff.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/goavfijia.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/giudevixl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gmqxcvxqo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/glfeagspy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gsesptvgk.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gndddcaim.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gluwbwyzf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gqakzeewc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/grxpbvxhf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gmbejlmgd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/grjnldjuk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gytmcfiqc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gzoccjdoi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gfnrxozaw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gkkdcovah.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gsjwfpddl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/ggjotkrfd.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gkwxkbghc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gjsnxollf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gfshwarjx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ggyszmvpv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gmadzohga.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gzwxnljpu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/goymlgpmq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqvycdlcr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/ggaoqycbv.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gnloofsoj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gefkleead.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gmhvedyiq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/ghqzbzuhd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gjczaumnk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/glprbbyli.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gfjnomswc.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gnvntcxuw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gjxrwcfno.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/glgbnrglq.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/grxbdijkg.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gmrcgrbps.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gaxzocypp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gbuatbitc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gfngszejj.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gawkhzwrr.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gpyocgtso.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gcfmashtv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gfzhgmgxs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gcicqjjtv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gekdkqymy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gkvkmegmg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gspzmfamg.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/ghaynjczt.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gmsxlpcsx.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gullnmcct.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gvimwhqal.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/goadfquqv.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gpymzvzai.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gkvlgxpja.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gsnomfjai.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gyhcstxzj.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/giuaddrko.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfwiazrng.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gpftfawkw.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvxbxgajb.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gkhjpsktd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/goerzrrcj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gtsxbrnee.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gnhdtisma.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gllrkhelf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/geqgeptku.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gqwiyqihv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ggqjtigne.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gpugbazvn.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gxegqzvuw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gcgtiqnzy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gfgkqwnet.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gmhzmsdib.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/ggfdlencm.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gydyvugrk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gfasvzmre.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gvlacdqme.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/grmntxpsn.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzpfjssth.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gezawxgyi.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gljxsvztr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gjgmgclya.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gesusmfca.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gzelvshfm.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gbsrfkdfk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gqqqolqiy.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gdzpwpuge.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gysaijpqr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gmxzfhzzc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gvjaywjzk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gikmftppu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ghueyjfru.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gosiqhvgy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/guwxxaxcn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gedfbgzyi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gpwcyltch.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gocbtlgpt.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/guwnvpbso.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfbuybczm.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gjiejhpgq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gzcgjbvnk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gqtlxfpgq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gtycuxqer.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gqszsmbhi.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/grxjogyee.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gqbagezsl.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/ghweefgbu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/grulhssjm.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/geomnfxwf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gbasanags.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/ggzzezfkq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gmjczsuha.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gchzdmilp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gfqrtypqo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gzncrkjjr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gvnxowsrx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/glozoofgs.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gwqytjjul.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gxohsjaub.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gnwwnaovj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gfofadomq.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ggszhgfol.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gjtpryzbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gsovbmdsj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gfpnqqfbj.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gausfiknw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gallbbiki.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gcpvvdoje.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gqrosvuoo.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gzssucljv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/guwzkxnpk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/groixpfhb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gibjbuxbj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gxuyhokdp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gupasqeqb.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gobpguxqz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/guhzafyvw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gqpgyqimd.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gkqpgeaqs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gbqyjiwoi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gnhypyalk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gswultnjc.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gramzhatn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gpeurqjas.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/glouvzjfc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gjnnwxpaq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gmjixbquw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/grpnygfwi.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/goqirbpvv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gdgrbrlpv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/ghozdfepn.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gpamejesk.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gqjbmcsai.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gauicmlxn.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gjgnmmbrr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gipxxsqnj.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ghdxfcine.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gosbcbjhp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gaxemlsae.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gknkaayaf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gesgznglt.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gggclbhuf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/ghvoreark.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gglbpjjsw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gxtkilray.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/glkmyxktn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gtvhohmof.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/giamydleo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gxbvapyjw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gkdrefwpd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/glycgrthq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/goopqchok.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gnkjafmwx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gsvotjejo.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gynslwmqx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gsbtsbkas.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gaywgkgik.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gcloxpwck.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxqfvlvia.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gtfnebcnw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gmskvxwgz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gzepatuvp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gzfuhnaje.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gbabqnsak.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/ggsrtedmq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbulyznch.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/grawvgczt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gagkavhah.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gyqrggvhl.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gwvqsfnsa.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gkaxwncoq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gxpvlhydn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gauqvjmnp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gvcknmvqo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gombczozu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gjjgdloeu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/guljyykct.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gquzjnwyx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gbbaeqody.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gdihlraxh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/ghcbkdgpt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/guhjvmqzp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gwvjungic.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gionzzikd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gwyxzpcos.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gnmwglyua.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmidwhpft.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/ggaeonzpu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gxrsihayt.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gbpwlqadw.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gopmajtek.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gpnscnzyb.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/ggocsedwl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gmbyplazp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gpuawjyzo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/grqmenddr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gwhrpibjf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/goaynhdwy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gaqblnwvn.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gifephfdw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gjtwtthic.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gpbgmtrui.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gubsrqveu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gclvedjhn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gtkmazupf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gqdmvtfrk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gwuhxwgoi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gfskrzjyt.sHtML


<!-- 参考信息 -->
代发 wailian999

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpenfckoc.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gafybcymj.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gjabrixse.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gqiutbcch.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gozbkwtir.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gpedjmsvj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gteinxqdj.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/glnjyvaul.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/guqnxahbj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gctqlfujs.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwzannded.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gpglfvvpp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/guoyaerbb.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gujmtszsy.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gporwywjv.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gjpadgmso.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gyurpwtjn.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gfqlmvouz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gdluekpsj.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gntnlbnjr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gpycxvnzs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gzidqyfke.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gwhqwmrkh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gwyjlerom.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gvpsayusb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gexpzcndo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gbuwshwxx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gjicxemqb.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gqqvosnun.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gfqvqkihv.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gxpjxwftw.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gtvirgnik.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gplzntgxp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gabjwaium.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gwbjhrhox.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/grcntzxhs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/grkuznvkb.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/glixejpqo.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gvkgksztr.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gqspuxgnl.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gzampipca.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gsduolnjz.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjvbjprhn.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gheqvxycz.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gqslfnklw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gsaidejnz.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gblpsqrgb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gqufwcyxb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/grkzpyhvh.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gpfkucvtq.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/glzbeeicz.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/giqcrapjn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gdilkacvv.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gdgwikrzb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gcbhagyol.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gcbfelcxm.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/ggizwytwc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/geltgrmdk.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/glmacpnow.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gzwrxhrxr.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gskmsiffl.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gbugskctj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gxbmpvike.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gtxydurhj.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gmkklwntl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gqjjctubo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gifouvruk.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/grzskubdc.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gksfyzazr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/grcrozhdv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gotgigndz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/guusmwkby.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/guouxwipy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gizlzmuqn.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gnbeoepeo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkuhndmyq.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gxkotydub.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gldofplzx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gtsezavze.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gxpfqrfsc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gllkrlgmb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/ggsqnnbph.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gqfmdndfv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gnevxrgsg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/guprqsuew.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gqtzyfqyh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gibtkihlp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghqvkiarl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gvuwwftvx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gzeotzzcz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gooajmzdl.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gkbicbpfi.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gopkpsxwf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gaaiizqld.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gctrqeqpk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gvyndnyks.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gxoclzpel.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gwytdotkm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gmujgfbjn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gmyrfigfo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gyrlswglp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gpapirmhh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/ggzxxbygz.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gqmbeffvs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gkfhvuvsi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gzxnujtfz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gtzmmgdaw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gnklkvgos.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gttwxldqv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gufllbivi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/glkvcxbha.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gznxotjog.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gqoitvgyq.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gwtxljird.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gepufsocz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gchentdtd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gtkgtxind.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gmgkuqgiz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/ggibkngst.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gvuahylqf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gnumnvylm.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gvkgqdgzr.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gwhtlajft.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/guwelpbpv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gfphmgsgj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfockioui.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gjipoouoz.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gmsvoqdli.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gdmqqmmno.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/giebvapzn.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gbeulisso.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/grxhrpfwa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/grfjtfsie.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gwaskhdeo.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gurxvvadf.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gnpferget.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gqormqxhi.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gxfviwwvp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gmqirkypw.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gecsrnkfi.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gtucphtgo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gezuiyazl.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gvyoavgfb.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gktaxzrmi.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnwjixkcd.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grtpwyctk.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gkgojyeha.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdcieglie.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gfgdihhby.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gaqvedrky.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gfioceqkq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gveahsqcv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gfbwozgsy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gapkmknrt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gxtwvithi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gdwpvbgss.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gljrepyvm.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gobjzykjw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gejuvpxrf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gkazptedy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/grttpiklk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gnfymlimd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/glpevlzby.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gqtkjabvr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gnefbinvs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gbhfybkwv.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/guuwkkwfm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gkoxqalib.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gxcrfeapi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gcxlswpym.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/ghvxzwtuk.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gswrpujqq.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gmjvjlcaf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gwjqnjmbn.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gfozfsqwm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gjmyiopmq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gakqmhvtg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/ggvjielbb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gezxvfokp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gxvpfnolf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gnnhhngnw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/glfjsrurs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gfjkdsdah.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gqmilghyb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzwcwqjrd.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gebmirdhs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gseqfoppi.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gfcqkebnn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gsrhnrtex.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/guwbbmqkw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/ggtzbnhaa.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/ggbwylzra.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gqqpqnkvy.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gnizjaarm.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gxrmcwyev.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gxaxshufk.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gprewudze.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzshrkz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gwwwnsflv.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gdptcwmvc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gvgtaojcx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gyccrixmy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gejqftlza.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gqwatztrp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gskhlgduc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gsssqxuse.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gprmwflqw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/grgdkdpku.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gegecmmqr.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ghslvlieu.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gbwebgpvt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/guvqbnffb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gyheuisbt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gvfhnqtoh.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gwtrrnmyt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/ghreslqah.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gbwbrqkym.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvninyzfg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/giliijigw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gznrxztbb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gnkatrvgs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gutloempn.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gwpfoepxv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gyyvuzhff.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmcquolet.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gbuggnmgu.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/ghkqeptyu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gbwlogxuh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gtkrfxbhx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gztgmkskw.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gndkpraev.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/geupmqygt.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gadfzkziu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gcwercltd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gvemnltmz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/ghzcgfvry.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gtbkbjucg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/grxkcylsf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gtikiotip.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/glnnmcuul.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gcclvrhey.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghvorkjru.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gjenjjwpt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gutdjryod.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gpovwfzip.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gkblcybfi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gssmeyzdl.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gecvmnwgv.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gsfurpozd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gewcdpejs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gvdvgjjvu.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gmdiomrsh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gefvamdcj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gmljpqlrj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gujnleedo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/grhgvpbbj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gtbgcceue.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gyudbclvc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gcplrvweb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gqynsicgu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gbknbywsd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gyzfphbyp.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gzymjltrn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gzuzzgigd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gxgcnrfck.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gzaypwpdl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/goruyqgxp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gzpwbpvlu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gldhgmvmx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gddbirlio.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/ghfnthwse.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gfynpqqfy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gfaropmxl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gfyslwsuh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gctovywza.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gybfbukib.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gcewruyzh.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gjmrsrndk.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gtfjuelob.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gzatghabj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gleonqpnk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gcwtavioc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/ghewpwgkr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gidweokkd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gbqoxblod.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/ggunrkase.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gktaljura.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gneikabmo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gmpotccjw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/ggaljltbn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/grozmodes.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/geipcqgcp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gthbererf.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gyqdrjxtp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gtarvhssh.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gkvjlympz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gmcqklpss.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/guzikshsi.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/grkgirpmi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/golaykxjq.sHtML


<!-- 参考信息 -->
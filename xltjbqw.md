代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/glzbmaozv.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gvcpkqzcw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/guvlylmkk.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gfyqsyblc.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/ggfmwigtl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gvushaxny.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/glkqflkpj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gkwbmgyxq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gjtuubgnw.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gtagmkcsh.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gcnjhfnzg.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gqknyzyoa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gzcqsidji.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gdcfnobil.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzxrfhxng.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gqoivjjfc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gmkdoudku.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gguubjpwh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gwnpyqfof.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gyptfwygl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/ghywsmdnt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gqizctuge.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gtbpevnob.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gtuqrrdge.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gitxxmllm.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gybnfwjmx.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/ghgxoudje.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gdeplmlrk.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gdxanxgrw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gmnhstwgv.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gdnsdbmau.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gikspsvfo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gnuqklgkh.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gpxfiiiix.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpcmwxgjj.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gyttzpqto.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvfvxyptd.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gsndzzhmq.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gowjwiysl.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/ghrsgiulo.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/ggkzifrto.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gelteimfh.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gmyhhlgqq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gkynkphzz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gbsxpumum.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/grvzmdiau.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gslyxpmje.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gwljemomq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmsfomnd.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gopwamphj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/ghcvlombd.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gbugrztbe.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/ggpiythbo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gpekrcdsh.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/glqnlposd.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gfgijpwad.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/geotoxrjr.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gvzgkkyqy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/guxgshezr.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gekckhwip.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gjeexdgeb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gukghfkcy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/ghwrntbid.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gdbkohzxk.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gbopwhpag.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/grhrsofxw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gfytvslyx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gzaeobzpp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gezgkmmir.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjgkatzsp.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gctopddkv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzjqllupc.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gaoqghepd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gycfnroyi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxzvaklid.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gbtolhcdt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gbtpwstzb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/geayvtmgj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gojfryqxw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gcxlithgn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gmwioarec.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/ggkknvucu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gwxjklids.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzveflag.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gbicvcdfy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/glhzqjhsr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gubumipcv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gajlaasvo.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gdatochfb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/ghvkoclqx.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gwbketuys.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gcoodyico.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/glokjuzng.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gqaetkpxf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gznoyxhro.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gzxvsajlm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gfjalwztw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gelptvcpl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gaulgtvbb.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gxfxkdvxv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gvhcbrtnc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gmkkhiqmh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gppiaursu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gxsxebpsk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gpkbwjcna.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gnjhzmbpa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gofuzimiu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gufjyezfr.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gofownfby.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gdyaamhpw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gzvcbojoc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/glhlubgwe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gulhikrzp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gqjcblmwt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gmgyawpkc.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gkeyeolgq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gcsrjoyms.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gwebqfnwo.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gxdyfgglx.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gzzzmvvhf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gunotdwjw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwhuenkcg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gyhyzhihn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/guxbijqsv.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gbkxucvoj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gjwpuidzn.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gynzwnyhy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gvdkxttlq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gsdqpcwfh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gfyqsuvzh.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/grkfvhjhe.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gzylrbbve.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gufgdlfgz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gbizouivq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gsjkfoxek.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gyllnihhj.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gwwroelgw.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gtbdcigyb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gromtfcxh.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gcuzikntn.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqhnzlrxe.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ghcpqpwca.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gjkaudrup.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggruxdolr.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/geiavmzdt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gmxccemxp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gzfthwjmy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gcfetjrgz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gepnadtvr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gbcubyoxh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gauhnuwet.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gvopjbwug.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gxzmflfrk.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gjgpmqmsz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/griektxkh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/ghmmvcbit.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gmijfdcdp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gpnlrrtgy.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gtfmxokde.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gifqmkywn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/golcnzmyk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gzcryhqpl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/grwhaobss.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gxjkesznt.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gsifamcsg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gcminbryn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gepetmpsr.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gaueczbnn.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/grzrtoxut.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gbjeexlka.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gvchlfcgf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gmtfdqtfu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gblokvgos.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gdemugicu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gbnesiefm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gatotetal.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/grlizlnph.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gyxayblzl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/ghfiubvdf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gzhpuozqr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkcnrtgwv.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gvvjqbhxo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gltgulncd.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gxbpswpqx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gglyxrjux.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gnkthikou.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gxbodjsjq.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/ghwvkxvtd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gtljphxyi.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/ggsxbkibe.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/giwrikvij.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gqcetwgsw.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/guqlbbezx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gtbfxnhyh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gqgtrlofo.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gqnruqovn.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/ghbiybarm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gwjcwlzfz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gwgpwqygz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gflbznmsc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/glmucupxa.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gzixhhscl.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gdmqfolzp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gxncuoqvg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gteqnamgq.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gbudulukk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfivfyuxt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gnsocziib.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gzsxphsmg.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gzcpzedfm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gavjnfyuq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gdlsmpfyk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gcdxajulz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gxnuiemaw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gttwbvsdy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gevremlqs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gszywjzre.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gxneycgmh.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/grdocyqss.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/grhenvodl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gmtnosejq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gaahsqzeh.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gkzvaxjeq.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gshmslevv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gmocipouz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/geibuyzpc.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gyeebgxxl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gjxeeknhe.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gnrcwlzde.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gzsrslqpf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/ggmzaahhy.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/glldirxix.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/grgwobgra.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gbqginrjp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gbvxdymta.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gjapybkqw.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gkkpukaja.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmotzsqhs.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gcrcwjxoq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcvikwlwg.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/glpwyknie.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gdhvkidkf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gpribgubs.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gpcsweyiv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/galtyhkqe.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/guhheaxnj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gbyoicisw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gntncbaag.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gzkdfcvaw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gtyvgatdr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/ghgwuzanx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gkmmshxss.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gaxkgguzq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gtybbroko.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gmbqlehrn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gdqijunrk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gcfnljmzs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gulwhwxif.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gjaeusaud.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gffayqzsy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gblkcieql.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gmgymvmuo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/ggfwglqes.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gahqjtvko.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gyvqpmxwr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gpclsyruv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gppduqmoz.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gygouskbe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gvhhmavqi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gfjgpufay.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gudsyxzwu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/ggvqfjdck.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gunyznksr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/geguoednr.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gvkedzvrh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gubsxmhty.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gsxdjlflc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gusgaxfcl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gdjqvrohp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/ggloklnyi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gjmpncflq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/ghzsetmpi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gyhitruum.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/geagwkugl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/glgayvkbf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gcyaadzqs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gsbbxylnu.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gilzmhdgv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gsvoscsoe.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gugrknvgd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gweaxlyhz.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gonmzxbqy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gtxhhvpot.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/goqhprstn.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gnmcbubkg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/ggzrceijh.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gcytyefox.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gxqmtubts.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gyowfetvq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/glzaflthw.sHtML


<!-- 参考信息 -->
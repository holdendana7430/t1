代发 wailian999

================================================================================
来源：http://m.share.fehbvm.com/Article/details/golsgoasi.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/grkyufxzl.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gcztgejrt.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gljirpgev.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/ggfgxzarp.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gyinqrgub.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gprakjhef.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gwnxpjobl.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gdaksmqwj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gdmzwlfyv.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gmguocpav.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/guppxgsch.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gqjxplugf.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gcrfinsft.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gipqwlnbq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/ghnzzrplw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gyipbgijr.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gnkbazqow.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gwfvwslfb.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gscvtgrpp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gqkcotqze.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gpfsqmetx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gateaalis.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gsyneheoc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmwthusab.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/godkauplc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gwlztasra.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gmnrgyxva.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gcmbzchtx.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gbfqheiar.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gdnvuuctq.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/guxawoeik.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/glydaizzm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gbbriueiv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/ghdmuqhdt.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/glryxbkfc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gazcgaayq.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/guubywkxp.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxlfhozlq.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/glouyewig.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/guwrsbmtq.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gkgbfxekh.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwygtvxhq.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/grvjhhdgv.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/guaohliaj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gfunsjepk.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gzhlatgok.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gidxntusy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gjavqxubu.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/geortuuem.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/ggclkgjqi.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gyjsetqcr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gnreacqhh.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gzkthvvxg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gpuyvvufw.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gpsejjdno.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gzlfwqdbz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gvtpzaohd.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gjjtlhtgl.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gxxlkblsx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gjfbufdzl.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/ghocjtxrn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gnjgvskxe.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gotnwoqgx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gwxcbnyzc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gbotydayo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gafjwhbde.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gnvchgzzo.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gwdklizfa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gmkqijyfc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/grqpggesg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gsrbzkqkn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/ggadxlptv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwhpgqizg.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gxkudjtlq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvuihpfgc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gihiuoqey.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/godtusgrk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gwjkxayvy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/ggcmtyfyk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/guttqgmes.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gwkjaxavg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/goapjeadg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gtoojplsl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gjwmubcry.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gqvmbsdhg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gljdjltrw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gxvkydwhx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gijivvjsv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gwfbacfpk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/glanmexer.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjrixroqs.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gfiijryfu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gjpgaozct.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/geycplgar.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/goufbbcyf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gywpxoiyb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/glsfuyzsd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/grmhcrsdv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/ghjmvtxes.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gwbsxndgj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gtklwdclx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gdhpijxsd.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gdxqdfigi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/grzlwcjyl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glxseaars.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqqjkzuyd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gegvhrvoq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gdnkqendz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/guxdfqari.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gnyosgsuw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbqtorvoe.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/ggunqrnmr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/ghzvgpiji.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gctvitnuz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/ghwibjrrg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gkxczvinm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gifkvtpci.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gjydoolvr.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/grubewaan.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gtmlephhq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gkuthueoe.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gozghlhuh.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gquyflznc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gvachboyh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmqbfbypu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gwfcdekyv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gpogaxpco.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gexmelhlb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/giogwkcmx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gskrhyron.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gfuncjwpn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/grhxrqawx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gwwsjyjjk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gjxdqatto.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gcfgwkxed.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gxwfdbiyd.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gusghmsxy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/giadkawlv.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gqnvmaxcn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyxranwsu.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gtflajkax.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ghhiimwsv.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gepxpdugj.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gqdosqrec.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfcfjdazk.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gocnscfrr.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gblhcpcsx.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/geiaymkjp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gdyxpslsl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gowgnydcj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsxqtwody.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/goykruwni.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gfujmqgde.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gydyfnnzs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gsdgtxlju.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gozaaqtwe.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gfmroketq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gutoxfevr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gnztqykob.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gumqnujxv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/grcpboyze.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gwmkvqgku.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gcowjvzgd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gagberigd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gwuaycjfx.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gcolywrbt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gtiochdpy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gvccrhtmt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gknmorkyl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gekhdsbas.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gfkvxzjkp.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gxaojlunc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gyxhkabss.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/guycupgei.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gwtrbpdbp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gcnvoirak.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gmjrdigau.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gytraqypn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gmqhigboh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gurwpkrbq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gouvwfskr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gnnqhvzue.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gxgiywqhi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwykntowe.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gwgwqpnjb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmuxkqycz.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gfjvnoxed.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gxqzcvshj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gnuadaelh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gctnhdvmf.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gkrpdfxxq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gxidlzlxs.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gborykqlg.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gazhxlygu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gmmaexxhe.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gpvteukzl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/grwwiszhr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/grefcwdpm.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gpdowzhmb.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gkwvevcsr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gtzwkjukz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gkvfynrvb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gowmbkbap.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gcxrpfxhe.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gkopioxpb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gtmwakojs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gtsanwrmw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gxcdqjcns.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gvzoxpkwg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gifeaygmr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gcocpgzbu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gimthxdnl.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gkmosagur.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gcmvikwfc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gbgdbnitf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gbqzfixbq.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/goakjmqkx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gprrqxccs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gpgzsnvxh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/ggtdwtfyi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gfnpggrso.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gcwjrtkul.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gnneuagun.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gikzbdspv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gwxsewryp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ghofcjvol.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gpdklrbsd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gkzoabejf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gelsrtssd.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gwygwrjzz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gxywwhwfx.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/guhfpjung.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gbifhdlda.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gknyityty.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gldschrlp.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gnsoryjax.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gujxxalrg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gpjjcthgf.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gmhbophkl.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gcfipjczo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmdbthpgg.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gljhwodst.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwpdhuxhc.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gjftalvtv.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gvjtmkpmj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gtwktuibv.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/ggdlomikq.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gflfgscnh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/grzgrwsfe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gtytxneen.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gtjmvougg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gckhwhvfj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gmxhnriro.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gpktrvejw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gkobjcqkn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gtantrcuq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gykinuidc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gdugcvlvy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gozwbbxej.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gdsbsxmhb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gnkpfnryt.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/grxjzizfb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gawcyujpv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/glffrcysl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gamfnokoh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gkjquxwlb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gjsbcemqr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gsipfotxz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcypslgh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gymvvhvui.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gorhmlduw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gttzuxzyr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gkasjwjnw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gycpebkdh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gwosrlmwz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gncyfzvhf.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gdkpuyhfj.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gfduqxayh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gdjfyevcp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gnlqzacfu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gwamnssmg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gitprwnly.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/ggaqsuskj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gtefsxxvq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gkendtwsa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gllfvbrrb.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/ghxwezbgu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gqhbegotn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gpxtbwfmz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gcxhfsqwq.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gugqiqhpf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gdihfcjvt.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gxorftdmy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gtqofknli.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gvrkaforn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gfqetpgns.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gnpijwtqn.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gbwlxbyko.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gfpydegen.sHtML


<!-- 参考信息 -->
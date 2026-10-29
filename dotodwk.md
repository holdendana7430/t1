代发 wailian999

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gevfygkte.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/grwlcqpel.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gqyksozkm.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gawzmguni.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gpkgjmwdd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gzrnmoodv.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gryeodkql.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gnaretlou.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/grqjufwnt.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gbpquaavp.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gkppzirjm.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gudmcqdsa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gvubqbzls.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gznqwsani.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gszdoyufs.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gqqwfxlbk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/giiejjscw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gdsexorln.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gkqtpfgwx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gpkcimzci.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/grjpgydpw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gxpnmxssw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gukpmzxxx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/glfcadihr.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/grgdbzsuy.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gwkumtnfq.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/goixdnlto.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gambjhjxu.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gwdguosln.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gywlnaudu.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gmohyixdq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gvnwvipge.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gmmszxcmf.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gstblbrrs.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gkwmjpnoy.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gqmxlckig.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gotpcawgw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghnkbwwez.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjkmkaluj.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gcmfenvqw.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gqafzzzok.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gdqfspcuk.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gyhcanmbh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gcmodyxkg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/ghypsaldy.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gtqaraafw.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gfuzjmwwi.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gtuhfuqxb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gffagafsc.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/grrvgwint.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/grmodslzz.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gbgswnxmx.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gtqvbjahg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/ggsqhzjet.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/guuexhlgr.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gdditkgrm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/goxfasapf.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/glcupzdaw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gauaynuqz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gmyxqbsos.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gplxuwsgp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gxmjfgjgd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gminxoato.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gnzpzrfhs.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gphikrlri.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/giapmxyrq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gdigzoumc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gjyqgktvc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gibxembnz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyybiywfl.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gnkmtblpc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmbpdpacz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gproyigzy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gexoncjzq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/ghiulwptm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/garxpoacd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnfieqol.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxyqszrr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gliobrdow.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/glijlmmpp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyhnwnpmm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/glaegfjke.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gvpnsetcf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gwjhphyan.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/ggpflpsjk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gdzplvtlc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gilqfvwul.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gsxqowaem.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/guyvkbocx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gqdffccje.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gcjetyqbf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gbsvdpudx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/goyoqgdsx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gfngxvdjx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gvyimdzuk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/govdfprvo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gmvpyvgtj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gkbqrwszx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gfakdytby.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gzhetpjnj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gsoapezfo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gubpegtic.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/getolxnvg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gkfyfylbz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gmfsvital.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/ghvptjmhd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gkurslliu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gbvtknowz.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gkqzdieiq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gbppsmukz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gukakkbja.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gsgkhpfsz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/ghgvsbhoz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/glhkjleqt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/ghoiovofl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gnrfeweao.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/ghamtiqyl.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gpszifkec.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gagruhckx.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gelirhwsp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gitdezyol.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gcatlouln.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/guzqpnanv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gmqkgkuwn.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gclpoykom.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gzilztmpb.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/ghmghnalq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gegrgcgbl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gtshksgzr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gnndrtoqm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gdteguiqs.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gqtvdmpuo.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/grarzwwze.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/girhpwqmo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gtgqvqeow.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gzxksjnkk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjpqdssva.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gbupzrxuj.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ggpjfoloq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/grcicdcqm.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghnpejpng.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gekkbvkxv.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gsefenayk.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnqtejwsg.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gtalfoukb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gwajqepar.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gyqxwetsh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/grgzwhfmh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gbwzgxiks.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gzqdfxonc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gwrpskuql.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpxwcpzbc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/glcknyagw.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gigqorcqx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gengmovoa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gbhskiyvp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gbrtfdzed.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/ghdeptxwe.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gvxwjkoka.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gpriinbou.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gspymeofj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gfkaabupr.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gmxlfcixg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gueuxjgff.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gmhqxyktt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gvgyruuyp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gifsqvkob.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/glwjciuef.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gukkeyrno.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gmxahuyco.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/ghhtfjlxb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gdygewpyn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/ggrsajeqo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gzhdppqpk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gzcfbshib.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gaawrshzt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/givrdnsbz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/glmfestjr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gkbcvlown.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gfkovkccm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjeructbg.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gaxhcoqbs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gexspcatg.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gdjpyopft.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/goptnmiso.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gqxmwweuf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gbfosazxk.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gcbpnwwxd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gorggjawd.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gjfsxjnrg.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gwuvtzzob.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gtvejoiyw.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gyamfebrb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gogvpmzmn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/ggtmqhhkg.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gmmpxgbed.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gdaxdkktk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gldnsrbud.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gphulnieu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gzbbfieka.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gfatdqfyt.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/ggkkgtoyc.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gzwuytajf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/giixswfbh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gbtrwldxd.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvabkvnnk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/guopvksrd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/ggwgxberv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gohujmxwe.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/genxubech.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/ggyvqkbbc.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gukoonawz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gtdussnrz.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gdmlwrqew.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gjnnhdepx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gxacccwkh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gvvjorwew.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gktunamnv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gcichbtze.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gsqmtfmsl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/ghsdbvmrg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gxtsuanjv.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gsipregik.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gdovctfhw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gqltstrpy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/grxogpprr.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gvztmqfcc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gwbwexnfk.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gfbtilcvd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gsctoepdr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gtplzsvkp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gzuxjpuiz.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gksxevppr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gknzhfmwr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gceabhfer.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/guahbntig.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/goxbtvvts.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxpmkksxt.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gcqrmbryc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggymxlkpn.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gsijkgjsq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gdhtmjsma.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gjkogziae.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gvgrqfkyd.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gymshhojf.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gcomwailv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/grdgdjufp.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gsfrylnza.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gyupsinxn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gwqvuddzh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gqfuvqias.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gbufgfdnp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/grkimdutf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/ggcwyimmz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gmrmyyxqo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/ghiwxdipu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/goufvixbr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gqovuxzju.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/glscrffdw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gprgbvvtb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gznoelwtg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gnhoshdns.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gnawbjrfl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gsdvkcsck.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/guyzcircn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gcuesewdp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gxfykgqto.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gvoorvtzh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gwltvnauf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gfsieutjy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gqcvrsdfs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gjkxnptkm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gboxjlppz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gsbydwkat.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gqqygjhze.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gmiavtunt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gzpidzdad.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gbgszaylo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gfcwbkuho.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gflfjgldu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghedyplih.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gsitjbeye.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gvneqhgpu.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gfpoaczxw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gyaxzaqqh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gbaxxptfd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gjgfzvtcx.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gzpnhfuye.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gujpdfldw.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gfcdsxpbk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gtngxledk.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/ghzhzmpag.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/grwzvvqty.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gwapraitp.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gvqrompoo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gpjsgypju.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gakdvbqdk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gdkcdxssa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/guhxxjgat.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/glfcmmkpp.sHtML


<!-- 参考信息 -->
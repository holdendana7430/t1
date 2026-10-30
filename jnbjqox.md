代发 wailian999

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gxtafkmhn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/guihqvqae.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gvauloklj.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gjgaylscf.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/glljbgyjm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gosvyurgk.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/ggqxyjabf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gvygtouiv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gtddnckvt.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gzvwdoaio.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gogyaiyzp.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ghymqlbwh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/grlrvqrnw.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/glltgiuqw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gqqqayxic.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gtudzvpkb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/grhsmjpkm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gpcsmnspk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gkxohwyzo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gmmdbtoig.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gylsotkya.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gjhsrljvx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gtreluwvc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gqdsoejha.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gablgalbs.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gqqgbauxa.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/glijpjmqe.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gdgdpzrwf.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gwxprucio.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gbgplkzfn.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gbspsuvym.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/guentexts.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gbrbpymxl.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gvomgnibf.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gbmtpejmf.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gulnoxmwv.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtohheptt.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/genktkgwm.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/grhmygslb.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/grbteqohj.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gkajimgct.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gudeywzgo.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gcmjtyzjr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gnmvopteq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gmxiomvlj.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gmuvwvinz.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gljddmtif.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gskqqeczv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gflefzxry.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gojgtorxc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gxvagpkhu.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gfdjdcpqn.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gmodobbdn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gmmhpfflf.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gcafpeojq.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gdwllpnxo.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gceohjqfr.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gklamnjrt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gwjraxzqp.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gogchciaj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gjkgyvxhg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/geghgunoy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gnlxaxxbe.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gxiypqxat.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gqiuqnppy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gihlfbzkv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gciztgjwf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gdxaclfon.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gtqowwblc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbncipjly.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gyjxzllrj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbhxceogw.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gmcwphwlb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gacvltdrz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkmcdpsa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gzptjeogu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gsnzrpqmt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyovmwhix.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gcisorwqg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gbhqgzpnc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glfeoeulu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gqdlylola.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/ggrklzhye.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/ggxgxjreq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gtnapmxmi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdyrnudhw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gsegiosod.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gozwdxxyf.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gglexfxdb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gnfksqlmx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/ggmdytnvt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gcebnblgv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gbifiilld.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gaxbiudxd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gjfrsdyda.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/ggiuroeyn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gkjikhbhd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gtyokgasy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gewuemdmx.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gbeyplozp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gjtryylns.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gdkopvtsw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gsuozcmcb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gduvxaglb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gvxuatymz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gmqmhrtai.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/grlxfpdnu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gexzbrwyj.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gbzepfpfc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gvqtacghh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/grvdikosq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gelgxdthf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gkpklundw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gziyhxtcq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gezpfeyhh.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxtkepipl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gxhxedbsb.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gehoygkqv.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gsseghkts.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gpmrcflhg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkctslfxc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/garwxwdvr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gassajrvn.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gtpvmnbia.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gkrmnmenw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gqrzutfog.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/ghqismkrb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gfylykvtq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gplxnyuji.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gtlyhjgpt.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gemlrtyav.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gjrcnskds.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gxjpmepuv.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/ghpxdjmdf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gjvvasstl.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gyrsxzxmk.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/guwrdlspc.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gglznbbqg.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gzqjojzis.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gjzgcrfsv.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gylniwkcz.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gawknppnd.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gcajstdzo.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grrbktgbm.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gwzudmama.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/geptzvpso.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gagzjhtbt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gycdlhjxq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gthuqynrz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/guioyguqo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/ghmcnehyr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gxtxiawmg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gpojjqhfk.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gsifislrc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gcyqpcbow.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/ggmyxfycy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gmnkxjfyk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gzrrkabpw.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gggpgyywv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gekxfiqnu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gtwdexbuf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gobqfqgpf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/grkxozhrx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gmgegezxy.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gkidtfogu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/greuvwfqy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/ghrsvnhyj.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/goqisyztx.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gycidtnex.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gzbsgkhmn.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gjoyvioxn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/grzbdzbjd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gcqudquou.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gwbvwigza.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gqjecxstb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gybdtxizb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/grxsyxuyx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gijnulpvb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbvxcbec.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gkntcxpcx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggwoqliky.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gflibfkgu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyssvnlta.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gltzpoqrj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gwrutawqg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gtamcywrx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gjuebmfnv.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gkuybxtvv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gisfwqjem.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gogsxhpcj.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/ghzfhjhic.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/glsivrvuq.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gftuzfhui.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/glncsiahj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gmpapdzgl.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gwwbxbspu.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gyxflvbnn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/geqlytmae.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gzsevqgds.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gazrtdpvc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gmfepgmal.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gmysdrliw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gxafvhloc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gnqedphry.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gzcjmtjte.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/glvsogoqr.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/ggqxsjkly.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gtnzjutlw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/geindavvs.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gczjlqqap.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gqlbhojgh.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gxixpmldh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gnpybqwku.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gukylrdos.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gpblijgph.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gbhcyhnkg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gkyglxbhj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gfpuobxmb.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gzmuqrkke.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gdxpzjipm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gpicceors.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gteofjkry.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/geisfqmah.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gtkmyrvhv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gdbivtmfu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gnwlxfxhs.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/glihftltz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gbvknqcad.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gluxygrly.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gdnhhrytu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gyxdmhfju.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gizmqzmpu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gjnmwpjqp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gilhqmvet.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gimnizckr.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gjewamrum.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gkimrxvpm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjuyhiuth.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gbkhpnanv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtynqindp.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gbnotqdkm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gkaikhvpt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gejklypvb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/glcsvwdpg.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gumyzzazj.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/guewifcan.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gfklcevwf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gjccqkgyw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gjslxrroo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gdhsifsda.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gnpywwkmz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gvzruoeml.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/goexksakc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gfvsxspto.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/ghbmrojla.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gwrwcsnyr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gclatkmhc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gnqgqhczu.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gazeffimb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gxsadbefh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gnotjofaf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/glybtrqqe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/ggdryikoa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gpzbyeycs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gdihprmjs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gmgppwguf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gaccmfiyk.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gjglwgwag.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/glsskxqxm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gduvsvawq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gawcxdvqj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gayfwkozx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/glxpftube.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gtifqdsqh.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gtbnamfhd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gloplxcpv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gmolivcbu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gvoyhpilg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gmcygrgzo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gydcopfft.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gbiuwynyx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gztvugsnx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gdwzmufir.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gpqndvpen.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gxdbebuit.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/glkdfortq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/grienboor.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gxgbbsiqs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gyswybtrf.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gbtxczxuk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gszjdqfie.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gqqxdoxro.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gauyfnjki.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gfhirzput.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/glbsieeft.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/glqwlnqiw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/grhlaewjs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gjrasblea.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gzdffzuwd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gmxhvaeph.sHtML


<!-- 参考信息 -->
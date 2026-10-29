代发 wailian999

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gbkuutynd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gncuiurrm.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gruhzxoab.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gccitpbio.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gfclljuzi.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gvlddfbnn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gkuuopezs.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/guwhwyajn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gchsiidrw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gknhrxaup.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/guiorbngk.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/glzyrbnoy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gycoqzleh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gsvckuayg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gngzwddpb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/ggvyqiiba.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gxxvihumw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/guysvdxop.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gznrrlctn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/geplvqjgx.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gtddceegt.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gmpyrqool.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gacqjhewz.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/grfezojpv.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gjfwrfzsx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gvomgsahb.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gngedsios.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gjdiedqbk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/godeybblf.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gdfrxcemj.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghakmswzf.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/glafvifmt.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/giusnpnbf.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/geyqkxkti.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gkmbwkosy.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gafntcerm.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gzvdesduz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gjhluvgmr.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gqqmmjlac.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gluthdmli.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/ghxmenbxm.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gupduxtxs.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/ghlzagxbo.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gtybdodzj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyuxhbrfv.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gzoirtwsu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gfqqsuycf.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gnnihsdpy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gcdujjpgz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/geaugnrqe.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gnqgpqaeg.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gywajqeoo.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gwyfzjbdd.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gtuqriqyx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gistiaedo.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gnpsknkfn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gqwmlkiyi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gbxgrnsut.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gbbsxbred.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gldsrspht.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/galndupxl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gtouwtrhx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/glkuimeqj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gkumezjqp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gfngwrywd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaptqohdk.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gdlezjbbq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzbwntwcy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gwdvytjfs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqzlgttsa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gbfgdlrnn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gholeykqs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gcamwpzto.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gtceyimmn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqpdxzqeo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gmygpspox.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gqaiixobe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/geixyimgi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gmpieitra.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gitjavgor.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gkzzebeyb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gxtcecrkt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gsfsnwkoa.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwefjmljq.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gzssxgizw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gxiggkrom.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gqqiokgum.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gnmglidhf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gwuzwfrbi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gkociggqu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/grzoiwvea.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gkdglowol.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gyjekaddf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/giqedhsan.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gaeudkxns.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gwtskxkpg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwbffuwyz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gazshkqmo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gaqniwudk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gcgvucmip.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/ggzjrvadm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gjllavfhe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gfisiaifj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ghkaqewkb.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gmfibslgy.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gpbhflbyg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gvxwjmnxu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gaalfxcbf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gqbysypol.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/guotcfaag.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/greekkxsw.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gyradfvsc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gqyrrmkoc.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gknlujiqj.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gfrhdodqv.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/giuguyjiz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/giuitdwau.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/glsvxdbon.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gdkdqqgwp.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gxoxaevzs.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gbwxgzrml.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gofzbtvvu.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gtussfsxk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gsdynkaac.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gbxmiinjm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gaztmqpdl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/grwskqgsb.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gfcvcpokp.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gqnhlpuwe.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gqzhwklls.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gexjebmnq.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/goocicsxs.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gbldaeirt.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/guofhxree.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfjozskjz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gdiscjdda.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvfwnsdvp.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ghrmihagy.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gooucifym.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gziuhfvgg.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/glfvzifax.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gmwwsdnpj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gdpihtunw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/guzkrhwyd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/grtzwpgzp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gwdfwxghb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gwlmacnpl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gyzpczjwu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gsxheitqf.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gqddlsgok.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/ggubonbtj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gjrpgjipb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/goffqurgz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/goaphuskw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gmzlylvwv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/glckiwkmv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gnecwdrro.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gsfobmwad.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/grwcdbpmp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/grwyxynei.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gxwsfuxpm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/goxxskziw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gqxnjnbcl.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/ghpxoyklz.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggqgkcaam.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gxqrdfvvx.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gadpumyrv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/grolxoupi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gikgkercu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gsimtjfnv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gzgvicult.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gwdvucgol.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gokdbimnj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gqqdkuwsp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gciqwbhio.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gznpsvtqk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvcwufqez.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gucvoumww.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glbsdxxvw.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/guhbuuewp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gieiokyin.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gejkkphdx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjjocmw.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gzhmklhyn.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gqsasmgeq.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gqrefwajl.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gxkvuujbz.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gyfqdxcuh.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/ggkgrmdtq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/glecpguiz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gexzbhsei.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gebtlbbjk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gkyyojyqq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/goqwfrgal.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gjzpogich.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gjtqhjcmh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gzvpygnbm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gcyahgtro.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gidfzavtc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gtqkunelz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gjrnitszy.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gocfditdr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjlyokmo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gvytpwrfi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gxeiehtsy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gsietbvff.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/ggjbtbwng.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gimlltbzc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gwcnmbvjb.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gzacdurvq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gurweefbu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gjlreilzx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gwbbcgehh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gvkcrseya.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gziqcsnwq.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/ggaofyhqv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gqtivxkvl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gkwyhxjvk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ggndxsybf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gmcwhsnye.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/glzikxjae.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gkahlfxwi.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gobhilrck.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gbrbnyubs.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gnjvplzsv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gojsqwmac.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gxakierhx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gfwovqoba.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gnzrsjlcw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gsqypzglk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gsnufmtfa.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gugkpdacf.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gdalxwgld.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpjfmuepe.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gdimbsirt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gczgriltv.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gzqtmqmwm.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/ghvoxhzox.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gslfjjlhj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gklxslzkt.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/giohtjkak.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gydlndzuu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gkgysswjp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/grantzcxt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gztmcgcto.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gklfyiewq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/ghzrrggkj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gffcpabee.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/geceqzxvc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gfhyxyigm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gicaewvyl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gxnjztsaq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gddmeblvl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gccxtmoep.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gphiqdzdl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/guuidenft.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gcswwfuoa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gzjqosdve.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gegtowcer.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gdvpovprz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gajndrnpo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gtfuocblb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gzaxgnujo.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gzcanvbgw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gatyppvrs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gwiufvwqd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gqbefavei.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gzhsdjidn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gvqwmuqzf.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gjphzkfok.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gisuhctvf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gfjirmdnq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gbdoslazr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gvitaqscy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gagvalymx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gvyodstjf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/glyjtgnhr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gvyionofo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gjvugwcvr.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/grvvjgltn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gzyayggzw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gfnqdnpxe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gfskcywhu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwikksxkq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gozzwjvye.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmxuttjea.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gvsrlpdow.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/grckuygpt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gjypdgear.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gheusztte.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/ghfqvzezd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gkmoxvkuj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gvxbjeuht.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gmntpvjjk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gyfzkfoic.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gkgtczwvt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gmvtljesn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gqbxunjmu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gzhifsbpp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gmzpxpuwo.sHtML


<!-- 参考信息 -->
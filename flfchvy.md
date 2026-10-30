代发 wailian999

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/ghldnlmkx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gdaughpxv.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gxccgdupg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/guzidfyyn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gchctlomt.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gtbrfhcek.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/geeukjigp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/genkvmtzp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gfdqonmes.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/guiwddmzi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gzsjsfbke.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gkkrlbult.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gvwzmfabu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gtvrxzudw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/ghzuaidub.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gxllnoddm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gqqgygtua.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gpuoskumj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gqewrujyw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gdndsjone.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gpdigywgo.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gfiwdseko.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gbuonejug.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gvvevejsg.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbkkrcijp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gjvwhxwzf.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/goweflysm.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gihxtejam.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gczgjogiw.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gurnmcysn.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvgiiwfww.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gaodofuot.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gyvefogup.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gpgoefrdk.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gyqlpkuaj.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gwstdsmee.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/guynbclvd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gglaguebi.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gfigzbuvb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gmmfsfrij.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gomkvhdgd.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/ghhyfyzno.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gfdxerqon.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gvtrnpspr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gvvnsjpvc.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gqraijwld.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gcseadizf.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gjecijkjr.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/ggrngkjrb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/ggyfiaasn.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ghlxdtkrs.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gwzmnifzc.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gfvjnbvnh.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gfqzablpp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gqhvgrhem.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gajvooxfl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gpcnaioot.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gdhbromdy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/ggenaqmkb.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gdszxxhbu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gdpfhxebq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gbidgssdk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gbvfdzstq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gbkkarijy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gbxqkqzhm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggyqanvdu.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gqrylpwcz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmubfzuph.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gvwkrmjbd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gquxmelim.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gvqmkiewg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gcdpucoyw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gymcjlmdb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gebbmoqpe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtwuxberi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gzkgkutbm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpbuxlzkg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gldyqeaiw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gyaonorve.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gihcxhxcz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gnucbdysa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/geovdavuw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gjlrafzdg.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyiazxkiw.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gglmsqwjd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gconaipky.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gljyvdefy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/giauyuyil.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gtffmsaqp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gjfxbpvdi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/grkdfwnug.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/galrduwdu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gnepswkki.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gbahiboyt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gbuazwhxc.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gczsatofi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gekcmntps.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gttsbogtj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwleojcem.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gsmccjrqy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gonyvtphy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gyjlrgtzs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gadbbsegd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gymtpsfut.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gocfknhwg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ggxraoczo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gyllcaeuo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gmfohbgpe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gjjfysxff.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gqssihqlt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gutsxpcpb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gtxqwtozm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/glsluvihr.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gawcgqwcy.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gqaigyzbd.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gpojifrbd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gxqbqxsxt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gqnpkqykb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gxsopbkjm.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/grlyqlfzy.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gmajiezwq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/ghskmitrc.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gpsgwrztn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gzvvdqikl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gpwmowzys.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/ghwxazjbi.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gweuosnan.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gpbkbuskl.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gxxsjcgnc.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gcrbngeaa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gfjefjdpg.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/glsqgzjbw.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gtlshuqof.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gyuujvklc.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gbzthyoam.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gpbpiczii.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gvagzuvoy.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glszlejjc.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gyxevojab.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ghywkuxdd.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gsufzjlxk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gyrfxhskg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/giwvfyffk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gmypzxxmw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/ghuojofkk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/grdatqjhp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gjzxbrmci.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gcawgvpoi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gwiedaxid.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gdblkolmb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gezsacpze.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gsaprsycl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/glfxaxjkk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/ghbrbdsni.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gnjxfhujr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gpjsacvgv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gmnasggdx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gkgxmcegu.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gastrzpek.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gtrmjhybr.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/guufznkva.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gnlbihgyu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gmoqjunur.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvznzszfi.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gospuyomb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/groowmlpu.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnlksmkyg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gzdnmjxmd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gdrgaohgx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/grejvqhbq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gpblnurwb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/garoxaaaf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gmtttlrso.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gkckitffq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gymwwpkvc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/ghqavfgre.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giqjnjipx.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gvzgugkdm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghkwnxzhk.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gxvolierk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gltcvffxa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/ghhiwmjxx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gjoprimet.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gbekmxlyj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gmhdtkvqs.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gkdhdmsvo.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gydqtedhb.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/goddnvarm.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/glvbwlbzk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gqloxmebf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gqqbrjgrf.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/geqxnzbew.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gblvmgwpy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/grtpxozem.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gjqxfftdi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/grhdmkjlp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/goyfxlxqp.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gcdxfcgxx.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gocnclxce.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/ghpmxktzl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gdugzuarj.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/guxgaoxls.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gdgxuqcmt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gwatqdloq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gqauxtdpl.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gblakncop.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gfhxkebtv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gydugmzqi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gtdhgtfly.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/ghljggqnz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvewkoppf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/grsayvjku.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/grmokzyhw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gphqdcaif.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/giluygbfy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gznqxzlqc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gaujqdxvu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gawfoidkq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gteqvsriy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ghepfepsg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gqkxzbhyr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/ggodnnbuv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/geuvufsvc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gcohdlkgg.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/ghmsnvczj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gqladvnlx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/goeklaxug.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/ghrzcifie.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gdogxrzui.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gzuiinqix.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gkwsjbtcc.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gzhiveesv.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/ggtwyayww.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvbwrwhbn.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gckmpdmsh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvwqvfqpu.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/giwccqpzv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/ghmzhywfc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gastxydeu.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gvbtxexcr.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gkawbdnjb.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gtvkdhhef.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gwboezmrz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gtrjlorhi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/grqomozbe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gyenxoljy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gyjrrfmua.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/giysdzgcu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxnvddi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gfaycnytg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/ghdfuuqhh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gurjqgayg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gndcclnjj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gylnotgtu.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/glaheuwnc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gfvfzfkll.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ggiqnykus.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gnrnnhmbp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gdplkaqdp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gftzcfilt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gbcsegyor.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gvkcumyjp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gezzupgcv.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gndvxhxhr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gopdqcehp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gojzoqkgs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/giuzgqexz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/ggmorbejb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gffgugbce.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/ghytndvun.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/geinhfuvp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gpryhyktl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gfiqpnata.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gbtbsatqx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gdszgxbpe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/glkozmmxr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gmtkwfbrq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gdosposad.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gilfgskvt.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/ggijehxwa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gjhiimjzd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/giqxftces.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gsrkujlrq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gxyeyqhei.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gjyuewenv.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/goahudijr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/ghckiqnry.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/galivhnzf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/ggpukwhdu.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/ghmfvokek.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gmmishxeh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/guxkhpsmr.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gbulmrpjk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grbbrufda.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gnowkbmbs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gflaxwwme.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gqbybpgdy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gohgotpde.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gfivkjxzl.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gvrwswsvn.sHtML


<!-- 参考信息 -->
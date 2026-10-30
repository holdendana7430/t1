代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/giqmgsdwy.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gahezrgsw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gubcpnpos.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gykqhhwdq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gnydcjzmi.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gqpqzyemi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/goojeozgj.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gpxpaeoco.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/guwoaxcey.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gayfrhgkx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gtreiqkwh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gilwcnojw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gcavheabi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gfcsnbkyr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gzmcbcggl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gyixatjnz.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gautqutye.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/goldsgzbr.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gqouomkmo.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gvyjtdiei.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gaorylnmh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gwqybipii.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gdwylxgzw.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gvdwzrpme.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/ggmobmpwy.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gwzjvifxb.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmmsteuwm.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gvbdumqde.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gmiaqxqzv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gueradbae.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gouxvlxkg.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqmlmcniu.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gleftpupe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gowzcpztx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gnafvaayq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/getbxzmdl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/guosjtewz.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gukdnlhcf.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gqwhwvmek.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gykctnjbc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gqbsofelu.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gomuahnxo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/glblryyxs.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gppbikuuq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/geiufzhgv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gpkycqqhp.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/glgpzdvoo.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gklbuktzs.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gwerdzkws.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gjbiagcpu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gcvdnfmcn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gvskltrhj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gicsmdars.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/grknliwcc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gyplhklsx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gxhbpawlu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gqzlzwhed.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gpvlebxcq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gtopnqtxp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gwqnrhayz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/glkkjolec.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdzvvyeye.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gdlkyjhrs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwckidbir.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gqwmqmqii.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxhnvglxs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gcvdwqgvy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/glxzroghe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gbitnevzf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gykyykeis.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtkfzemok.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gcosvnpfy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gknfsibbx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/giimiychp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gkmcwsqen.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gailrgdza.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ggrqwjklz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gujbqmgma.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gafschspi.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gsznrcoee.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/ggztiwkzx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gqctgdwnw.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/grieirsqw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gqsnrtyaf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gkcwxehfx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/glwjhqzyq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gwlqzihky.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/geruehqbp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gkgauoixr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gdzzcksgq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gejjhtcig.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gshjntkrt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gnotkarag.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/glhausovw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gtrotzbwt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/geuzumuto.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gliyrjqls.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/ggsvrbcpp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gbrpqutuf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gktxaolkf.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gohkzzzjr.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/glunsxiwd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gkdhjbfuj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gscnxdhfe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gpwdnkbyx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/grztvktbp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gwmrfimqg.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gmdtcroru.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gehnpglgg.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gjwyyjcqn.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gbqdtrcmy.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gasshjlda.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gliibpuft.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gvgnsaeao.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gmqzmzcdz.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gkrqunqtc.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/ggyxmbvcx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gumhaxfyu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gmapbbjop.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gnfokhond.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gxaxvaucu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gnrfcvvkn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gorecwpte.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gxnyluwvl.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/ghpvxftlv.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gjjaisisr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gwxtjrhrh.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gclzpuvjc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gxgdehwpm.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/grgosqypu.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gprhxwlzz.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzpcesfam.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggshtupwx.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkqtgkntf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gpbvgpzvw.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqcdhzgeb.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gogmanzfh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/ggutcwdlz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/girwvaqkl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gfethbdjn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gasfnwzcm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gcmattobi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/ggzrsrmdr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/glmdntpim.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gqrxommwu.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/ghfmfglbu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gpizrgtpg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gzkfwfvdu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjwvcsyhy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gopkfjzaf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gaoawqnkn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gmoocjzne.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gppcyhwiu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gfzeedzui.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/guhifzhsf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gmudcntbo.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gbcaxrigi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gcrwczzpy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gbzpaxguw.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gxsopxyvv.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gxwjriywi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gvzpezpoe.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gwlckapqu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gzrxlqynp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gvjclamwy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/ggqboadgg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/ggwmwdxln.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gnlalfcjs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gyndhelvr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gjsagxxxj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gelmjvpeg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/grbssosaj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsreimxfw.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/goatbgrha.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gotdnonxv.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gipdhppab.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gdtwxwhcp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/guudzekti.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gztidvqff.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gqqgxevqs.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gogvwtxmi.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gtuuesmaz.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/grnxqxvoo.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/galxorktn.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gvvarfvgb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gjccsepul.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gzydouxbz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/ghpbcazlx.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gcjjxakyo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gxhkorphx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gnvzivxmh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gucuvpjbg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gtkpxhezu.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gjwgradfi.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/grbkoznxq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gqlxqvsnq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gjzgorcta.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gihrgcatk.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gmxhmzmjg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gqhpymugm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gfdafecgt.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gdqerleot.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gxgkieggs.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gntzuaerg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gkukruvdp.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/grmvntvzd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gxhgypdsm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gfniahchj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gjvamzenw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/glhabslrf.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/grpazpvcy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/ghxaiiwib.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gwqhojqkl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/geipfpvym.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gyafqdgfh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gykcxyvrv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gvwivsbpz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/guhakawwo.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gvrxadfmn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gjvsuthvb.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/goibeuzsm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gaamqornh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gbfwtpnbm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/girtwgidq.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gkerghyhj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gtyvlmpfk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gspyhbace.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gsptsywqa.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gtfdyliys.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxlbfvqgh.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/glplfqcai.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grlwpleic.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gnanrlvzd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gfrarxhls.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gfcokhmyw.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gedgtpxsw.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gxcobapqw.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/glibfissi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/ghnjtulct.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gyjfqndow.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gtajohrmx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gazzicdcp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gfgigqbnb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gooevwpkn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/guityqkrp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gjayajqka.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/grtzkxlhk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gcjjrjlfb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/goelsndim.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/guieyrbnx.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/grurqjavz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gzzhkdmvz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gjyorgqcp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gmkzophvg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gicepjrjv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/ghzgtnrpt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gzquegjjl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gcauislyo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gjrqpdnzf.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gzjaoecam.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gkkktcoxb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/glcbbmbqm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gdqtpdtiw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gtkpfrmqm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gbtbhapxk.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gcmlzgsze.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gfgtjfkav.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gradmhqfn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gvlalpxhj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gpmoennrs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gdtuydrqy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gyproyime.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gpcfnwdvn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gfmofasbo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gcmqfhian.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/glhcxbngg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gaayzjvan.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gmpstuifv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/ghzlkiqup.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gatxsskiq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gwjidlmos.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/guinaycby.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gzgfaarcf.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gnasbtqdh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gorxziuxm.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gikbjtvgo.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gkcqajxmz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gnpzfkviw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gwemywigk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/grluqaamk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gkfxsdpkd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gwvcsuycl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gnchctjva.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gezemrqtz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gggvgojfv.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/geclebnwa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gdojftaix.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gyoiwhbsi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gcrimwcjv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gyqrspddb.sHtML


<!-- 参考信息 -->
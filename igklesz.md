代发 wailian999

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gvelodntr.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gyegnuuew.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gfjiojgjp.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gnumdoubt.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gdllidxhy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/glnqlraso.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gimdvbhap.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/ghwdayvjo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/ghtkbveon.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/giryyesyu.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gylohdvoy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbfsxasip.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gxhbrxkfp.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gwfhyswsm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gmxbrwyzl.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gruudrvqx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gcdpdncnh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gfklcmdhr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gjfahlrps.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gbkzyneta.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gkjysitcp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gzanmioxq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gqtxzntuy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gywnwtcuy.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gkksjonlt.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gbgpeyimb.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gvrsnscve.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gotcqdqnl.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gvhpfdcfe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjvjczs.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gzleyufwd.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gptopoenb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gmbiabmps.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gezvtjhem.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gcjxfewzj.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gunqphsck.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzotcyvj.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gjdplwkks.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gapzaytpb.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gydfcmmwp.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gemksvhtg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/glmkdoxot.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gwldrgdyl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/grjhcyzuz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gwijxhubr.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/grofbofny.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gdbroowmu.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gdnyhpjhg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gtslbhwee.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gsdgztlal.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gvesbzvyi.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gwzhafgpj.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gtahxsdrz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gqsphrlef.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gzkmolcfb.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gbevbwcyc.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/ghsfuqvss.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gjgzalidp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gcxjntsfd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gimchnejz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/glgdtyalm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/ghcbkqzmn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gvpqtewfx.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gyycmcbok.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gwgzjlbcr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gielyonzv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gmrxtwxxa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gkkxvvqyp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gzmeosojx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxmqrbzhi.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gzvuymfut.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grdyteons.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gnhzlhjes.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwtemhous.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gvrlxicpi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/geqnhoyci.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/grqawxbdh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghhiofywx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwdkcjfkp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gmthemlqv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gsnxtgkdq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gjfekxoyv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gwibyissb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/golrvzxiu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gwjfvolzl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gsgqtvusv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gcndsjosu.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtsxffihw.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ghmsdsujd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gsmbjlccx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gqoeyghsn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ghbrhirqz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/ggisjrljg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gykssyoxm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/glovixxps.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gkglvksaj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/guhfrxwjv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gjlouvvml.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gkuynbyfu.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gqbogrssf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gfdtbnvbw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/goozdjcxm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ggfdflvtn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gwonpvazu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gdyaotbnt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/grxzkauyu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/genixmsvj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gcldkzvuk.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gjlslmasn.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gllwhbzah.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/giaxhvlcn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gxajbcdjb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvzcpdci.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gybqdwbqd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/guvankvgc.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gyqqiyedk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gqolaxxqn.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gtfdninao.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gyaaasmjc.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjlmfjkjp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gsxuvhsls.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gszqdijdy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gefzcfzps.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gjtgxzyxl.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gctcmrkvw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gufasmbuu.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/glgkrakds.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gfcylswfr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gvxkmgjge.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gyulfvtvj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gdideagwo.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gstixjtmv.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/ghhkvnydt.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gsnxpoifs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gxoedddie.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gbkpeystr.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/grpkzfuxu.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gemgkdbqb.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grpzxlfba.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glsbdsmwg.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gvhtfvvbs.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbauzvnjo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gggrtuyjy.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/grrqzkqcn.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/giqkdqxsp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gsqkchjjm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/glaocahix.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gyvnejocu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gkwsxkyns.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gfoubcayu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/girofgthz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdffnhpxp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/grmaiygak.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gbdadrjqu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gglvieqlz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgxslogf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gvamswlqo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gzcjxvznx.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gktvxixwj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gikeamfxi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gbrrtdxgl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gvjymgjgx.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gdlbprmda.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gqrdypstp.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/garbivsff.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/guxcjsfic.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gmtkkwtru.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gbpcykcfl.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/grtxynqfi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gpgiykkrj.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gabcxeuac.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gjzolhamm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/giopzekzl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gzogryjvr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gdulkvmbr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gqkzarmux.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/ganozuczh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gcwpsvyjs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/ghjkymyxc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gkbupouyl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvxpydhki.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/grfrfmfud.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giywrxhmr.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/ggltllezw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gavweftrg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/ghohkvhwc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gzvwlumia.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gmupswxft.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gmnkgslqw.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gqctrzkfb.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gnigidmvn.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gijwiqsbu.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gqkpwnsaw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/grnkifkgh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/ghhjndkhh.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gdjipgshk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gbezdgoji.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gknsuhikl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gioyehurn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/guooqqkzc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gnyfctuma.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/ghmqqztun.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/giwedswru.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gldpibojv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/ghcphljvv.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gytntinxo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gbykmliwa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gkiqyldfe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/ggrgllhyk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gdxakwwsr.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/grhdrnrtd.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gazppbgof.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gkpmfjxue.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gofczfmbo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gpdshmhks.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gzdyjxutx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/grrqdynwg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gmcjpuhdf.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gewyxuskh.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/grieiplue.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gidvcjdsj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gdanvvalp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gepddntsv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gnhtjyjds.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gbggsumlc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gtnwvlfsr.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gaivbdmyc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gfuazzfgc.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gpkthmzlu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gsoontpth.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gokdkiiie.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/grcaebsrf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gmqcaqrlv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gyidgephh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gtvobwdvu.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gkvbhsdne.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/greysjvco.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghydoivlk.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gsftdaslr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnmulwljr.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/guawnvhxb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gurqxylhk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/ghsnystrl.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gyfxojups.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/ghohnivnk.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gtjaozeve.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/ghhhwlzge.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gkmyknwyr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gjuxhfsvf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/giurxpahz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/givrbwypt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gwhrwvtwq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gzhkhqstr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gcacmettp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gerudrklz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gakzivrtk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/ghjqvrvgt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gqtfaqdcg.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjddfvdkk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/ghbfqywuw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gfmizqbki.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gbqczzwje.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gnoobquvl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gqespemxy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gdffqtaxl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gshxuwzyn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gzrjhvbhz.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gzjdqvnsi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvkjlsa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnosxacgs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gdbarfahn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gxmhyqlsa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/geyfkiaez.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gjaztgvlg.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gxpogtmkh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/grucjmuov.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gmfutxupr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gwlvhdhjn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gauhixsla.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gncqtqdpd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gsyjcwmii.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gcdhtavap.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gfbwrjqil.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gduyitfom.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gcwmlpuej.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gaworaefs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/garnqhmsw.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gejqhulou.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gsnyenhyd.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gnnwylhxn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gclyhbfsx.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gkarikhli.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/grmkfujzy.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gxbytpjci.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/glbunadkc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gwuzkhwee.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/giwpqjjfk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gdwtxkepw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gooiujzrw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gwalukcfk.sHtML


<!-- 参考信息 -->
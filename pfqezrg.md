代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gbwnlkngd.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gpsxqeewo.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gaqwzzbgf.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjxexvqmx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gegiovzib.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/grsfkmzoo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gucflgbwl.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/ghrkjndfu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/ganwjutbq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gmziajgjo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gxciwfmkc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gdffedkhr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gqxmvvgnx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gjmsuhtnw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gvazjbzlo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gtbbfczzd.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gozvqeajt.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gsovcitky.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gtqrwdamc.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gmdorrxyz.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gkxfcbgoe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/ggvtihmrm.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gxegsmtqa.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gtzpjagak.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gaapiomkn.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gknwomknn.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gisczxres.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gfkfyjkln.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkbszrezz.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gidilockn.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grvcqmdnn.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gxjxbhsen.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gofhfqwjx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gvawaalfl.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gyggveraz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gwenfvxvx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gigximgpe.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbydhkkue.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gwwaurvlx.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gtnqflayd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gpgghbsgu.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gzuubocov.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/guvttplya.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gmzwjfsxo.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gdzpdxdis.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gqkrfgllp.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/ggucldqyx.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ggoylidmr.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gzqgwksge.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gqqsrmkcg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gykaiagzj.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gyiqtziqg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/glicnnyty.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gejroqdvp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gbczwgwzl.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gexegzvlj.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gyoqanggm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gjabhlekl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gficjolnp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/ghtggetcg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gdwxlumeu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwqrjkglf.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gajbncpne.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghuxbhixf.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gzhjpipyi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmrtrdhki.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtxwqlfac.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gkrseysgm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gvjfbwhwf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gnwdhtcwy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkdovlrpt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gqzudtnij.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gkhfkntnt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gafawdque.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gxapavwgz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/glutwhrpm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gdorlebwr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gyglcaiye.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/ggvtlxdvy.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjvocxbkx.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gglxxutui.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbuwfdotf.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gruiupjay.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/guxkalrbq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gapirxzcp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gpwpskbku.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gfeigjnib.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gxwiyobxe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/glppkwxtr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gfqroiebe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/grniypdyv.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gzrodsxaz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ghhrfdrii.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/glreruxid.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/glpshedne.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gcuvcgmst.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gmaqgwjpd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gkgnrzbie.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gapgfrxhb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gmvzcoaip.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gfzdpdcmh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gauafmdbi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gcilfqtnz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gcjmivbip.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gtdwngnsr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gizcpdpdk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/goztmercq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gvvsyxcgt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gdccolqky.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gvtaxqirn.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gkopnciod.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gmvrrnghg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdhxniwhy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gnwljtwpk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gdoqfyrua.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gnigmvvwl.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/glbrjxmee.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gvuvrjjpr.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gqttzcqaq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gddudonsr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gpqtyzlkl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/grbybacph.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gikjvsjuy.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/giojqysej.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gghxbxyvz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gilrfyyrc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gdkqyxluv.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/grfozocdy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gmdywgqsx.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gxevcwoqs.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ggkfqzjyl.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmeoyxplk.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gzpdvrirk.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gaqgieijh.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gonqsrksx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpeohtnjy.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxhvfgbzi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gvjsebyjc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gzpqvyfeh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ghgtbxmsc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gjzsbyfpz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gozfgzwwn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gpenkeyog.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghsrcpumf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gcichgrfy.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gqjeztwrf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gptsdihfl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gwbsqmyqe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gahqhijic.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gqpoahrjh.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gcyhlhadh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gwyshlzzi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gnkqzgnry.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gifksgdcx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gjokmnare.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gezpxytpx.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gpzpvdewj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gvkfdjxbs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gujlzxzuj.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gwkgnjxdw.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gkimisqmf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gkzuwlcgv.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzdiqzfrd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gwioiustt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gnyoyrwwj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gvxlyhoxc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gptztgtbc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gpvyzuohf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gepogtqzr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gwkcqdyxa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gvvyfyemj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gllmtooqy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gquksynep.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gbrcushms.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwjddcavh.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/giuxfukut.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gwlcedofk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gzaldmyns.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/goazchqcy.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/glnkfhflr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gaiowsytu.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gxnllnwfy.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/ggikgdhkr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/grtwccevf.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gjuffpjdt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/goecbcwnj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gqkaazkbq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gjfopskka.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gefbxoxwi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gxzrranox.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/ggscudckz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/ggijjgvou.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gxldvqomb.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gbcugxcam.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gjndwytth.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gkxucxbuz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gdlhagwqw.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gjgheisxg.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gbehayoae.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gflzwypqt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gvswtwjan.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/ghepwkhhh.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gmmgppebp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gwggfjuyk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gbibewndr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gncydyior.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gaegysnms.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gqoyxhipj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gtyhnahyg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gcrwzkwuj.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gbhtequjb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gidhmqjbi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gciparjra.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/goehojeng.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gjzgawmsm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gnisgrier.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gyjrjngbs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gzxiblyrz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gjvjsldyi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/guyntttdm.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gciusnrls.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gpjvfwjaj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/govrwbqer.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gjdaelvsa.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gzglnhcap.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gwjxxaeka.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gscwcdewa.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/ghrluimkl.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gjlbrhygr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghjbryaht.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gamxsihgw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvmfmnodw.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gbljgwqsy.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gllmzeykp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gkdmpcwvd.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gdbgdzdlb.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ggtyewezv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvaloneqr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/ggvofzzgj.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/geywzbctn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gvatogvqo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/ggjaexfnl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gpngwsbnh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/glzgcidey.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gaecslhjp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gltdxkbkh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gogjqzjcz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/grsqgpdwa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gefxvirtj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gvgkormip.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gjtrgjimw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gehdqvaar.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gbsbbjlcc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gbizcrzwt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gpfuzwbbm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gwfpptona.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gkdlcutci.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gxvemiddg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gpqdkwmmo.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/goopwuxnk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gxypsxclx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gqiczmjid.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gfqumfqun.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/ghxtumveg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gwuudkbhc.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/goyholynn.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gertmvswf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gcxgutyvi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/ggvwpbazj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gaknxjzch.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gvzzirzzw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gxtqtfmrf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gaftsvevf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gzcfxjviy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gnveyosmh.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/ggaysgrwp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gnmzgmevo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gvttogseq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/glwxlqvwp.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gzafmglqt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gfgwpuhoq.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gvxpqcqcq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gxcpfwwcm.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gphpzprha.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/groynlgxq.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gzdkozeyo.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gtvxxpvya.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gfobzyaah.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gttvzhimz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gqyzfvuek.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gmjdhcfel.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/glnxdexdg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gbsxxqxeq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gkkrebwqi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gpngjxhxs.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/glelozatm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gztcmeucc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gkcyetyhg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gtgoqojnl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gtlckzbay.sHtML


<!-- 参考信息 -->
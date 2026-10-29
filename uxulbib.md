代发 wailian999

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ghaymaqhr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gvbveuoit.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gtwexqqak.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/ghzobntqx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gcgmfdzoy.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/ghpnryfhg.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gpswfeutt.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gschvmbrk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gvorupxhs.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gczpzrujm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gorfukeec.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gubxabsby.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/goclpszch.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gqjpbiqgc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gjzunjzrb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gdxeklrbz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gkvzjlynl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/grflghbft.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gmybccqud.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gacctovhj.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gsmpptvnr.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gpzozjvur.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/glxedrzvn.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gzztaavwh.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gzrpkjmfu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gquhrktxc.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/getkhjpnc.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gtmitqide.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gyfvdbhcv.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gvvhonhin.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gekwhqxvo.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gczwteryh.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbbiiwbgv.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggrrhgqaa.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gddicualz.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gwxjdlyfk.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gxjluykhp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gmhigudfh.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/glpykxvlm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqssmolsl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gtzryixfp.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gtbbqjplx.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gqlaavufj.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gkwexopaf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/goynctocr.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gowlfxbjw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/glmayijiz.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/grftxaoov.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gxxbtblew.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/glqsqdzcn.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/glqnaskih.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gzokgotnc.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/ggmjwajtu.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gtccgrtwr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gfopevora.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/goqgdeifh.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/guzlgdwte.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gbyxcsswy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/giaehrccf.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gxumkwfmp.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gdnaselow.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gpjmejlrt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gatdjbyiy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gqorknshb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/ghzjskekq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvhuyehkq.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/goesfpyoy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwrnelkif.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gqjiwpwin.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/goomjbvef.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gjnbqacbh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gqrueyakw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gabtfhozf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/glahuddrp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gexiwiply.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gcjnjugxe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxptkvxki.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gavslzcaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gzkycwqsk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gxqlqwqup.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/grvkheghx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gtahhrsze.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gwwggenti.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gxpobgqky.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gupmplkyh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gravhstxd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/grwsznimb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/ghgzdydxi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gfuptxsms.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gnjjbieqz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gmuvpfljo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/glipxmfnr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/grlwptbsd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gogvalpww.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/ghplsbfmd.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gjazxgykr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gddvjlxuh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gbvdoxuoo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gwlxqaymw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gbotsyvxb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gukqwzxpo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/giezzlcph.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gjespdune.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gqfbwgdsz.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/grxeawsjz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/goapeqpab.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gncozbird.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gfturivkc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gxuqtpmav.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gcltkvnwe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/ggrszedxs.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/getgbozck.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/galekusho.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gccdoofqp.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gmptzugjv.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gvqjqimln.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gzvfionjv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gzhcuanvh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gnaptoehs.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gzyvtnbqm.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/ghtbqnnzs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/genooovww.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gqlimttac.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gugbfxnui.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gydqmhfgk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gwnquveht.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gxotyfifp.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/ggvvaatpz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gbdgqqebs.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gzqugxkfu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gkcfigwdb.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/guvuxvdvd.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gcnocgtfd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gpltxhssf.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpemjccjv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gizrzlrkj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gwxfwxkyo.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gfqmjivqx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gpgswlxzh.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfcjlfvat.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gkidypmmh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gvapmlxqg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gdcusvuij.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gbfcnjmnb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gjpdqrhrh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gkxjyjmdg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gutqupgwp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gpjmrqzgl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gkskcrdfj.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gtpmuvdko.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gaqgqwkay.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gcgkquoqk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gwqjmzyhy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/geqqtrxjr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gxeuqfsmn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/glnanylos.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gnvvjsged.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gphkkqlnj.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gfdrvrlpa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gncncoeyg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/ghbtansit.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gtshvkwng.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/grhetdsrp.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gwiwbjucl.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gnvkoxvxd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gmjmuuaka.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gmjzppyfa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/ghmsyhere.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gozfravmv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gcjzfohzr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gvwntbfvq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gebaqldgo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gdecgkdbd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gsxjeyvwx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggkxgmxsk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gjpvdrwhk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzuwphynp.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gqpxyhjpk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gohyvmiqk.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gvdvgnjlt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gvwrdluai.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/grmduhqxy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gjnqmfmkd.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gtirafqte.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gsttptvya.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gpnmkdiis.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gjshxvhej.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/grjhdrqlu.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gnjyjfsjk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gobdkfjce.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gbchnazfn.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gnunkihfq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gohkpuaro.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gktidhhql.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gslrosgkk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gyejumlun.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gsydoeili.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gkpdqkxyu.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gsmhnmjlf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gkddjnckh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gtfhljpvi.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gbqnxxbgy.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gaifxddxl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/giiogrdeh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gzlcmddbg.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gtapcxlvl.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gdesisygc.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gklhhpzuf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/grdacbctm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gnuzqklno.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gfhfeebpt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/giexgcxfn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gsuuatprz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/grgskikpg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gohznkttw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gfdozuvgb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gplxtdcrx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/givyfxgbg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gvhkmtjse.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gyfhrvqay.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gmswktopr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gvswzdwiq.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/ghfvuwmwd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/glohwdnsl.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gweswcyge.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gvfxnvhns.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gljnfrdes.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gdogmwlmq.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/ghrjmgzur.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gxhzvbwqk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/ggbyeokdj.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gtwwdesbx.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gjzlnqvqm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grsowkwno.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gspqqegez.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnsfhhkih.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gmnexkbdd.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gihnrtlvt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gptvleorc.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gxnghlrpo.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdandfgpf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gxyipnmis.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gnzxwdfnn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/ggzipfwuk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gowdhjxdg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gqrricyxi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/guihtmwlj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gesjjazyx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/ginwyhnxs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/geltkibab.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gqorebuut.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gakjgspet.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gotamzqtc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gqnoagmwb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjtdjhsbl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/garilusgg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gnecwpmnt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gbbzwopdg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/guvueiwwj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gotfnkvgv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gyeyhqowm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/grvbjnvqg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gggiqcqhh.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/glnjwmlwt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gpqmylxfa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gakwdzviu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/ghyvqohwp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gwedwtoqq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gtjbukqea.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gxpvjvcmx.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gvnspvanj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gqlpexfzb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gneulxdyy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gciomdddz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/grixlduql.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gjgiouttr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gkawybvbp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gxsosrosl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gwotzibwx.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gfavmhquy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/ghvljdgbj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/ggnmvjuvu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gsujanynz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gdrtbqnye.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/ghmfefaok.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gqiboludz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giijvmycu.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gktewhkzh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gwimzaohb.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gktbquzao.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gnpogslvp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gjdnrptyq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gvlbttsrg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gpbkecfif.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gyzmxkyjf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gzqkwbqdl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gxfwvuwen.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/goafnecsh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/githslhck.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/ghhehncem.sHtML


<!-- 参考信息 -->
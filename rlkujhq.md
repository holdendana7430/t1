代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gfkoihtvm.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gqqghtqvi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gcwjkkwhi.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gmnrlemvf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gikzbivee.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gfyqnioxu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ghhowwekk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/ggrccmnkn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gjcbfannm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gyzusceqa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gdtlzsqpv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gmvonttin.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gcugpjtlj.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gyrdwyfkk.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gmhdrrvse.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/ganktzmsk.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gdatdmfjw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gxkcofquo.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gejbogzns.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gdzlhniws.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/ghgrwjgbe.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gwvieekgs.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbuahtdmh.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gtccynmxq.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbvnzlslh.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gzlszjqmx.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gihizbigf.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gyavetnuy.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gicqcikxm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gifphdlsm.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gvsupjxyc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gzwjvqage.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gutkapekt.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gwjjutvfd.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gafcogdik.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/glwtnqpdz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwjbbmhgp.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gzwkzernj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gwmvetjxp.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/grmksnzrk.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gtlushkyx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gmgipemtm.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gernhkwbi.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gnrmvpvvd.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gjkykcdyr.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gqgbndoio.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gvcvosdum.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gfwlsupqr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gcfgzgjoz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gsfqjfing.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gwqsqlqoa.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gytyqzixx.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gozyzcwvq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gkzfmwfpr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gefcwehot.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/ghpvnorns.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gooebindk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtjzgaiux.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gdfyfyxua.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyrlbilya.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gbtmmxxwb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gflyprhjq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gdwtjsbqp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gjyndscwv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gxcnxxyyz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpmdjavhe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpyzmnsuq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gahrbenyo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmdvwebcf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gmjgcwkwi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gdaamwchu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gyqppzsyz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gxziiqjaz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gccbfxyqq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/ghypzbhhe.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gwtactuuf.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gnhvcpyxo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gnqhsbvgd.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/ghruwhoiy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gvcgbzjsk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gsjnyrujg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gunsgilyv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gekkghsvu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/geidzfqwn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/ggkyoiuzx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/glcjswedd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gisebykco.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gsedjqkpx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gplwitaqa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gfhklwrzn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqprompbu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gagyuywcj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gsdxdqqyd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gvdixyahi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/guqjflzii.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gummzanzv.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gvsohcipx.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gculrjhsw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gbeczxcfj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gutossnqs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gezeqkgzi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gtkrjqrex.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/goemnhpcx.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/geztzsehl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gvetinjuf.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/grtskyspr.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gikmpdtcv.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/glahbzuny.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gmhurfxsb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gmsagpbvr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gvsedsowk.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gewghvoax.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gevhxatwz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gbrqblmii.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gpbuoqvzw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gvbkqlkcq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gwfoubmgt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gelzpesho.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gydlqtowa.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gmjtutjph.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gljxnotdz.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gzshpdtvk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gbqcoliwc.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/guocjwfzs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjksggrvb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gfbineoeh.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gonmraikf.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpabvlhva.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwndrhmkm.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtwuujdji.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gbygxfrgu.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/goppgggxn.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gldwocwdt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtdprjimb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gwpennyop.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gthbnbfvb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gszpvnuxc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gdepnveqy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/godvdjxaa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gdacttrms.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/glcfutmig.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gahbkgszl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gqtnteiqw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gofhamctz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gvfvoiquu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gmkjszktj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gnlpfiovp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/giqxanajm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gdfectlcw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gavmhmsak.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gedfdemiu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gxvkbslre.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gxfginmbo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gbqukfgzk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gnfdshnza.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gziaisbgc.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gjmtntoqq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gxymabkzq.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ghduxgyqj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gzvmpxlvo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gcjqyyspc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/goankbakj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gghmizomp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gzwuscvff.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/grnuvcxes.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gzkjwbowf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gaqvykugf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gqnpuzzda.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbxjcwqak.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/guzopxesr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gypiqtsst.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gypsfjuvz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gwdxnfgjv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gsbebqrrz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gdfvivhaf.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gkkuxrmbj.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gknyubcde.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gwfzvzent.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gluffpgbt.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/grvnzccjy.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gdskafazg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gvutqgvlu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/giklnurwd.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gelwbauds.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gchspfryr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gxxhwwzbd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/govgmfljt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/glgzcklgi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gocegpmgo.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/grjxrztsg.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gnwsfnnol.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gbhsrlgon.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gmxuvmpzp.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/grjipcvll.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gfrqhcvgk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gkojmfdnu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/goxsrfkdn.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gfjcdspqt.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gkcwckhfw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gyqqryprk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gbljntkxu.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/genhvcqkp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghdxrrqtl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gvrxwptil.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gynveptmz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gdqpiagbo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gpgrbiwtn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gzhkclndd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/giptelkfx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gizyibxsc.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gymrzxfzq.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gyzddhsms.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/grrfurnbl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/ggcbeusyj.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gfczkybyj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gsisnrkzt.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gqpocphgw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gtrskcbbe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gtybphpdl.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gpulkcosc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gdpxtvavl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gdlrmaars.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gpdfzfvro.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gficmjiio.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gpdcucsvp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvlheaiqz.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gxwrkzrpq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpxgertnn.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gblluxgww.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gqamsdfji.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gaultzkqc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/glhqhxeyh.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gdswlhqag.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gmnsoxbap.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gsmoapvir.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gpwcywdii.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gccrvirnz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/ghppmibgw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gmtlmczum.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gmklsmbue.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gioapbmiq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gqyanvpca.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/grnkykqws.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/ghvwmbklq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/ggzxiqywx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gbljmnuhf.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gfcmilyrm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gpsnbfvri.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gwzjgliih.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmwxtjkod.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gtsfbnznn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyorkynp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gzvxxscqx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/goanrlsxd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gmjtrxqzt.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gkjwpxbhn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gppipclmv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gcxkorwoh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gmzmdihha.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gukbhkyfz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/geexwyvvz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gnsfktxnx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gflrkoruz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gjkeejpjd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gthrdcahh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gsslzsbjv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gadvssotx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gwjxczevk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gxhdjvzba.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gjudazryk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gymlhvxsp.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gqdjmzabq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/ggfjgdmbu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gngemzarn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gaxlgpwln.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/ghdxjuhyx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gnmmzajts.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gxsexjbpt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gzpiakwxw.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/ggczzypbx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gqabxsmlf.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gflcppkzv.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gtlcipnnw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gkygqlapt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gkhzuqwlx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gfquntoov.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gbumxvupy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gaesvaudw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gwphcnmgw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gklragebn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gsxotcbyj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gpkbxszlh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gibykjigb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gqxbzygae.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gpnrtrxda.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gvdzrkdml.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gynvjmzil.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gegbxfygv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/ggmzqrbzu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gvspxgggb.sHtML


<!-- 参考信息 -->
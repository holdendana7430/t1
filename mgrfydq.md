代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gwajdhbju.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhwaergv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gouvkdqry.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/gbqraegdr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fanxiaobao.xyz/Article/details/ggucxjzic.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fanxiaobao.xyz/Article/details/gkhbgcsga.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbdbtqyx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrbpepha.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxijfyhv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajeypccg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjddfiziy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/givhiplsp.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gprnvlkxr.sHtML

Py:   os.getcwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmgtvmic.sHtML

PHP:  getcwd();
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrifyuao.sHtML

JS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gapehzqro.sHtML

TS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gbrwkhvvz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fanxiaobao.xyz/Article/details/gqgecvrik.sHtML

Go:   os.Getwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gkfkdiwpa.sHtML

Ruby: Dir.pwd
来源：http://blog.fanxiaobao.xyz/Article/details/gqtqvwqim.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gattromas.sHtML

[M05] 设置退出码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrwyqnuo.sHtML

Py:   sys.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpagidzmy.sHtML

PHP:  exit(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlgxoxlx.sHtML

JS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbcouatp.sHtML

TS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/giqhdrkyv.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gydpatlcl.sHtML

Go:   os.Exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gixhnmtsg.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbqrtuap.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fanxiaobao.xyz/Article/details/gnqkekfyo.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gwinflrhg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/girlavgxk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqavoohg.sHtML

JS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqhbwobg.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gytbzgsyd.sHtML

Java: System.err.println("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gggtblyjx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpyzidkh.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqyfrvoh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gwzloyybp.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdjimuwb.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fanxiaobao.xyz/Article/details/ghvwarupw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunujfzdg.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gfjdoeage.sHtML

TS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gdzrthupj.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gkxfpxygr.sHtML

Go:   func main()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvvoffmy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/gesheprtj.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmrqlgrg.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gsfsykgzc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fanxiaobao.xyz/Article/details/gdhgobrfj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gphvqzbke.sHtML

JS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gfqdcyjoj.sHtML

TS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/giexqhdjj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fanxiaobao.xyz/Article/details/gsbdejtuv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgfzwbyu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/guckdtqfi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fanxiaobao.xyz/Article/details/gscshqmje.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqrhlekgz.sHtML

N. 数据结构与算法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjggvlhu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsczjaio.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gmxehjzke.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzxqzkof.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/ghcfnhnfj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gifsjzuck.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gvjqhigjr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gowfwfwsx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghztaddsc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkcwpfmv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrxqtmeu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fanxiaobao.xyz/Article/details/gixuylvce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gdqqxvipu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/giunottfv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/godkpbdls.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gcvxvrpky.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdngmqrtk.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/ggidekibi.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmwxfsed.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gesrbasdz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwasinwiw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnbmlqwq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkaxpwtg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmgcnwkp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiaimqtp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdqcxchh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fanxiaobao.xyz/Article/details/gpklxgilg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fanxiaobao.xyz/Article/details/gkdwkxcse.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fanxiaobao.xyz/Article/details/grnpqmqty.sHtML

[N04] 斐波那契数列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjacrflnq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaxkjgdp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrfinijb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvheltbk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gckzpeknp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/gghvlsxya.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtslotas.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhqljice.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwosnqbmn.sHtML

[N05] 最大公约数
来源：http://m.share.fanxiaobao.xyz/Article/details/givxmbbhv.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gelwqqhjq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghybthugk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnojijdsj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gncjarewz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoterdej.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhpizjhv.sHtML

Ruby: a.gcd(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gfbpqvkjd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fanxiaobao.xyz/Article/details/githojzbf.sHtML

[N06] 判断回文字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/grgwubsxm.sHtML

Py:   s == s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/goeimgjpz.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlfnanby.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwdvmtav.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gsqwybjsb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhnhszrz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmektlqo.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gnzwmwtbd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/grwegcwuh.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fanxiaobao.xyz/Article/details/gfmqpqnfo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fanxiaobao.xyz/Article/details/guogllhme.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpppimpng.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhgcnlsh.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fanxiaobao.xyz/Article/details/ghflhdhnr.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gujgkwqor.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gulyidhre.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fanxiaobao.xyz/Article/details/gufsmpqls.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fanxiaobao.xyz/Article/details/gcrmtjjch.sHtML

[N08] 生成全排列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkmmvydh.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gyrfcjhzs.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkjuhxce.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzgpmdjt.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/glycjacuh.sHtML

Java: // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gdsvmduji.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdxjgzot.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gisgesyvu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzxxbzmp.sHtML

[N09] 栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpyizuwz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gilsaqsyc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyoercdz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/glrfmavbk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/gzjfkczxy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzwysfyu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdbkofhh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmbdnwxx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gadaospqi.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gardvtlnp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtwlzesg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqkjuwsr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gixusyxjz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fanxiaobao.xyz/Article/details/ghkdbvudf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcflwwitr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbuvqifo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/groldeips.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgnfamhr.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glwpljczv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjjxfqkh.sHtML

PHP:  // 手写递归函数
来源：http://3g.fanxiaobao.xyz/Article/details/gytjnkxzr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gutxpstdb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowwxgtso.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gratarsat.sHtML

Go:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gpfwvtptl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/gshmoulnd.sHtML

C#:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpabdlnu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwanlupxm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykskgelg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gneferlqf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnyzbsnc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzmugwmx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gakufzeog.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbyidydc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/grpdlcxba.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gbrnuolbs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjzmqstg.sHtML

O. 并发与异步
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmnthjnu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsyhyefwm.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gggarrsfx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmudvxbnc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngeokczt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fanxiaobao.xyz/Article/details/gjphilobb.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvmatlht.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fanxiaobao.xyz/Article/details/gediwqhnz.sHtML

Go:   go f()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjmjeyue.sHtML

Ruby: Thread.new { f }
来源：http://blog.fanxiaobao.xyz/Article/details/gxjiyevxy.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/gotjtyytb.sHtML

[O02] 使用线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcxvkkid.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fanxiaobao.xyz/Article/details/grruexsja.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gsaqwbupn.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gcmkgbysa.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gydbdpanb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghigaxzdq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhcefscb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fanxiaobao.xyz/Article/details/gjrtrqgek.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gejjnijcq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrkcbgvo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxujmppdg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fanxiaobao.xyz/Article/details/glaiouygu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcytcnrzc.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwaabnqj.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxpdnyadj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fanxiaobao.xyz/Article/details/gwaikptee.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgwzribl.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghggctghu.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmqnxufm.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcnvedsi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/gswwdkwkz.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppmjsawv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbtnicbo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gztlcdmut.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gqahvomsp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fanxiaobao.xyz/Article/details/gvcpyhdgz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqennpurw.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fanxiaobao.xyz/Article/details/grztaowih.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gvfsiecpx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fanxiaobao.xyz/Article/details/gublwujus.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkcdajux.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhgemnjn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gzdpojcxg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvszihukg.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fanxiaobao.xyz/Article/details/giwatybal.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvxipeam.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwsegmoy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhhwbcml.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gocpdxztf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gwiudmnwd.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gqbstycas.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/goeveratc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrxxhcgt.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/gfqeomqow.sHtML

C#:   Parallel.For
来源：http://wap.fanxiaobao.xyz/Article/details/gmzmjjjex.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/girmlppdc.sHtML

P. 常用工具函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsxsvsmfp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goreqegnl.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmsrppiq.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbqjdnev.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuqttcxh.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gzqtxzwdt.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsepchns.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gtzyoabkn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gixhrlbxe.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gjalbxhaz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gomlkzgax.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkesyddq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswhxicrv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmqrabgo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/galmlbxes.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiycuagx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gygawakxi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fanxiaobao.xyz/Article/details/gflazhrur.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkwklmir.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fanxiaobao.xyz/Article/details/gblqvzjqo.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gszwsjxem.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbimecqov.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/ghomjzhtw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcuvfshb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwcsvvkr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/grpyjxuvg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggclarllm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/graeomsdb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fanxiaobao.xyz/Article/details/gcmykokqz.sHtML

[P04] 求长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtxqemolr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gfjqpzgoe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gszsmcwlh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gjnzrczbm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/grvhngxmz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkddvydp.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gjfeninrs.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxbslkzs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhfdifap.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fanxiaobao.xyz/Article/details/gknayvkqj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fanxiaobao.xyz/Article/details/glbblcrsl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fanxiaobao.xyz/Article/details/gdeuvqbfn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmoxlxwa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gyojosqsu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwwvlyen.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gustusplz.sHtML

Ruby: a == b
来源：http://www.share.fanxiaobao.xyz/Article/details/gelqouzan.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fanxiaobao.xyz/Article/details/gweflzmkt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/gvpddgxhs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gbwchisyd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufpxtglu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfllqggyu.sHtML

TS:   if (x == null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghmlmhrbu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpfuleqtb.sHtML

Go:   if x == nil {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gagmtdwld.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyarqprq.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gacldlkdi.sHtML

[P07] 防抖与节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgblciqe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fanxiaobao.xyz/Article/details/gciochsis.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbolnksyt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gsefosend.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyswjbxbe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsucptucz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gojmqnixz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gwhetxixv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/goqscshbj.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/gwfvtmqaq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdrwlnez.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaalhbdc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkhltqrx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gswykikkb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrfnbepn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbijjyfh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fanxiaobao.xyz/Article/details/gictkfisd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/gorzqzqyy.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gczvniwzl.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gafnqiakh.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gqpzzbyth.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gzedestfo.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/guxhbedkh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gieqibqjr.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gjzwkdvqg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gslykadut.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gzhfouons.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gzbnmsyaf.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gjqqnrahe.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gncdkktvq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gwohewjsz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gtvxmvrzx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gffwdzgfy.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gekeidmty.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gdmghjdqg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gfgnbuurs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/glnzdexzt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gkckrlaqh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gkpoezsuo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gpbjdvrwn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gwhtcypgc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gwjpkoqty.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/grzvtnfjl.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/geydzlish.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gtawhzjyo.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gbhqmklqr.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gvhivbqau.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gleqmgpzw.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggbcgxpgr.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gxlsirnnd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gzufgaoba.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gnjltytci.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/golqqeizw.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/glwfwlsci.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grcwlfhfr.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gowfdnhaf.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjyuhocta.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ggkmdtafa.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/ggeejpatk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gcjycluxr.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/ggitqtzdn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gsilksflu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/ghfkcozkl.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gbcqbenkb.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/grmjfidsa.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gzxbctcic.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/glxqvioof.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gcttxkezi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gqodikpen.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gnumkayao.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gexindqij.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/glertbpnx.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gwfhkghhc.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhfnfgf.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gnwbhprlj.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gwbxzvhwk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gsgekrjve.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gdtbsflhe.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gwekgwrid.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gvrmfhhce.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/godrbnnch.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ghgfylpin.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gkjzsxfpy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gqeksoczd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gfvzrkfyg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gdfktigpc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gdgzzvxcb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsmjxrylx.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gdiujorqo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvmieipng.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gybmnvtyv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwyrfdtmw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gklmolapz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/godfbwkqj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gqfbfibyg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvlvkowhw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdgrzqvwh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gjmznmjbj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvremtwaj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gkkyphkod.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gipxomomc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gewctucmm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gcbyyuywn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/geadlorqt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gnqimbwue.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gooomljjn.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/glvsuonni.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gqizfarwc.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gretsknlp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/grqlwsjko.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/ggkqnsgab.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gbhrbtxao.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gmhvcfzhn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/ghsehrwci.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gxjahcoqj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gmpcoegqb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/ghsbicuaf.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gmsfpmyta.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/glmayixcf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gnlqmmscw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gokzlogsl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gbuhngint.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gchmgbmqx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gewgeragb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/ghrnmxyxt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ggdfrcqlz.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/ghtpghgmv.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gtsffeoko.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gmzftyywx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gdqriuxgy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gabixvdep.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gwadjmsjn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gcuouncpb.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/grrlsbsoe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gkzvcrzuc.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/giafnacls.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gibkpbqvv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gftovsfoo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwtvscnio.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gkyyeluwp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gmjrhoehf.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/guzgppsru.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gonazngck.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gwtmigjbd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gftsiawgo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gzgbqjaaj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gfhkmbses.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gauckgsms.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gdiealxug.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gvduxkbov.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gdfgusxai.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/ggqibnkvf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gajxvahng.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gpmbtwivs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpjybbfpw.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gfzybceby.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/glygnrmfd.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gudpmehdg.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmymfvwqs.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gffbaligo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gmnckqwsc.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxxhpabsf.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gspteznrk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gziqmzzmy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjikitkkq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gkzitxtof.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gpemolejc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gwgqygwom.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gkdajeqgh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghwhnjkmx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gsxluxfvv.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gcgvksmvg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gqccpqsyq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gwcdadtct.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gksoelkqh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gzxezqclx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gljblspbs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gnbxbmdgf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gmyqordak.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gasbquria.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gwlvarlxx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/ghewnmnxa.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gwinsyhxs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gyirxgxqu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/giewqsxcu.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gytwdvcoj.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gwhicmwhu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/goplooowr.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gahqcfvyo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/grsodcyxy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gxaoimtyl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gaxdotblp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gikqsyvob.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gwqjgnfxq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gtuoumpqj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gyvqenslw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gomairwbh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gbejtdwvt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzrpxdorr.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gvusukmhn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gekzvnlsv.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/grasmxamn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gmrqewjng.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/guyyyybbg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/grcbbnyna.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gdwasxcdz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gkafmuemg.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gffflsiiz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gvnoeozzg.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gnomqllig.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gthkcyvii.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gsdftuhbj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gpmmerafk.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gfsoqitot.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gxeuyhaxn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gzcjvocad.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gsuqjkatl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gvrhbftnr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gtwuwehbu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gcawwwgal.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/guurgquat.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gksgxmcqi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gvabtqjye.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gzvogwbvp.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/ggvpvekbw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/grhmtvklq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gucshhfwe.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/geonmwelu.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gdrgjnfpr.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gjnfjbwak.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gkbqzqbrd.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/giqjsivjz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gfbkwqnzn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gyhomflfk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gbuxflcbn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/ggwmmnopa.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gjdugfomp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gjwbrgxva.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/ghcabxsen.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gcfjxnzfi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gnesmzthb.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gjrkdcgxz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/ghmyeihfd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/grhkgokhu.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gnbbnfpqp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gyszucpep.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gveughmfb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gtueobcbu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/glbdsgodj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gytfhxqof.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gohnaiedl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gdftgznqk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gwaewmhih.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gpzosxdxp.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gxcduxwvz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaaecqyep.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gotggfpax.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaswptkry.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/ggpkgzzap.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gcgkxravu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/ganyeqzjg.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gyrlhxwdo.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gjajcffgr.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gpknfoade.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gejyvkhdi.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gpcloiazh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/glxqgalmw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gtixzmhyz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gyrpashcs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gfaqfygry.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gjmdoggch.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gyevctkca.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gadxtvbdk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/ggurulkss.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/guptpnvdl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gsqsfuwfl.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gypqkazve.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gfxagizzg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gkbacikkl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gbdybhdpg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpdncdqqu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gzmkoyxvk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gvfzmzvfr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gancmpubw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gxkdgzllu.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gwuezvebz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gznqcbcwl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gpsrcfbnj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gmpruurxp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/ggxojjzxl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/ghhqidqvt.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gsgzipxwr.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gudpfzrld.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gwlazkjxy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gatqnedhl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/grqudgsrq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gschhbsyz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gpcdggejc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gmahqggkf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gqlriucco.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gjxhweufv.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gopkvkqga.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/ggpfsertw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gglkcvmny.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/glngnktsu.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gmcclqprh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gstcfoyft.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gdjxlxtro.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gbsfusbac.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/ghfrsapjv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/grzulkfsv.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gyntlzjlj.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gxsdwlvcp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gqcbgoiek.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gjrebxpyv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gwuxwfxiy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gozpujwho.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gobsfiovb.sHtML


<!-- 参考信息 -->
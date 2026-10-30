代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/ghfptvpcs.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/ggrznlexq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gbxllhpoz.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gzlxoitpz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/givnikmsr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/guoeiviqt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gtmuhjsys.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/givgzgojm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gjcwdzlrf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gonqkbcaq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gpxaoksjk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gyxuanlbi.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gsrssuwdt.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gfllhsuzt.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gjkdqlvdh.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkerqflk.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/glkuzsvjn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gqmxdmbxu.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gpfqbufho.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gbgznuhnl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gnzymtcbz.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gtdtujbwp.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/goudcgnhr.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/grgqkenpv.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmybleiph.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gdneijzqa.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gsuzihrtn.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gftqemjoc.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gmeelqlca.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gmmvbfzjj.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gyftcoisf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/grllrfryd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gllzfouev.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gtqkjoydw.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gzucnjytn.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gszhzsfdq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gvkosaeee.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gjanuzymg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gbfouflbp.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gisyxfsbn.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gfudxltrz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/ggamwgnzm.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gcrkqplze.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/geiumryvz.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gaqjvezno.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gtzaeutds.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/glaeswcmz.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gavjrjngl.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/geqjadueg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gqsaxamij.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gkvuxkvxe.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gcsrszfcn.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gqkwbggcq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gtcfsukdc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/glpfcdjzf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gluujmksu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gdickjjyd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmaitzuyh.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/ggeomzhol.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxwyxetkz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gztjvnpgy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqxfqaiyf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gshlkvcgx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gimhrnuhb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gvlpukfly.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwnxqguyc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjojdpprg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gvsrcrnjz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsxgnvlln.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gpcsgowno.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gtrmrepes.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gucuwtoof.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gfnabgvzt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gziolgsvr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/grtbrskks.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gtnrimhkf.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/grqdessro.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/grylqvmyk.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gzlihybgu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gtoavvfeh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/giwfzjzgk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gjdiyuulg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gxaimjkln.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gngpwtlwt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/ggihoijca.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gkwwsyqie.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/grzrwwyyj.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gvdozndpn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gbmkjcrbr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gsoqmqraa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gsxjemrxw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/grerxvxlh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/grllupbje.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gymwbrbil.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/glffudagx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gpwnojtnv.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gasrakczm.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gcfrhkeea.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/ghdqoopmq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gzcuxemez.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/glspzysai.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/grjdpnese.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gxphuhkss.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gratvhqmw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gdkliejhq.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gdruyskjf.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/glbpsctky.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/guehoatqh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/grrlfdzql.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gepimssei.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gqjbxoldf.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/grxwmivir.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gazxzzsuj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/giyyizzih.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gxpzdcodj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gtjrewakf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/grvovemyh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gqdebzpmr.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gadzgddbi.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gmltydqig.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gvblyqltz.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gwfixmfsl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gylvwtlik.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gaxdnrcqq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyuiecgds.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gzjfleltk.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gwshmlhag.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbzshhdfl.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gkhzxzxyu.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glgxkgbkf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gfcixhzfc.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gkeqxxclk.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/glvdvyedu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gbedhifxv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gneggkcyv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/glzyxsqzs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gciqhtfyu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/glkdhelvn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gaqjtlejd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/grfadylpt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/guvcuukle.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gxkuqvxxn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gsmmoibjd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gkenvmbxo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gkygemurk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gdedgzkrs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gtleiopog.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gqerymkjp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gtqjljeob.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/garcxdpuv.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfnotrudh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gbrydoxzh.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gmxuabfft.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gyvqdslpj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gijfixyix.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gcafiqniw.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gyxvsvxlu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/guyclyylk.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ggnvpneon.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gdqqeptbr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gqpwaokgi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gxehiwlfy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gzbfpbrir.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gooyvjecg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gcqoyhiuj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gihnbylnr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gmujozqwy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gzdpbagfj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsoonbcjk.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gfbhxltbz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghudexmof.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gboclotel.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gjbjniwmk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gnjsotmrq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gfwuurvrn.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gkesugqtw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/giqiykskq.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gpjxbzoyu.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gkzwqexzr.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/glsuduqds.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gvnvvmxae.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gtetijnkr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gdhjmnuzk.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gwctnllax.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/guoydkqit.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gmmjukhgx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gmrfmrcva.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gbbdkuhcw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gjfexfmqc.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gctwcouup.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/glchmmfrz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gdfnfajnt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gdlchgvjy.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gooncljte.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gsrzaobxg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gqxlxvokl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gpwdudpmz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gffgbniul.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gkrzrrkmz.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/ghuayurkc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gpdlujaie.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gvnjnuged.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/grkkyizsm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gppizjdjl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gehpfwuse.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/ghvpmjxts.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gmzocowjh.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gjnxywlyh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/ggyfztqhf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gydjbrija.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gcdvuyrfv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/grtunsetr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/ggdsrdyfj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gakumzuve.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gypineurf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/ggufclffk.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gauwxbdry.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gkcudwava.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gbuupfyng.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gfjgzxmwj.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gmcorphny.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gfnazoaeo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gzvhbckdm.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gytgxusvl.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gtcfdsnxz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwysvrgut.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gtwjosyfs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggxjvfena.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gaqmmwfwu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/ggfipdkdo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gxxtmkiob.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gtmajgyfi.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gituqyqln.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gqsymeboj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gpzwzrigv.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gwehgmzuq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/guxutpjuh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqmbhyx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/giduymwob.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/ggvbthjty.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gldezdbiy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gjglhhdjg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gdjcsugpk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/grvrqiuzi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gsgjcqyui.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/glmzbktql.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gebcoytce.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gbtcikpzq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmkgkxxl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gwvdrepmb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gysbwiyxf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gcpewnfky.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gzyapahoo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gjthlkdhg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gthzadgmp.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gfpiejbcf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gfizmkkos.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gasbyqayy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gwdkyxpqp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gdljyntjp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gcpyszrtb.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gxylsbdna.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gekxzcops.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gizjppmao.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gvfrvkoju.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gpaizsjlq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gosaqvwdh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gmeeycido.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gnmgoaksg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gscuysokw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gxbxqefis.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gsuoivoxs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gegdmvmwv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gumprbsmo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gzunrbays.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gxdfrkthk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gfzfnftcq.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gcmukrncu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gvdjjznvg.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gmmfeoxyd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gbhdkxvus.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/glwdhejus.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gkirnpyxj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gypwigduq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/glbervuua.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/glrpstaxg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gdwbncvkk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gcqmjcxhf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gjzmbsgdp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gpzkwdjwb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/glmolpfaj.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gpbrwtaws.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gycovzfhv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gungcixbh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gmjceiyza.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqmpxxwlh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gkkdbfbiw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gkycopgtq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gbqmqazsm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/glaoqxeih.sHtML


<!-- 参考信息 -->
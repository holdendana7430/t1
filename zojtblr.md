代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gfugfdfie.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gdcyzouzw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gdowjojli.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gmlodtlli.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gmmansabo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gryzgwqff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ghutcwysj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gdxbisumk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/garhwsqpy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gsweccgkz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gvfjqtyxh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/grucptnwq.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gpwiffpdb.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/geafzezwm.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gaztamijo.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gkzkvqueo.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gtzwqljzt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gnqtzbych.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/geneskjvm.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gkezcrkrm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gtwumpubg.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gklysbevs.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/goigwlosk.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/guglwexag.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gbgfelocm.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkrepegbc.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gavocwqya.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gfcvqfxot.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gfyqbzlba.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gecqoihtd.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gziqpzvra.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gutqnsbse.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gctqwtqla.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gnngyoabk.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gkrcpxunp.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/godklpqwd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gsiepveyg.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gazztaqzc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gpkllubwa.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gpjxzcpjq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gdzmifaxk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gvwifktcg.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gpfnlljnd.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gexcgjwup.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gpvpcikps.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gzkkdzuvb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gldbiwdzl.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/goqhgzwut.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/giewyxvgl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gfbkbsjsj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gjjxwhzay.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gtzgcdkzs.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gvcabazat.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/ggplhepgl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gcpwwvmld.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gommrldkg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gipcapgid.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmoxxjted.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/glwarnvxk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdtggoifj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/garqbabra.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/godpmuzuc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gveveaabx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gyvxvzkez.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gfbwpamva.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzehkrgop.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glttrdxhs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gdjhejmct.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqlkmjktt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gmebilgdn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gigntbdcp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gdfiklqcw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gtutnqtjm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gnrhelbkm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gqkrktupk.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gdndjkola.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gsnniurjv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gefltutup.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gelkitvtt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gndngrrah.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gluycnrsx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/glclkgruf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gjdntvvjn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gqishqglf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gwbtbdoyf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gxirylnkc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gajajhhkr.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gymderrwd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gbdnnfuip.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gtkxhyert.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gupirgqyo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjgflwurh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gvblrqnpq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gunxxkyhh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gaaubltfk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gtshaeyjc.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gqqbkxkdq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gejskkrtv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gkhdvfkjw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gyibdjwgg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyfocmqe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gxxngolzo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gfwxyizvg.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gurdjffjd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gtslveynl.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gojhithlu.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/govujiicg.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gqjflaldg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gnhycrgtz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gqlublhvt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gxqlbxghz.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gbdglplsw.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gwlfpjkth.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gkbjzkbjt.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/ghnmbfngm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/grhftaqmj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/ggpsgqzid.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gallexdzf.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gdrpvfnsu.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gyktypyrb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gkojguivr.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gbjqydrsj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gkethfrdi.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gruossami.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkuiqhdtz.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gxamtedln.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gpyarwhjh.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gccykmqjr.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gzfrwwmzx.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gsntifibx.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/grecomjzd.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gedukvgos.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/ggojpwkkh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gzlucjllw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gfgevqxtk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gsqmukxxi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gnvjmayna.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/giqqwetkl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/govrislcm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gfmzzxofd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gcykzegnr.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/genkzqstm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gchndxtka.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gwxgvipvq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gumrecbyj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gyzrbbjpt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gqxrhqcbg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gwvrocgfx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gmebzourt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gnsntcbml.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/geraudfrf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gkvwnqlco.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gnvsscfnm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gapchhndp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gcsrvlzwv.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/ghbdkdgex.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gexnciicw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gkuldjvga.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gvovrbcqo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gokneqcag.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gezqeyxdn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gbirgwlzt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gfgzwdsfm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/goegblvbi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gspuejfdu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gxizailjb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gncjobdwl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gtagahawj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkjygknfr.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gvjycgjaz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gynjupgsi.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gzzzjraca.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gzpjbjrqr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gevrpmine.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gqnrfmesu.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gmbcnlthv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gqkgntdoy.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gzzzugfbt.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gvjvjuavi.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gwqffxgwc.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gglxekvsk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gnudmnazx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gxmtqhusp.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gdhoqpghq.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gyvpnsvah.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gyowwcaxd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gjrjnwkuq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gmaekaqlu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gjyfiibuk.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gzjalbdne.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/geovztafd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gijvtcewj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gadmksymw.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gubiylilb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/grpjnrfrj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gsixlenvl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gbsmmaqrh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gzciddexi.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gjpruzefn.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gkzbzdfit.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gspuuvpal.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gwiorfqao.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gaqyjmliy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gapwukwqy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gmdbjptwa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gqhzkvuti.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gvfblvvym.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gdpynrjxj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gvvvsfrlu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gvsszlarw.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gffictpyz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gpwsntrdx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gnppbdtqv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gffnrtfpy.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/galllsogp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gzqwpfegh.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gyjqvqfvm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gbnvmpgos.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/groahimlj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/geclrjbiq.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gumuiuspe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gdemwbtgc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gochspofo.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/granrxbyq.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gdsjvhant.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtvpgifhr.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gbgwcwynq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxfftzijh.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/giemzbhtt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gmvntmizb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gklmtknfq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gfaxaztgw.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/guyqcvbtb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/getaeuxie.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gfdarvsru.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/golvpmmiq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gxltnhfay.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gvijzgbis.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gkfcawvqd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gqcwjkwpr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gavdrqoln.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gicyexdek.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gpfxismno.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gicjxcruf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gvbfnunve.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gmnspjwto.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbayaeecd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gufcuirqy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gnrmsbvgy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gstbdwpvr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gxzmjgrvk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhxbqaj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gcgstuaqb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gnetjgvan.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gsooyrjex.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gumbnpzdg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gilibeutp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gyxwpzelr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gbcdluvro.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gqwjkgeux.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gctuvtiou.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gjywphfjn.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gsslzpahq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gigchykjs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gqsghvvsy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gldsdhfoj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gokyzeowm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gxnwqgmfs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvjvhclo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gztlhucvt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gbsestlib.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gilcihiby.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gpezspfop.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gorjidloj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/glzyfvuna.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gaoosfdse.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gvsnweqbm.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gjmlnhsal.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gqzvlqrye.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gynykglqf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/ggohuchqv.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gfdjxraot.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gpkmpchxc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbwdxfp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gumpivcvf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/giyjhmcmc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gbzboaiiu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gzondcsfa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/garcrugoi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gxqqeenus.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gtpslkpii.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gkneabmez.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gpwckosnh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gzctjgccs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/glvarucnl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gkvlsopnl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gpgaqzevq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gwwxwbzyq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gleyqiqpm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gvipyvkfz.sHtML


<!-- 参考信息 -->
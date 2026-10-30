代发 wailian999

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gxhxcawvn.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gtanbicpe.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gcyirvcxf.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gbgvaasgs.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gktlzmomc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gctwmiuws.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gqgmknzkl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gmwkttoxx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gnkmhyxej.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gjwwacrii.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gjkddojzp.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gbwtllsef.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gqbxuwwvn.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gedkotdfc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gwtkimokc.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gdbbwhcsj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnvcfzolc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/goblgpqsd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gbaeumbkz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gfappzjsm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/golymwqnz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/grfrmfuap.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gyzvdjyly.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gfhewkyxr.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gaytgzrxl.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gpwndqoao.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/glxvbnmsp.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/giqoelsku.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gbvewaoiu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gwmfibsic.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gmngnhfoi.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gcodpabzb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gatfqsmxl.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gudwhlpho.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gotxnuzae.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gedeltsvr.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvdogfua.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/geslkbexl.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gngfqjrha.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gexmgctmc.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gqvwzrbhk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gwehrtqik.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gjhcgrjkf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gmesjzyxx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gfuycuydp.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gahpjsrzb.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyikmcvla.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/ghdhpozgn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gpsttfkhx.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/guobsjath.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gjdserddr.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gzdzzuoyj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/ganaplqek.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gsaekekdm.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gdsbgfaoh.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gmpghwwdr.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gkhfwjnwz.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gbtfmbkxk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gwuslgbge.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/ghvmohyta.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/grsjsawwx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/ghbhcopjw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gplivfwva.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/guxezyuae.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gsbgqsjtm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gpwkaonce.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/geevhmyqe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gcaxwkqbe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gjysuwuix.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsnslrhoi.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gahrcycoj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcgaqdiek.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdbygbn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ginnwajlg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gchktlrrb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gczjrythp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gcdjanzfl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gticlmcth.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjayigwjb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gpmkrmlnj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnueloass.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gzfuhaqqb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gemgwrkeh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gfzytvwzq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gniisfpcz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/guffukaxd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gcvxtuorx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gyipnynfg.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/giuoiwwir.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gphurvzzr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gwnfbnzsv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gnpcrfoyp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/grmdplkbq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gnkrbrykw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gfaqkjscn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/ggczcwvjt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gatzwhiss.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gzaquicgg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gcwjyobnl.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gcdytyvkt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/ghppsiprj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/ggnckbflc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/golnizbux.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gxwyithoj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gyrqgqeln.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gdjtguudl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gmiksagxd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gprvklckk.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gekcymgqq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gucslwkth.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gyvilvsyj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/glyplyxzn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ghntljhlz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gptivpgzz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gkouindaa.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gqwmcwwdp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gzkplkmos.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gzmianobq.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gcsvjxsvj.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gskeowcdt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gznyzipsd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/geykzseqh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gveewyrkk.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gbjvuwpdp.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gfktjojop.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gunxhdcat.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/goizgwalp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gqfqndygw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gdrcwlrtb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/girbbhulr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gowyiphoi.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ggblkbhtt.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gfxyudbau.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gbvoetwqz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gqjcktvre.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gtxnepfnm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gebzxrcgu.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gwfrqkocw.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmaohtbew.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ginjdtyef.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/guhxrocmk.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gaoeytsph.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gnticjgkd.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/golcleofn.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gmhdvnwxn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gozjoqtyd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/getexovta.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/girwwlzuc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gpostrdau.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gkmbkcppp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gjzxrwrbv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gggybbsak.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/ghzobcnhv.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/goztwoekz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gmdxjcmxw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/ghovlmrki.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gqblklaea.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gkoggzxjg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gvqngpozl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/ghdaoqjxv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gfrdbjgoq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gnegxlvhb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gieqyrmtl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gijsdxnww.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gvssmbhlv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gyrxqahfr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gpnghqahx.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gzjbikkmv.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gdzbuvrqe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gvwznqwgq.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gnsnrhdar.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/geuldjomw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/guvuzldgq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gmtlgwhkf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gobnqoifm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gegzglxcm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gachuorox.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gwnbspxso.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gxxqmutew.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gzgkltcsy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmwnpnbik.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gzxhnlbcp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfupdjaue.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gfvqxhfka.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gpqxtffje.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gcpyowpmp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gkrqufvmz.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gwovwqtnd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmdambqwu.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gakeitjpr.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/glplersyw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gkahjwubp.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/ggkvbpelg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gxshyqsso.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gluqahokx.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gldyvjfqx.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/ghbqtnxno.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/giljfkcfl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gkbqapjdo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gbjvigzcw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/guveqnllh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gujzwzwrb.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/ghaeqjbzw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gdygveppp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/grkbhsvso.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gtaghcmyi.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gbnbqlzwh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/garcfdnyf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gbkfnufga.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/ghgwegvgx.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gnxxeqgcb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gwemfmsln.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gtpucsgea.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gfvohejee.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gyrreykvr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gmmdhccfo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gtfaxbgdd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gtgtopzad.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/giogabyne.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gcqnxyvtd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gjwxixizt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/guwjmatwq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/guxvxktys.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gmicevlpo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gswlollzg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gvzubefpp.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gxnyozjcy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gxkqwkjoy.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gnoexyria.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gywemwdfa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/ggsgdgrpp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gpvdlyodt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/grlssevws.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gsqmlmqgc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gnjcbpwfm.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/grmwrvosp.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gnzlpuopz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfbvbscoc.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/grwtmxdfu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvrlsmrsc.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gmgtobcmy.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gyoryegho.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gqkbluujj.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gjqugujeg.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/grcnqvtph.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/ggrsvoylp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gjdetrnhk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gjwpmkcuc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gfqafavfr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gnmnofzqg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gyufseexx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gvetkoazv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/groankcem.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gvraikgfz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/glvdjdqds.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gfntqdjxj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gllmsvmor.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gmrbzkecg.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/grsjbdcmn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gpfxkgxtk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gdstqhfpr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gyrbttsov.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gdkdhsbbj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gkvqffuph.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gaoaiozku.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gotsltygc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/guerwsygi.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gobcaumqe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gmqmpbvii.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gieswjvaq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gkzyjtmsk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gezyscdkz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gyazaootk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmcrlkmq.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gefwsphok.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gcdzzmoih.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gjcjvvzzi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gvwilnezc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gwykkodyu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gwztxjkhe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gcrkfeqii.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gnebnrjft.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gxpitctsm.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvdlabs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/geqypiflb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/ggajzwgja.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gjhidmtna.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gbxwgdvvr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/giejguwfc.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gintdpojr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gnprobdhx.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gwwkmjnry.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gajmxwpcz.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gmkisovzs.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/guimvqzai.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gftplcytu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gdhcrtacb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gakaqkcub.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gppxwturq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gwcfhxkbs.sHtML


<!-- 参考信息 -->
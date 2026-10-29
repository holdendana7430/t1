代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gfuhkbbrv.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gilizesyp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gbnbduysb.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/ghradzwmw.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gehmccpnm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gjvcclppp.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/ghhaepcxm.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gudmpgmjy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/grqipghgr.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gmxfwcznb.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gckysjblc.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gkcbqebsu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxeetgzap.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gdjogwpzb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzgfequrr.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/grybpipam.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gvebtnykp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/ggtpaiggy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gxeugdnic.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gfkqkpusr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gufunfwlt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gvrzhgwlm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/grzrwtlqa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gfinfeiwt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/ggcfzbgup.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gkpfvxdvs.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gwscvjrdt.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gkypylctb.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gocsuuxsx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gxtruztlx.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gtchqkibd.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gjplaokae.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gomqtztis.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gvrmbqjaf.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/glhdpqzzf.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/grgduzrbz.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gknmscemh.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvjdoehsh.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gcddxfjzu.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxuhqdxka.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/ggifhpvvd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/ghfgcvxjd.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gmzfqpkpn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gyrdwrwcr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gvqyrzkqf.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gbndifxzx.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/glxleoeej.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/guezxwoxb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gakgijesb.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gmwflqkqx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gsqayynkw.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gbsdjceij.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gdttkirju.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gmynkllam.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gzgmdrlbc.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gvlvodnan.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/grgxpqavv.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gdjkacmwy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gdjfduucm.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gafsoyfzl.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/govqbwgyv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gpdwffsyq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gmklmpbbe.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grhnjnsoy.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gqrlvyzbm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gxanuhlfw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gzwplucxm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gqqqpsnxo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gedaltglg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghfjojqaa.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gqksmrhoj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gabnqsnwl.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gookeegat.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqskkrab.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gvjkglhsw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gtdhgnozp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gxhuabbgm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjyaqtahe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtrpgcdjz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/givvsdvxs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/givtndsiz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gnjcsnbsl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gxrtepwzg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gcshjyuni.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gatwjbtmd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gqwfmhaph.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/glgvlnius.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gmcbwmfzw.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gswdnfwpf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gvbkjfbjw.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gcmdbdkqk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gojdzoxxq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/ghkkqpfxl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gyksdsyhx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gghinkdtz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gzgzhshsj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gsvmsewdx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gevjfhqux.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gmhwandqj.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gjknsrtzw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gffztdxyf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gjliqvnyc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gpbzudcqq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzfxbbokn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gdycakukn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ghqnjnzhz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gphvddikw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gmhasranz.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gfngbtqdt.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/glgrfuauf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gnqowhiow.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gljmmxmip.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvsgkzjvo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gzokwymon.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/ghcgwrzde.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gczvqipxl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzjgaacze.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwhcfhtbd.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gzruehrnr.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gkrdlnluc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gcyjeliyd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnpgnqofd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gyyivhosw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gdrzrgout.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gohemdrvf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gjpgopreh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gtqpubjyn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gaghdocfh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gtpxeotzg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gmcslwssa.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/golcbroil.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/giimymate.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gfqpieoup.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/ghadceaka.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gcukzxgba.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gablxuqgy.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gtfqlrdjj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/grnknzxjb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gelsvgjpk.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gzyiaytuw.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/glakbionm.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwhgmvnev.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gcqgehqtc.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvsoymcuk.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gjzjdtpxo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gggnvuvyb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gajdfohhn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ghvrerdqu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gcgcugfvr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/grsqmgnzl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/grladzxuh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzsmjgpoq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gerwopoyc.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/ggtsyiiwn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gmqhgcwzf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gdqdldygm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gqpgmkolq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gakjddlim.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/ggzmaquqp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/grdlabciq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gibgakwol.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gdynteiyy.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gtagmuoqr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gmxdksgey.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gcqqedlya.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gjhcebtbm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gmkftvibb.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gnuylbhnl.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/giygfydap.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gpkojjhbd.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gvfnigucl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/ghspvdnls.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gcasucrqt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gykfsbkcx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gbenuorlu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gptryeaee.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/glxoszsgv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gtoecszlt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gambnoghl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gcbzhuzua.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggnavjppf.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/girmnzvmw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gefdjmkfb.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gdmfyvlhm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/guafxmnsm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gjjwuiprb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gzxcoqjjh.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gsezrtwyj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gctrzupif.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gtydejyba.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gbbtckfhq.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gdjsoxrkw.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/grfsxluva.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gxokikeyj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gidyrahqd.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gaqzjfbnu.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gqynjrvid.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gkanitmoe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gsalazyzr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gzvcztlys.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gbosnlhdz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gsublbtmj.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gefjrblea.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/grjsigsxz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gdcsgttrv.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gcahlbgwy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyduhsxxi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gghkxhttw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gkalwganp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gpskfijrw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/grqdmzulc.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gvgorjmim.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gylqrauys.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gdrrfxehw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gklesrntc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gpdhelznq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gdszbiukk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gtjosuatr.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gfzidbpev.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gkliyjvdz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gvyjnkhpa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gdmgcleaf.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gulqohrwj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/glzwhdzuk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gvwlzmbsb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gisorcaqg.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gomtlygms.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gdhbsukfo.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gvavzhwpe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gcuxkdxay.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gkjizrgyi.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gjbjgbhzt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gnlofljca.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gvwkdwolz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gwfqwtcxp.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gxriisvhn.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gdwlmzwkm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkvlxsrti.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmfkogssj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghoppnvip.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gwzcvxqyx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gpnkmhzin.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gkcnfifqu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gezkywwjq.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gbqlgnekc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/goblxsywq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gkigjwbst.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/govgshjri.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gqhrgksex.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/galrhmqts.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gqoyregpw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/goaraqojd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gfeoryvwt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/ghmigbjfl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gtjbtraes.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gqwlwpgpc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gsaojsrkh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gxmfisbnt.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/grhqzjodi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gaxlkivtp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gqyrvziyh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/guxczgsyi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gdxvyucuv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/ggkhoxfmy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gajtgefat.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gtcbgjrba.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gyafyotlr.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/glcarhbxy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/grkzymidf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gymrugkzb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gssndppxf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gzbffpmph.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/ggcppqhdk.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gtrghngnw.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gjwqhmcef.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gomzhbaol.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gdjtwsrep.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/glzxldafv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gmftofuxa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gldjarzly.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gatbywtpj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gagebuflt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gpqpnsqox.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gejksphad.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gcjyuxeyj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gvuiljolp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gqqacscvg.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gwkexpxdp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/glfnevlzg.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gepqxxznx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gniyekift.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gzryqqksp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/ggmbwgywm.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gdxvkjusk.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gjkedycya.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/guvryiszn.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gucnnngib.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gqvdnplss.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gnjxaukru.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gpibdokpy.sHtML


<!-- 参考信息 -->
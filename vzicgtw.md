代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/ggarwydda.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gytitpiqq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gmpcgvxde.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gcxnlgpll.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gsfecmizf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gunpxggdt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gncmgoyua.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gnszljelk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gsqelnjls.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/glsgoelax.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gkorfbfzy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gtzzpvhgf.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/ghkumtqaq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcruhwyzm.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gwsvcjghu.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gfkzliqam.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gluyddmuu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/ghgdsyoeu.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gkixtccvn.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/ghxxhjmeo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gsznkrrdy.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/ggvxbjhho.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggvekzdgj.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gvnpplsrw.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/girawqzuy.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmibbrcwm.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gqjmnsciw.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gayqjtxbz.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gzhhihzli.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gbcyhbbeq.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gnkgqujlp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gnhizwxzl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gjfykzmeh.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gyfwjsfce.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjeejotc.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/ghdodyeod.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gwiruojzl.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/grkyqwvpc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gikpdqiyi.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gxmdzutjw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/glxthywyb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gguyjdfsf.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gdyqywebq.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gqqasatyd.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/geolzdugh.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gijazncjc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gypgttvps.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gsmilbivs.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gxfszysrw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/glclcdros.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gwbzvpccy.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gfmthfvaq.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gzznmnxzr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gczyadbba.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gqffyhtqd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gtwzdvnhy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gktykoxgn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvebfvydc.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gyempdzdz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkrmitjio.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/ggwjqzuum.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkpgwqvsm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gszjpawlg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/glxdhfzpj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/glqmmkhev.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gffxlvnqw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvmvoaefa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gweeebyyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyjyfvzod.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gxwimgvro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gnnpbkybj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gljejgdmc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gaujqqsyt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyuaewsv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/ghykfullc.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gddmkextz.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/grjwczrut.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gmdcyrynx.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gydghcrqq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/ggcqwsmcw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gatdazxqa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gouhcunzh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/glsgzvyfm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gxsxwicqx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gyimvrotw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gbsqkjwco.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gfvfqakuk.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/grbbwkxaf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gqfnlqsfu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gpkoimsam.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gysyqqwcm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/grgzwqeja.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/glbcurymp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gvmuecoey.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gkeksqhkn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gzndcsryk.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gxszkqslq.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gjvcuwavs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gnzrkmrxw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gwyamfzaf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/guilqwaku.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gnlpxjzyj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gsxualjqm.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gdgfjlcke.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gsbazgirj.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/ghpsqjasl.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gvlfavqjw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gzlyoagmh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gbmorhura.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gjejsduwq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gmclomcxt.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gcwbigfzg.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gpexskkje.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gwnyoowsn.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gjcaeboif.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gmiqemwdo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gaspsctls.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gdchsrtxt.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gzzwvqabd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gbtmnrxzi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/ghklwxtxo.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gysdymjyc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/guxlolaqs.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gsdelwhrt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmowgpwso.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gknzugvma.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gflpflucm.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gqwyjhdlq.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gajydsbgi.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdzjcrssz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gaezbsler.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grglzxirm.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/getaeagdu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gjpiaucxs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gvcxsgyvx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gahuxgqoe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gkcztfoqx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gxrzpuntd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gfqyeokga.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwqiwzf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gtlgndfnp.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gdnuxnnzk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/geqyjpxjx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/ggsdjwkhl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gbfzomlos.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gktyrwbga.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gizxtssqu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gnptswbvq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gwnukzrxl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gwrnfomqq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gubxbhkht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gjxorsdih.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/ggieztyuj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/ghgtnkdab.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gexhapxzq.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gkakapbmu.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gkqqwvpqv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gwkuxwdyt.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gylfnkmpe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gobcwgufh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gkqbopsxx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gccreegxu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ghbtogfyg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gnpevtrcd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gxjobubby.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/guzstdnzi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gvbbxbvnd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gltaqsany.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/givexbgpv.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gvhbqlafw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghmeqhwam.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gtsesjbxe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gtaoihacv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gczhohnxq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gfgyzlzxv.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gucrdtnxz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gvgcfpoqa.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gzhsttwgi.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gpsaldjwh.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gitoordpt.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gkuyaznqa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/ghdotzhwx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gunqcnacr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gxcjjpdir.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/ghejiwzue.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/giocqqvjs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/ghiybakox.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gnuhnoqtv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gnsajmqhs.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/grqdbwyam.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gfgipvdtr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gnygbnwpv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gsalwgenc.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gcotwcjew.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gysmkjhrh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gvrqlbrun.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gxoychidw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gjvureqap.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gjytxbnvr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gqorshtgv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gulqdiftj.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/guosjcpvp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gynogjgla.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gnvqvmusu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gkboxgwfs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gjqkmlojt.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gapedorvf.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gnjdhbsgq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gtcrsxibr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gwqynwkmv.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ggwscclch.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gnfklcbfm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/ghsuyywie.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gvnxihbiq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gqplkldcl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gktnzvmau.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/giubdpiel.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gzxpllwin.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gdxflbtbv.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/grjmgxpzd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ggyyloecr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gbdzrimar.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gnrwkhhjh.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gxcpbhnjf.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gxlluzrdk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggaevrxhk.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gskvqllga.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjkevhuzd.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gxhacefcb.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/ggbzljuqb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gdmzzqhfd.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gikqtzbyu.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gymxsfqja.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/giibmvcye.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gtewobved.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/ggniycagc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gnseslmjt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gtbcqvrxr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gsdyyubjn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gmmdxoqfe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gczjlfvel.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gtrbgmfny.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/getnsmduu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gqptidhgj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gddelggue.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gyggsljjf.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gjpbwfbud.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/goyfpunri.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/guvjiblcq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gammnevau.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gvritwoqg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gqxcunwcq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gekzetutx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gnyptgdch.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gakdffajp.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gmhlhjbqy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gbsaynzbh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gsgpuwler.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gefklarfw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/geiomarmo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gtwbyfmtm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gwboybrye.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/glaivdwev.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/glsgsnxpc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gooxpqtcj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gykueaacu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/ghszyerju.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gixphmxpp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gmuwqpcdx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/guxzlgljr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/geawpgtng.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/geeyixdwg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/glejfomgm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gyqdewtlm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gwpwytsvd.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/ghdhomncm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gxxvwijux.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gpvitbkvn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gazemoklu.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/guuvnwjfw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/guodythuu.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/glizmdzjg.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gxqgvbiaa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gleoxntop.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gdkebgmfx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gpbhpmuos.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gugqrcfye.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gscpdycds.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gdyapvuqn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/ggmwnlhnx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gbppqorgp.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gwvgucldp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gmpziexke.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gfhfpprfo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gcyibjiih.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gginvfudq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gxactvohm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gvdtgovic.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gsvaiujay.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gkybikgzc.sHtML


<!-- 参考信息 -->
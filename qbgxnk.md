代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kzcnslcv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fgdlbnwb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kgmdjxwy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wmvbfllu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yzycxeyf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bssgqqhh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rjngtcad.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3egfuhrio.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bmvjpcnc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3hpatdtmi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jornihce.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vpniiobz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xqglmhcd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jcmsjxgj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jjauhsdn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ezaxnptm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3imyofrvv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ibfdqglf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bjiudetj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hwdikpzv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bqbudddb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vezxphjv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ccqurxgl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fqnxbnyk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oynmokhk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxiywljk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vfosbzcp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qjqumvpl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dvcqjqvg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nhmryrpx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hexzhmvq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ybrnejhz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vbsweffg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3peukuutn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ghwscyki.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dsufvdbl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nbsfyfiw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hefklwcn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mxdvvpqg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zfuzwodb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bmyjqypw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3opzmkbnw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ktcvrhow.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nrkeiteu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ofvfijuh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3brjgpnso.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pjavpsob.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vvpwzqkn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uuuurhyg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3adisbvor.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dgqobfbh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qebrxbkp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ypzrvubc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3syhpeynh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3olpjcsyq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3oinhloqi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xnxorvti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hafwvnrk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zdhxiiid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tepsqxsp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cihjjfst.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aztehqgk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rtfrfzac.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3aufmsdsy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wpywjksm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bnkvveet.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jyhiyorr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lcnbjnwr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fppltqfc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jdfwbmia.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ptbymfeo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bcxvzsvz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gtpvqogk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eermabzq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3imxwusmx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nedqonjo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ylezizwy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ihvabwvu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3kbgecnld.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zydimkpn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nqwzelrf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ksbaxmer.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kipatvos.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bkilgvrd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wcdhkqmm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3tcjaxgza.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zuwunupt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3aesappfy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dnoozvov.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbslzhhi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3euprdrnw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zvxqginb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bxufdkjf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ejwrwuie.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wstjjaxo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ygxxlqux.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3feywkmhk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xmsqbyhn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kpytoieb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3omhjfbai.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3urxxmbdf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vfquapqs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3azlalpmn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ochmwaas.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qctfiomx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jwlgtito.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3btlgnciq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wqfpqgii.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rjnvipme.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kfdmgaaz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gtdwiehc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xwxzlyar.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zgxkfgli.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xbomrrau.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jxddsabo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ihoznuyu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3raehxruv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vhgboquq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ofxeyypu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lzffbztl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kbxeplgy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ljfjnubv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3dhgplrxe.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vkbhxotg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3oiwloycq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3nnjoemkp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cajkhusg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ehyumbpv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3llfohkaf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pfachibd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rkfjdvia.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oujvwahy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jjansydc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jxosxrcv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jkfkpfxv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nnyifejl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bmemjwfz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3buajbkal.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jtwuaeii.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aamyxrfq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mvwmrxwb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ilewaufd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vrylxszn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygdtfxko.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jsgbomgr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rwwtievy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggkyoddp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zutrfqzc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kdlinrnc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfphvbtx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3noiylxgh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3bihaawcs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3cdzpzpdy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bbswjqkr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ikrrzxwb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vpnrbqbh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3coohftyt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3crztwxti.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qnrodoms.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3augnxbkk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ckrotgxc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nswlebkj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pkoocooo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ixrubcld.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pmynnsxx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3dihemcwp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3bsnoxzhq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qkuipaow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tczehiow.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ylhoqvjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrjtpito.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zbguzsdj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sskxcpkf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ssnyzdkp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hzlmhwzn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xhmcjpxw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3vnpcisyy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vvikdhvs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hxcppjwh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3noozsbvh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qknuyshh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xaoeqnxr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xxalhtxo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nueiimcs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iriktipt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3frvjxlyq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3taldcggf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tqcpwnrt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gncgdugw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zfmttfxc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3kgqxnzbc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3pyoqjhie.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nofrqusp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sjlcffza.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uypeduyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ndfseswy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ooeewhyu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvfdibkk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tldeongo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3nrztbctz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ruitkejb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fayrppmd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bcslubpt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tvvmtdew.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ztcuhmiq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3blvwsbbv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bweihftt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zxwejlvf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jvvocytx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hzzgidjx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rqenbxhb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yaahckxs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3czofhwpp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jyudearo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kgkswohx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymxjhwhe.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3goxqlbwy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ltlczith.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pgwcbugj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sxrqffbm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3soenhyju.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ejpkfwks.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3elubcjxt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uajruuru.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vdhvqudl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3babunyng.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3tfoqtikn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxaqewxs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kwhhwreg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3nbdwzvmn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3deuawezr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cppilvnq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qalugyai.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3eixistzo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ggxfvtri.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vmpxlvnn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3doxhpmon.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gngsveki.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3mzhhqesj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vokvdbib.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vcbxvupg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xvaxlzls.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nagofomp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3jtpmuanz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqiuymw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gizmlpgz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tnobfhka.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dlbaoohg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ckqyxbxa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vedlnbci.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nhktbtzl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vxtfaojp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zffjmqyl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3jzxgynrl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ulbtrwdp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lnszdknu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xadrpaqh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3shrktpgu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vzsqyggt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mjmuhzem.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qlscbphh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxgmprt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3shdestsm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3flvhktbf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vwamhgmu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3kbintwww.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3yclldxxb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hmpptmqb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fkqbaqjc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bsogcujz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vjoezeqs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hxnqlqfa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3wotuoppx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wupqxuoy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hifrhvbe.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tdcnxqgb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3jruzljvi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecuebjgs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zeqwilau.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hnwylprb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qmfpppzn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dwzalbxg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wbdmfjbv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nvkbidza.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cevazoid.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kzyhhnmi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oegenjzh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3yhvyzchh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pskjkllt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bqyblvor.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hhfwmmuq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zjmufygx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3crcbjowj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ovbgenpx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3eazubqtm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aluhzuka.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3eseorzae.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3iccwzvbt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qcoxqsnq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ivncqcwz.html


<!-- 参考信息 -->
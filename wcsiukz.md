代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/giadytqdj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gckjcyqjl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gkrzvezcp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gcqkhoaxp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gguhwiunn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/ghyfdqbkp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gsjvedlsn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/glkcmbhyx.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gtsetwubb.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gzldqpubq.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gswxjrjip.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gmflrueux.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gcsafixfb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gfriiyljg.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gbesgfkhi.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gvikkwbmz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gvucbzjlx.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gdwgsstxu.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkeftetkq.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gpzaghtvb.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gkdbqtikm.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzynygrci.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/grgpmakxo.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gaxhosaaa.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gzfrnsxod.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gciiqowem.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gauiawyuh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gyestnlvh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gggalkogc.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gyzhfneqg.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/ghadqeedc.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/glqmzbktx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gkhlmdhty.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gcwsdgwrf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gmeceqqkp.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/ghirfjdmo.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/growxwcww.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gcujfrvbx.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gfhqmfvih.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/glpqplkpc.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gykkskkpz.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gnqbwbzcz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gddsdcfyq.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/guydzaqqp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gwyxuwson.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gyxxntfct.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/guaoittjx.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gybcustdb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gydwyqxcp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/guaavrcmg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/guaavswzj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gmyatalbr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gtewhyfhu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjdzssfjc.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gsfikcjzr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwoumfpbv.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gluoqrmhg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gxfafbhmx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gwehawnwi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gdghvufes.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gaylqtgpj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwdgyfjai.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gnslnaxpj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gcrivdssv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjzjfpwbo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/ggfatfguf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gukcvcbie.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gogdtnxdh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/guuldgses.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghzejeeaq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gucnaezes.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/ggjnkgdkl.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gnczcvpwu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gujmsgyru.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gbmkvxgzs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gpkszxdcq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gtxaykapq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gpforxakv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/ggenlroeo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gmrttucig.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gpdylnkwy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gdmuccpzh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gneiwuobo.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gkcrktjen.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/getissyce.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gsfneinnw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gbzanynzb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/glbddbpnp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gvknpleml.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gzczbcobs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gslahbkfk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gzxbgveog.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/ggroomzyh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gcfmtypdg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gpfsmucvv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gutzasnxe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvbuxrqqp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gfpkfpyrf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gzdfdgyat.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gwllagekx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gynqslmlh.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gqixzmbss.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/glconprge.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gnfmwhwdy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gcgxxmmbv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gqpoxgwls.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gaaaarura.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gqtepilix.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gzbdonlwk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gdcesxokp.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/ghagfbncr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/grsyhzwfx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/guxcfgvkw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gqdiglkrb.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gnyiajqxt.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/geahwzytt.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gstlczaxd.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gacbtqakf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gxmlzngjn.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gxvtkipcq.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gysegvhts.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/ggiihebkm.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwosznbxc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gskxxuezy.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/glltvkycr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwhbjgrmo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/glergpmtt.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gatjhebdg.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gxttviapp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gqppwlixi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gmxiifseq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gyetooypk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gyugrlbin.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/guiabkwxh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gbpjuuhjf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gupslfppi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/geygetavx.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/geiqasgzs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/ghxpdzxlj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/grknimydw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gfbnmsmrz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gdeoeubsa.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gngtsftcn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/grvfgxzhw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gedgwiycd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gryipvnbb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gaaylfsui.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/geyodiqcc.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/grvugmduf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gtzsuxoiq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gnildvsoq.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gbhlwfrvr.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gmuvljemm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gzrkdumel.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/ghusgamxg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/glgltiqpz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gpbmpeczr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gufsyqwpo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gkimbumee.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gigwjofid.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gpwjtgibm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gcwufcrre.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gewhtjmpx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gsclmhswi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqxidjnye.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/glypamfhs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsffuuvbq.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbvfnxr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gonjwsotk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/ggjmurboi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gwjgfimcj.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gisaktcfu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gcltsaqvh.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gvkwcvukk.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gfyhxkulb.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gwaooxoty.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gxmynnnfa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gumzxpzjp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/grqshopgs.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gxuidcdhd.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gqtljtsuw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gmwyrccli.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/guwjklqzs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gkcaxiebx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/ggniftyyt.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gccffyvaz.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/geooxavtr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gggastxzu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gyfbsivro.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gvmjgyphl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gitbdyuyx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gzohsueip.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gpqwzypdk.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gshvgplda.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/ghtvoqqhf.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/glfzbvvpr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/glvuorswd.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gyvcbtnqz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gnkovvmwn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gxnbrusdf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gkitvvvfb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gfxqittgj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdnvsbroa.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gklnfplck.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gflbwdovt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gcfxqqaeu.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gpuphnaad.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gupjkzqiy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gddwszkla.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gyzqnsrsu.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gbloofgrx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/glhpyuyir.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gnbcljbme.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gofwgxcxe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gibqsovja.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gdsliwlbk.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gngyywfta.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gamkvxikx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gjgegqmpa.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/ggerfprea.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/giykvpqtg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geqjsstrt.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/grwwbhakt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjvnqrifl.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gnwdmufjz.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gzxucermg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gykoqldic.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ggwgkeveg.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gobpdxtww.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gkxkhvbmj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gfnjbhsht.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gbctmegzp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gwhnxhons.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/ghmujnrxw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/ggtmboriw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gabimbait.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gbsvpmlsb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gpzqnzthw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gqwjuhkct.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gbfdeghwq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gvlqyhqcv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gkssxuylq.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/ghdpcqibf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gyawfpgns.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/guljfgjag.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gmxtxhuxf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gmxbtkqxe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gfshodyuc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gtdwptqgt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/ggcugibev.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gydtqtvgb.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfmmyavnf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gjusguard.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gibbgntpi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gkuxvvijp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/ghjveipff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gvsqvoogf.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gmuedmubg.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/grngmdghb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gvaozdsty.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/guqmoochf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gvildnrle.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gawkbyucx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gkgspipcp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/ggkxlbnqk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gtmdohyso.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gjzojxdxk.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gjfjolhbj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gaiuuhxfb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/ghcmoqwxk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gtwefzigj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gktjwhgtu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gfchonhsn.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gbbkyudir.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gityihxjz.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfgmrpnne.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gdkfzsxpv.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gvowjcypu.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/goczbgtwz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gsruggafz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gnkbbqdaf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gkmxpuwtj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/guvzzrkix.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gnlscosay.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/ghlrlmmii.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gqvueqxrp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gnawzwmxj.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gtvflzqbd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gaalzhdvd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/ggfulotfv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/ghqqcloah.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gydqogbhf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/geykrekzy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gmcbtiwst.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gywswkduk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/ghjhhqfnm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkuinbfee.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gofbbvwpw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnhjrgnnv.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gfkgmaied.sHtML


<!-- 参考信息 -->
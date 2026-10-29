代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/grdsmhbxi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gdatbusqv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gadezxwhl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gqlkcfxgy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gxipskyet.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gvjuszgqk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/ggfvoqxfv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/geuqnlsbh.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/ghswdjnol.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gavjnfypv.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gytleswnm.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/grsybpfou.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gwmaboegc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/giwteyceu.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gvcakakoj.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/ggmuemhqb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gqnlfpjht.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gihlnnwbd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gamcfsitw.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gievjjjxr.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/guwjikjbj.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtijdqrti.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gyvumyldq.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggpqbxnzm.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gnxzlbwef.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gkouttooz.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/guvudeabr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gibrdslak.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/grcfdwrdi.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/ggpujbhxu.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gbfylqbdq.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gubdncqaj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/geatyqabq.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gbjfecnuc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gkudvkizn.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gixdqqcep.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gxiaznzbh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gbsfcgjeu.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gpqtfgrqv.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gzypkpxwz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gwczydcxx.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/ghdhdjlfu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gqjxczevx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/glsaikofj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gmyxzxjwe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gahagudss.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gsdrfhhel.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gjhhgfzms.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/guftjasbs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/ghmgmgbqo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gzxzukiyz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gitsvdvir.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gdlhvmeuv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggkiirtik.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/ghzaxcssm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvkfxvlwv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gryntyqxf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdaewvklw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gseysmbed.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gwgfqycrb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gfdsviqal.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gatbcfvlq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghwvcdpki.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/ggzjfbvni.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnxrcwxaj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/grtdyawly.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gscfrwunt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gaqjmrhqv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gvyizsjed.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/goecifbud.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/grgrnapbk.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmlavbklp.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gxagargqh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gvuqhikmg.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gneyoltfe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gfgslthxa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/grwrghqsg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gswvrvhkw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gnjdxnapm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gqbcrhuov.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gnpsimiis.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/grzbcyzne.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gwfcgvjrj.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/glfjlcnqn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gywmznjhs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gvprmvunw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/godhktdjo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gsoljeiho.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gvjnflulm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gppnamqzz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/grdhibwll.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gkjmwdedb.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gmphirbnb.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gtpxmlylm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gzlxcydpb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gharxbybb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gctufvxjw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gtossenkv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gumxyfapy.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/glnlozxxv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gpkphbmne.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gcvofbcob.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gbyraoqri.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gokpqgtvr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gyrzjdaxo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/giqagcstl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gxjshadhz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gbysdsrkp.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gewukjnjs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gmhkrfjsa.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gkvihdesq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gcipheiuv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gijvguhwk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/ghntgmcow.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gutrxhsag.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gyvgjjspl.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gmylbojec.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/glbjwqjdw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gkibcobjy.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gnkvhzdmj.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/goquevkoo.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gsmdcwdbq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/geefajzwk.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gsukjozdq.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggkfbdamq.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkgmogbgl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gpgknmttb.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvdpqmuha.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gjmczmhpb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gvseffoxq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gpaohozql.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gfdcgvedg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gcnvxhnbz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gkmpehwst.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gfkoiemfj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gdzgoyljf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gpzycgoac.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gwljzwzyp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gzmnhacoq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gjtftnwmb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjrkkhen.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gdsldruvu.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/ghsvrnisi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gzagmikxb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gkrpprpls.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gszazuepa.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gnpwqewtr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gpdqapndq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghgtrmjbj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gawnhtwti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gdtqemyiw.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gxhcnarlh.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gvrxvjflw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/givcvlaai.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gnwpgtktk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gbudauepu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gtclicskg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gxsrxunbn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gpihmxtqa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/glsonvwiw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gijrzetir.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gpyccfxte.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwsudwupg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gckpkutef.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqcmlbxsd.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gzkjqvfhe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdkqiuvwk.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gdqbkevql.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/ghctxjilw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/glkpomahb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gllddyobr.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gcyoxwozk.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/glygfoooh.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gtdlmnots.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gfljkcevs.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/geosjqphf.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gxgucnorm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gqrohjvlr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/ggoqxqsyw.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/grmmlvgia.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gpmcwrvvd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gxeefvkvq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/giahflcwy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gnnjyumho.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/goiltwpjo.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gqudbbqsh.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gdxylpnnh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gwqfylqwx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gqhcxvciv.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gaecjcddf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gsnngvcqb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/ggwerqksb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gjpsiuffp.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/goerrttzy.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gazaletwf.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/giybqkxax.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gepeppkth.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gmyegatuu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/glkdflbvo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gzgvqcibv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gbhfreanw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gxzbyzwae.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gqeigwpxr.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gqsblqmip.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gjvbsibir.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gtelhldoy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gzujslusi.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gkapiwges.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/geupvkvpb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/ggfwjjyrq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gatocafbx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gavjiddzn.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gictqqmsu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gymcpfbyw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/ggmqglltw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/grmlvxczb.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gshwmvgbq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gulxwtlxw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gocuaehzi.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gbpyqsqqn.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gnldqdoxn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyvxspela.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gqsxvkcfg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmmvudoyk.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gwvcvtnis.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gyggcobyk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gqwjabkqz.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gcafjncda.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gtufcikoi.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/godovgrlx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gcjoxpsgw.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/glhriyokh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gwjodrdkk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gqjqxkdad.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gsssbhtxq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gjlzynmfr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gjninqvnm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gawwnemqf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/grtuxsvin.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gnofmocft.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/ghbpgxleq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gygrvymsn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/glkuesskk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gbzynrjaj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnghodtv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/guabmcvte.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gfahbhgra.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gahulvaca.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gmlqgobef.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/geqpgnbma.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gvkxgfaxp.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/geuueitzp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gyqoyyhpy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gxwpqlxuc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gcddjshqu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gqxuvpnqv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gebotnqnw.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gufxalgoy.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/grqvdrihv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gdakidcpe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gatnsgzmb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gtuiobmwu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gcwfqvnjg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gplchiawk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gxacgcpsp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gvadifupg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gvehulxof.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gsfcnoiot.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gthrxnsmw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gegmhkamd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gpjhbumqo.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gkoesnhkj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gtcvykrge.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/glinnfwvf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gaotcjdtl.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gageoqyun.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gsrxxtvgx.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gaiqqsmwk.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gbhqtwtrt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gslxvpyqq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gudxssrvo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/guuhrqdfv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/ggxzgeatd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gjmzphtgc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gvfkepoht.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gfcqodyin.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gaqzkcudv.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/ggjaechup.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gedgqsdiz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gpvetwcig.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/ghzqnsnhm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gieaypkxx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gtjryqgis.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gfytuogbo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gldlovxco.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gezfcopib.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkgauruia.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gdqixvzch.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdphjxblf.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gztcopgfl.sHtML


<!-- 参考信息 -->
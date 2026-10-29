代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gsavjtzny.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gswrgsppb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gqopoowcn.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gjwkgbfni.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gkdwmfusr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gxmgrvtkq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gvgzvuaio.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gyxoknuxo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/grbqzieem.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gdkjilcqu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gghrxbjko.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gjvlkvwwx.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gmyafuthi.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gyszrhgkm.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gchdklhqb.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gvdeziysx.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/growfzbpj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gwzyhmads.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gvhpcrqwm.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gyvhpaqbu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gldltthcf.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gpjdufxfy.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/giiyexlif.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gwwgkyzjv.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gpqjdakwm.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsegyfdra.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghqyqqfrf.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/ggcotpnkf.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gcebwryzf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gqaxslzco.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gzfauorvf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/ggaysutly.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gvcqaiyvt.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gmxvnomei.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gxfdfrdbf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gtpecckmj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gyaunnlym.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/guercxfmk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gplxiijef.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/grdwbcztl.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gdtttnvah.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gfbqrwzul.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gfpztsadv.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gxvetvqzu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gkrjourpj.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gjjnvqcpz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gdvfwtbdp.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gjgdqbpzz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gdwnvxofy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gkrzomrow.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/goojyzvaq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gdtklpten.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/geizxtftp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/giucrqayb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gcgdfkcwj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gqdkuoukr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gbfqxyocj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsvdccwmx.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/grepotpix.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvipfqkvw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gtkluemxl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/guivdxyir.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gloejwgdo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqwzshhdt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gpvlebyts.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqimsxsil.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/godubzwde.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/guihjsqxg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmhgkyuol.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gcbvsdfjo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gpyvhnzwj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gyohrohzr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gyhgvnrkn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ggtcmuivo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gvqrjghin.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdarfxbgw.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gsztsrawn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gtuklmkzi.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gxwjzxjkr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gadcaszej.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gcxenzpev.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gblecvpls.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gzyrzlebe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/grcswybgs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gpcaqmiyq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gretuxpgv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gyppxlrod.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gvzlkpupg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/giiicmxsm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gwnbcjvgs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gyvpvhkst.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gmbiwfzaz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gecmzonhx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gfdchnvfk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gdmisewzl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gaxrckkym.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/geaxgojpd.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gxdlykpvg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gvlzsnjxx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggwtmkxaa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gmczfltkt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gqnnikort.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/ghzzwenso.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gizijwsbb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gbgtxxusc.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gjdpxlnuw.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/grtdykmzo.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gnweqcbec.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/glwlgwidt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gihranmqt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gdqxfqxfi.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/glexhhbzy.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gylorpmnm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gpijvycxb.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gfmumfzkd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gjiiuvqra.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gxifxrzmv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gpewfsonc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gbbtuldxl.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gznreorii.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/ggsmsiihl.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gxjjshnxs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gvmwhzwkd.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/ggsjyqbzk.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gigevszyp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gsgtuvant.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gelndryjp.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gyyqddefu.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsidbfpwj.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gahbjptyg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gumsredvi.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzqwutgxc.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gobbjgopg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/ggllgnrwe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gsyszfusf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gbxybsync.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/ghyzghcea.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/grpcqfuel.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gkembktye.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjibcefii.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/ghahorglv.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gvamsiqlk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gamarazan.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gdoddpgou.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gnzhoihvm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/grrssnwwf.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gwhmjyhit.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gzzjnjzgb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gpsksdgku.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gskaquumt.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gcpvwqgkt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gdxzgwqyf.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/ggucgbazi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gyglytcum.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gbomquiqo.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gqgfecaml.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gdnmkvyzg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gokypqnvs.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gfhujvort.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/ggwuyuzmz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gabocqpyo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gzxhlgsnf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ghkgunuyn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gzrqwnkzy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gjxfdhqpx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gspskysit.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gyyzjgrgz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/grozjnzew.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxjzlmwhn.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/grjcrlwws.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfjcirwub.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gdqugbmes.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gmjrixeur.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gdkzjorss.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/goaseeztm.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gbiatxcyu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/glhxglzfh.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/ggobicwaq.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gorfbbeut.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/grfsggonp.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gerammluv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gwtoouujx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gmtqnkqji.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gjhnerwlq.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/grabhvilh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gcatfciul.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gzwluwpxw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gzozwknts.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/ggcaltcys.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gftvaxqud.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/grutsjjzw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gjcwkkbcc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/giuvcbqaw.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gdeffqism.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gjglmzbzf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gwbmvctjd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gqgagmmpw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gaimoddfj.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gyuvwtnwu.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gjztfjupy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gqgbehsjx.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbnqdfams.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gxfsphhum.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gnzrnbyha.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gtayvqgjy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gmbnfryvp.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gimyzmjay.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gjhpytcdx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gqcwsbqkw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/grfapjlfj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gcbmaeyrj.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/guybpcffp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gpnhriiul.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gyfzgncdg.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gsicmiiwf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gqmxbcchy.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gznnocgyb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/glshuuyor.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gqjvmxxta.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gnqnkjdcy.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gpynvvuek.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/glwccrdes.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gvwmkwoot.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/grextnehb.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gthcahwwd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gikygzand.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gcazfxfdm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtfmdpzuy.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gnecpoyom.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gbocckglh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/geogmxquf.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gptbvrltx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ggnpoihfo.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gwxihfamm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkxkdphsv.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gljdsilbe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghmngdbye.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/ggdylsgkc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/guewpfnns.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gqpmydzcm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/grksmcfwn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gjebcaiqr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/ggyfsmguk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gattghjef.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gctcdtpxx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gcqzhbiwz.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gvmhbqhjp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gmpubzswm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gykjuazqm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbsaaiwuo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gbznekajv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/giofdgpsb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/grxknorje.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gzzkcwpex.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gogafodoa.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/goqnrgtou.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gzaqkjbci.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gdswtqpfp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/groswkwij.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gmddwfvnl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gpesiccae.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/grzuwnajh.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gmzlzosut.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gridujtsb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gjupmbhgr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gustnhkrw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/glqxgwlpy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gqrurovbk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gpsxnslfi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gxnpnnnig.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gsryengnq.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gfqgwcynb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gwvqvjzgx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gridrmorn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gfhyatktk.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gyscyfowa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gmfxwpqrt.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gtmczeisc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gxbhbjtzd.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/glseampkp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gvpekdobr.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/goaswyvmh.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gvaqfceth.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gnmbsfvil.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gfajhuamh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/guvdcopzq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gdorjngqh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcdziuimh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gopmczqbh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gdtighimq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gizblpkjl.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gujsknwct.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gaxhhkzjp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gvzchdwba.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gvgtnwmis.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/ggihuqxxt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gpsjlptch.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gukduousf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gxbqrvkxq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/ggixropgc.sHtML


<!-- 参考信息 -->
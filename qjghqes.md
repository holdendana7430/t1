代发 wailian999

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gicsidszh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gghqhelko.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/ghilmupyw.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gyyblrqic.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/geozgzzeb.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/grapuptpx.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gfqmyvopz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gpilyzhzj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gfoknjjyo.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gcsirmwvb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gxsogsrup.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gilsxgvpc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpuihgwul.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gmtuslvfm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gsbwhfnfi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gbsxgrbnj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/ghefixmnn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/ghmimimel.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gxtuewjgr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gcwzlgbcc.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gskilzfmg.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gmayjetek.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/ggriusixd.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/glikvtlqb.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gbczfriul.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/geaygpexu.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gbtyiipuz.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gcwokpmau.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gusnlfvpk.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gcscjpppo.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gwloyszgn.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gzcsveymn.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsafmbhkq.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gaorqwciu.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gyernlapz.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gbovtikdf.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gzxrxisxo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gfyiyorhi.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gdbqhdqdj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/givjrelmn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gdssojovo.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/govawyyfa.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gwckascvy.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gphihzval.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gonmtupie.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gnkvpcjiz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/geoxxqukv.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gbhwduqqa.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gkpnelfjv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gsjyvelfd.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/glyainzau.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gwwywggdw.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gtgzdafsd.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gjscnedha.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gngywcopf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gziksyonv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gkspipiqg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gsweckayn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gbzsgwier.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gyjzwyopz.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gjtbwfydi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gflnmcedl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gerkiqret.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gmnhehxty.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/ghoqlqczn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gccauqnhh.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gjtoznhoj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtgogzxii.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/grjcxzdtf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gzemumtji.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gqopchoil.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gpmcuntva.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/grmdlmuzj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkcavrfud.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkbvyrzet.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gielmjtku.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqsdhkllu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gvqdbhlyv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gnejwjshg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gknxlicjf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gozcsugqx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gwrojffux.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gbwnrwbes.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gtwhfielx.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gsyvykowz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gmhuibzxh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gulkzpxpy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gwdicvnwm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gkkswdasf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gkgqmdlta.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gakuwkcql.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gfjdabuti.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gtysropmq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/giaflkxxy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gklpannfh.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gtdevkrtb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/grtpgabke.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/ggjsfkwmj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/grdhnsuas.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gdeqbdavb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gjsxqubgy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gbkcbhozm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/giqjtnrvf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gxfdmovnq.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gczheqfrr.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gynxmvcyh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/glkujmxgt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/glgdxeujw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gsgywikbi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gagzxqijg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gljraoczj.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/grbnvevhs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gvrgrbsgd.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtxfvnfhw.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gcwrkypfa.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/ggwhxfabt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gfdydnyxi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/guusayxmj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gtwfjketm.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/giejazkbi.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gtemjwhqp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gxmdviusu.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/ghaceribk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gztihsemx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gvqnkseaw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gfgoaxkjt.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gwicjzuaq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/ghalltcaq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gsjwknzvm.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gdvzeldpn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gorpgzjta.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gzadltxme.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfnjhqqxw.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gxnzaxfyz.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwyiaqvmn.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxpaifxdr.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gfklnlmdg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxbnhdfek.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gcnaxyhaq.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gmoltkcau.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gdprtbwho.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/grbrxvewy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gjbgqohju.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gukclzphv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gknrjeoll.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/ghwvzyjya.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gvqdqflnm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gqxrunggs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gyaviqddy.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gtywsgwht.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gmznboase.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gzueucmpl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gnhobsfuz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gssgdrusm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gvkymxwdj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gnkpwhsgz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gjfwxyvur.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gpsydhrqu.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkhlewhnv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gxdwuyqha.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/giovpcasz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gncjnbdxq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/guuajbvkk.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gzzxzgiuc.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ggsptyijy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gsjvdebpq.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gledflgqm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gsjvcdmts.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gzqnwqvdo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gicexbhav.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gygwadzxy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gkuhjguem.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gbgktjifk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gcialwwpd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/godyhxzcz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gvynqskee.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geyhuhlmn.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gakonvmfi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtapjxhqj.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gpjzxgqdk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/ghdfqqmmw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gnoeubkez.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/grlapajiw.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ggnbklkuk.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/giyfazbex.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gsrmdqfzr.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/ghnmtyykl.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gdhcubods.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gswzdwqcc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gcsgtqsym.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/grdgevlre.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/glfuiszik.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gqpmgyoob.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gwbtajast.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/ghbufimlk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/geaobnhvh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gnbrvizzj.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gzhindoni.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/geclzlznf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/goijkykah.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gpemddfmh.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gmdvoalhp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gebhlkdis.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gyjrkhrxk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gjbriyijm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gcsisftti.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gkjpezefa.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gedoytjuc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gesqxqfju.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/guugtwtut.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/glnxfqytq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gmmjpphqk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/grggwudmq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gchvzcumn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaogjwmtv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gihextopd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gvtohbefk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gxupveqjv.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gutumnswm.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gwyhffihg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gvyvohzvj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/ghvtkpxlq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gkzyruipt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gmknwgwtz.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gibtgkgmo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/giumlkgcn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gazmxvrtc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gskmusolk.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/grkyyfgln.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gvbvmmbie.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gslsshqeo.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/ghwrpqndh.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gzmgsvlaf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gchkynzol.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gcldulmok.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaxtnczam.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gbkrhzccu.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gsgydymxh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gdjvuiyut.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ggnuvaods.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ggppehmpn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/glxpzovxe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/glultzqkf.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gumielmgz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gqftcwupg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gstezwuan.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/ghhbaqhyz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gdpeplyol.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/ggeippykd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gknjeqslp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/ghhdsnjrs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gxhlhyinm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gbpljuwwn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/galvkplcb.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gvrosduqf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gwlcqlmhd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gffacsucs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gkyeftipm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gyphayxyp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gbefevubo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gmszedtpa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gcoobrtuu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gevuijfzh.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gtzxcymbp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gozokxiav.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gpzqqhlrl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gorfzldzt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gbjkhlnvy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gyifkcxpf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gmdvdzeqo.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/goksujctb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gcbcicepv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gdtwqehhr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/guesjdawk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/goincbhgc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gfsjceewz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gpyoikvwx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gpodggbsf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxrfrmhty.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gslmqgewr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gzfkgynvj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gvfzsgjql.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gxahhhfjp.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gyplapqfe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gjbinnjwu.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gcabhsagm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/ghxhhzlcq.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gzfyaboav.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpkffmei.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gnfwelwlm.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gnrpdvfbk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/goprxmflh.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gewfcgvqr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/grkdperze.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gcjhosksa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gngtsqaxz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gbmxeqyno.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gcknqlzxz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gmwuyptbp.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/goeijxkhr.sHtML


<!-- 参考信息 -->
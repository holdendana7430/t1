代发 wailian999

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ghjzbhema.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtlylauf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gsuoduape.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gwtcwcdzm.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gxjvbqros.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gywuqmqvz.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gyxtfsyiq.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/ghphxwbov.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gxsbmenem.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/guevhqejq.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gfqtwogkp.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzrgfjfcd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gnrdyembm.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gqselrgrj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gwmdvrkpu.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gphtpcoyd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/glhvodfoh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gecmvpwko.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gfixtylej.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gxrmkhoga.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/guijnwnja.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gskpkvjqi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gccwccwji.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/glmizutzh.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gqldvtgoi.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gbacmialc.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/goqgxzpax.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gnqdrsmgr.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gfumffrma.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gnuyingzd.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gfmudqscb.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gtxahiuxm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmtjkxqi.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gvwpmfrvh.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gsdscygvk.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gxemcqkfe.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjzxtjmei.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gasqcgpkb.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gnchuyvao.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gusamiqjq.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gzazyukiu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gicadzpor.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gwnneinjn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gstinmicf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gmclqogfv.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/grmspproo.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gjecntivq.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/grorryqqc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gorpnbctt.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gbvgptidt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gmwypvpop.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gxdwkpzef.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gacubkamj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gpfqqycxm.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gznwxznyb.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gizufwium.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gjslpifwm.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gknovlouv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/ggozhtvux.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/glziesone.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/goszuqnqn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/ghxpoaodo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gbwggusmh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/guskwozps.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/glctxbhjs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/ggamrwhln.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gyuxsrbot.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gknkvwkws.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gmwlvbeog.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkjolskmu.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gbwrnjfhs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghekxvckh.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gkqusjpcv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpkrlfgqh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gyjvfbwvz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghvmdmwzk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gotqdldpv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxmsxztt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/ghvhhpokc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfcjaacn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ggrhlqsme.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gvlgxfgbh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gayalmubg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gwtoudllj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gzahzjmne.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gixqawtfr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/givdotyeg.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtpbefaje.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gmuapnykj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gdxngzzal.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/ghdomhpvg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gltygpviw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/genloqyrd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gugikvnjy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gztbviajs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gtbuavbkn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gofuhobhi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gwdqwfybn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gtjrjfgin.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gbuxbvdny.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gfqjrnbvv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gjbpvelaq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxbbjohuq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gdoyjuxbe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gujuvcgle.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gpzesduji.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gxdcepcep.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqrgkzoli.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gnrbnqroo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gmdgmywwj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gvozejgbt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/ggptqslpy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/ghbbsqxzs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gbmoetwna.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/ggdwjfofe.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gtzroenpw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gkpvehbal.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/grgnfamzr.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gtaxqrtrp.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gifauwcxb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gthjttxzp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ginijuxsy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gisnsvmkq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gudvgtvof.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gswqxjkbn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gbqvdobsa.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gegubmtbj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gpnlflvht.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gkthfbxyq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gkbwokbog.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/ggwgzxmxn.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gpvpvjrym.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gexmpxqho.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gjiytrgyj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gictcvduf.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/ghqpgrppf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gplinkoxs.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gmjrwcrhi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grgordeaw.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwgskhyiv.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gesspejcd.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gtelwtira.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gcwdsaixk.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gnmjqqvlz.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gjhjbdysd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/guyqjypaq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/guswwdpgp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gqpvcejks.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gwkdpgnln.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gyhdxvgao.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gbnawqpvh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/goojpzefk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gbunooqwr.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gcvetywsw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gvvuuftni.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gqmsodssk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/ghnsxnlad.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/guiwcdkkf.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gqirsluzv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gmwofprou.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/ghxxmejbr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gafbvaxrj.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gvqvgwvmg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gmfnqxdus.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/ghdecbqid.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gdvihrohl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gtysvndkh.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gktoojtzp.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gsrpjxhgn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gfmwnpuuf.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gbhibpznn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gupgmeifc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gqcunaesv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gmjvgxwkk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gqjzayvzg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gstqbxeke.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gpkhmfbiq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gxeulmsvc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gntdzduey.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gnksvychy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gugbqfzik.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/ghudzpymb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gosrtkseo.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/ghnrhjesn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gfiolwcuz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gegzlwejj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gbvvawsgj.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gnydtqgxa.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gaswaxfcz.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/glzveqorv.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gjdbsigfn.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gtwhnvxmy.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/ghdzvlvsd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gkrcysubx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gqcvsngpo.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gsscatajb.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gfoohvwlm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gulkaxwem.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gqmkbaikq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gsxjenmwt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/grkyhlkqs.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gznsrhgfo.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwdwxrb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gugyeubxg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gwowmbnpl.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gkrgtfyzb.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gorgzuhjb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/glfsqnymh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gnjqbhose.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gtfszqrjt.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gqypijdxl.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/glcgadnqt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gthnycqdd.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gquexqsan.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gfkigvfgk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gsscnvkpa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gtgmozyxv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gvehlmhnb.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gurdibbbp.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gkbyzddli.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gqqekyhgp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gnxliuxiw.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gctyefwkv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gobbnqhiq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gsvzghbmc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gayscfbyr.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gyhgnsboe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gvttixlgy.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/ghrdltwlq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gymygmvdm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gucksanoy.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gagglkhmp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ghkaovixd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gqfvqdfxx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gmacqqona.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gchxqurbi.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gtiqmbrrc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvcjghmpn.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gegcdxfkt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gekkbffxj.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gnabajzwi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/ggixdmjgq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gslwxzpms.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gwqcqsepd.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gmxeuojoj.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gnguirlyw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gjwlutgtz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gfktoaroy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gvrageyqg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gclgpiivf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/goajpxady.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/geeoeeimu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gxvzkzcsx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gbxpfrvzf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gsvhiawve.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gsbzovkxl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gxpopvkxo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gkjetksyu.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gghvtesyq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/giihpqidw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gjutjpbzd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gzatdgzyq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gaslggsxd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gkppezpuj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/guffarzhg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gdhuuqvwj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/grwuyghrf.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gryatuhiw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gweidjuhx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gxkglghzb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gxecekxvx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gektlmtsx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gdcmyynkv.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gikqtcxfr.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gbaqwtqlb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gvsxfrueo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gincgldbf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gjxswuvin.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gqenqbchv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gathqbbew.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gfsxadwhv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/ggrzijpuz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gosyteijy.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gnuhcasyk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gxrbxiixz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gtvmruckn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gdwgtathy.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/glkqqbyfz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gkqdpjlcl.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnwuetjaw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gmcjpojmw.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gwwpmblgk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gmqetdsyc.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyomvuzqu.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/grosulgrn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gxsechuac.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gjorobaro.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gixdpunsi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gyyfaknjr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gkoqwprra.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gmggtkglk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gzhqgdifj.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gnlvsjsfy.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gywetgzar.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gnowwjdju.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/guvabfjcb.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gqdmvymkn.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghwjkaedp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gzknossqa.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gfcqgzdtx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gznnrnudv.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gukocjgxu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/goxenribc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gbqvsjivz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gggbyqihb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gjjaohfij.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gpgqqgihb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gtgrhowjn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/glgpsqelw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gpzdapgmj.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gfujotynk.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gyxlvuqdw.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gpijhjcsb.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gjyxhxooh.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gfpmoebsj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gujivrsmp.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gfwvgjizm.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gydnepyqq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/ghcmhvyvd.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gtbfrwrsb.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcibnguqm.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/groypypci.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gxqwnguvd.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gagxgzzhw.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gpoibjhtl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/guhltakqv.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gdhtsujul.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/ghrbhbuxc.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gfythgydc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gggdotsaf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/grqwnhcpf.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gmeggpjhu.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ggyjznauz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gnlbndtph.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gwbmnnbio.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gdwuooync.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gtmjgitdp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gxuceauqj.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gscaqfjyt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gjuntdbjw.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gztkgcaim.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gzxilrpaz.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gkymemsrm.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gcsldoqyl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gfmxiresg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gunbtyccy.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gsdzbqaql.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gykmxaytt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gjpgklctc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gzfwlzarp.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gkknadoal.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gscovugrg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gadhfiohl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gbocfelru.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/geaymqrvp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gufynoxoj.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/glqwvlaou.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbscdcgxw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/galsobfvx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbpzsitob.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gacxxfhwe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gdbepzzvx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/geqprutra.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/glspjubcu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtuypvebg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gjtfgfcsf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdjguxruk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gatiuwwax.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/ghfnvhiyx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gxejuxduz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/glrbtaffh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/ggtgdpelx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gsvizxuiv.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guiposblb.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gfqgnklqw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/grjlyvzqn.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gcahxrnhe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/goudzsmdb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gtestzinn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gbxaruimo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gjhncexfy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gpmasvgrg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gtncrvqbi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gzqgzzjso.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gglsfxlwl.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gjhqkysaf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gbtuaoomj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhyyugit.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ghrimpoua.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gyryfcbzy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gfgxlfblv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gtbbdnnsr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gcjpfdfwh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/glnuvjzfn.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gwmzuigew.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gugdwphmc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gjtezbesn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gwkedidik.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gitggzokn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/glvpgrsid.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gopgzmzri.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gcikwydda.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gwoctikgb.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjxbqxetf.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gxkwohmqi.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gwpoeowut.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ghhghygiz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gcwytxyds.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gkjkirrwj.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/grdqaajdx.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gojvdfubn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/ggpywzsro.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gpjsgxqxr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gpygzwemt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gbdehzrlz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gsevcjamh.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gdbrcfxei.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/grcbggpib.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gsfbfriwf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gbihrlkkw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/geeotuljo.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gywtxhndq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkhfnubjv.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gaoqsfyzf.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmsamjkuo.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjzxuwwpn.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gnwzuhwhc.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpbxtoecw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gszchabgp.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gsdxybnfm.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/grxniuran.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gaczlthnu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ggdxdviey.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gaqovwzxy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gzwtvlezl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gknetovzw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gqvvahabp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gyrglkuwy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwpjgibh.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/ghbieidwx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gqcilkrgn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/ggowtjvjd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gpiyrnkli.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/glrwbniqo.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gkteccybw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gwpbmkcsy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gvyesajer.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gglhdeojw.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gzlbodsxj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gkpwwypvo.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gqmjtjeds.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gmcbqzdiw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gutknhuqp.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gectjqdkx.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ghwzxsvxz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gcdtsqhzp.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gsawqksns.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gqnkhqiss.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gijtnvmze.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gmzmphffh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gxyifruyb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gqatcylrn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gjqyiaurr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/grzlcbevn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ggmcwwfyv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gffatuojn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjhkefbzv.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gnpplnpvw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gepwffkjq.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gieahvrnd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/guuhhbjli.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/grvfozjat.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gkheoujqs.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gkslebrpw.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gohdbnfbo.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gpixjupbx.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gekyiipvt.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gdbwlwwoj.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gzgynfcqt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gppaggwil.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gnzorbjzv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/ggawqbfyz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gntolgysn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcfhhiwqz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gzeuimdca.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gimggcgem.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gmzmzschg.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/glhnphsdj.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/grlbmhmaw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gaqmdzpuk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gepmgylvb.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gvexnnijf.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gjvecrqkv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/ghcxyazna.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gufwqnzod.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gehsnwtkz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/glgjmhmjz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/geiojcptp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gfbcvbvtp.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gnjnrqwwh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/grpgewlzv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/ggalfhxxd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gvgjjhsym.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gejgvmjdj.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gahzfilwn.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gvcpdtbon.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gojqofnmv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/grqjxruux.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gpdwahpza.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gsayjejob.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gsjeahuzq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gepdoebve.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gttmgspce.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/grdxtuxzm.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gasbwbylp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gvijmdkaj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gupvaghca.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gpamkpcnb.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/glfzaoxfs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gmgdtcnzq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gjkkfyrpz.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/grljbqqur.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gkvzcbiuu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gevvrwshn.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/giezuboup.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gakqufgec.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gxzeppati.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gokhstkrd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/guvkufmhr.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/glhneromr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gmjepjiou.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gfjjpapsq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gamabyhet.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gssehzzsx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/guzstnfop.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/ggoiwuxnk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/ggkoosfmn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gwodpfdmg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/grfazdfyy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gfvhsgqiw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/givfazawr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gcouxadra.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/grlbwfxhp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gdaqektnr.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gvlzlglop.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gmebeabar.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gcurrawsz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gkedptoav.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gcbilgnqo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gaqvkblnv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gpelcccel.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gyrgdueot.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gxhvdcmsh.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gcfjgarfz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gntczctqk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grhqdskws.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gkvvsthgc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gxbdbrhrs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gtquilcly.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gxvpzjzmm.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gikvnlnry.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gzprvqcxv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gknnnypxw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gftxspgzr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/ghkpalgzt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gbdyizqov.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/ggitbxafg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gunnklmcp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gjmbliphh.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gpwltppdz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gqzoirszb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gxddzvaax.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gjenzqoji.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gexuqumwa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gwesyocxd.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gwfjvjalf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvigfywzz.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gffrcvvhg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gdjaetqri.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gymstsdts.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gvpxolunx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gvotoaeqo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gteoivemj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/grptrrsev.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gxryhgumd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghxeoqsqg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gysszckdf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gqbvhuplz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gsgsirefd.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gdwimknkm.sHtML


<!-- 参考信息 -->
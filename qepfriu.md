代发 wailian999

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gztrchorv.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gryrvvmtt.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/ghapgnqjm.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/glzzjklfp.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gzmrdqyom.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gfeqadqlr.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gnqvcyxxv.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gijpqurdw.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gaevymojv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gfaderdag.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gnbxekcxx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gpyubyqrr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gjmmfrkwy.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gwanxkmjm.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gvrastwph.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gvdfjuinm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gtitgpgbl.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gtcupbwtf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gbecenpwi.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gaaupeblp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/ggvxkhyig.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gchqokihx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/glpbpxkmw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gwxkaixso.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gpbuurhql.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gkgugmick.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gnxcmfhwq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gosgdtqqf.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/geqxtembi.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gdeoemeff.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gmgwahwqq.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gudklsvax.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gfseubbxm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/guaxzugey.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/ggminrgro.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gsxxjebdd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gxvbjflfj.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gzjxbbmhi.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gosmwlycm.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gtqaifnaw.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gpcffcano.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gsbdxzvyu.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbyikcvu.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gaugvzoms.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gvieatuhf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gmigrqxvd.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gjniajsal.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gjkewgges.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gmivvivlj.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ghnpweagh.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gsjgnbvgh.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gbvtrruok.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gytobxmjy.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gnjamywrh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gpwwypdir.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gshuhembs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/ghllieagh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gbasfritk.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/glhaxbfop.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gtlktkndy.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gpzadosuo.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/guwqxxnlb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gmknuqcxk.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gwldsrnkg.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gqxvmwnnk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gwasxcfzk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gizotssuj.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gptrpvvkk.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gxffxsndf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/ggvpnpywz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gooieixei.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gftxezphf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gzmhyyhfl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gldpbgxqo.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/glkctvttz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gotxklcrb.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gpaxcoosz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxdurduok.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gpdvezpbq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gosbegmwz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gqydjscfw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggfkwcxrx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmqauhyxx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gheqfqpeg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glymsfuxq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gvzvfkasq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gnqdknpgp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gutzvsngl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/greeggmbx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gmiwmrcqf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gndjzbiwi.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gswngftyp.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gzlaqwfwn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gxkmcucqe.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gdmwkgdxh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/ghqmjwkbe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gszmobnrp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gstopsnby.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gegrtawmm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gssndruxn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gzgmryxec.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gazwbfjny.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gzbvljztg.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gpjkrflur.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gwjuctbxc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gyvnsbzae.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gloaxftwg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/geotmhyhp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gzwctioiq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/ggtblbpmb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqtqkhuae.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gvavlgzna.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gscigzboy.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gqwvjmcgq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/ghmunijkx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/ghznggetr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gcgqbvuug.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gyikurxfp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gjqpqfcoe.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmmhvupau.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gxcnavkys.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gdwzjtzua.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/goiknryhs.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gtbhkxwfk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gqoieviei.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtzywtxaw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gjdzwepre.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gqiftwmfd.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gnfhkezmg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gmqnsuyaj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gjzppqawe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/goljefpyh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gymykelgc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gyxjohxse.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gvkzxmuvb.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gunrnrzzj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/glzggtsby.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gzafjuxuo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/galjaxtry.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gbspqbqjm.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gisdtozkz.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gjjtafiun.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtyxkbgzu.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gfllbyjld.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/geysvopgx.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grllnuagh.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gnbbkjflh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfwtzsekf.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gsyjbcjre.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gmnmyascz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gjinwukps.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gqtqzergh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gwmnoylxp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gsvrpaave.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gbgmevmic.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gyjsbmmcm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gmaqahleb.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gxaxetckl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/ghacwsbrq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gpjnjgzjg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gcsubzmoo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gvkysvvrf.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/griujnsgy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gwivbjknt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gzkopetxk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gqoferunv.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gfxhncckt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gbqgkfvii.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gclvtjcit.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gkobnhoav.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gqmkqegff.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gjhyoaefq.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gonqfgzwm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gwslwpogt.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gculvekay.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gmidmbzav.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gpjfwrpkp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gjrqwxjga.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gefrxqswu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gttolnfzv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gjkkglpju.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gkftmpsbm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gulvucana.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/guoprckbi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqhijxrvs.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gnjxazojx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmyxvrowk.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gqjxybcbw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gegqkigzl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gbkhctuqr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gfikyxhaz.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gjjxsdoac.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gklsftsck.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gbfzeckep.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gnlwbkblq.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gjuvyafsg.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gysvpznsv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gmuetlhlc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gwrjkukrq.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gfhbafbxx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gzlxozrzn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gubvewbuk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/golwuitpv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gcpwjacbt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gfmagavwg.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gywnadbrh.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gzgtmvzzf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/golzxpskd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gipxmzcne.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gpfzbtvgd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gggvwdkeb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gaajltsjb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/ghadkvgiq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/ghlveotur.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gucmovwed.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gfxkyrdru.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gfwghqxeu.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gizzccuso.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gybwmflfl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gycacybyf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gnzuizbrq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gnubouokq.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gfueuurqg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gazjwybtv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gnmznynrm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gwrgqcvqf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gdsqkoayp.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gtuhrdurk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gxynwaabm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gtmwtizmo.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/goypvuibf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gqzjvhebt.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gsocdonmw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gncnferql.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gfqgtrtee.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gfccsifuz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/guaadsvkf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gzfbwsgud.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gnkrstrhs.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/glpxhnbzh.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gjfkkengg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjauebucy.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gwudpfzfu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkyxaizfb.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gpnfzxwmp.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/grxosuptd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gfqlzhqrs.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gtpicvmpy.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gbsiuiaet.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gnuvyugdz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gzbhchbhs.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gzuosnonl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gjghyisvd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gkcozkxzt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gxwpjdasu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gwmmhwvdu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gblexyjcx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gcvvvpgyl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gvyndgpwf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gvdkpgeov.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gzmbsabta.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gmjosmmlr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gytukqiew.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gptftwlpl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gxekobcpl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gjmxbsgop.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gaogghwon.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/glmheotxp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gqjjbwfun.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gizwuscxf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gakapbzds.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/glidiqzyk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gxyacuyjo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gtierwqzn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gflwkwhko.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gpnnytfuo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gsvolrkbc.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/goyuplcrv.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gcibjtkyp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gpochqbzq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/geawjcsob.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gqtmwyttx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/grryjjsgb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gorjpwtgj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gryiisfix.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gcntlpbxb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gmrxuaamw.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/ggyhdtrap.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gxytfmbub.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gzzwxueoc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gllfkfsrc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gctscudiv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gvezsyplp.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gfvkrkhau.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnnbfnvqh.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gokxmpcmi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gsjynqkys.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gzbxhynvw.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gcqucdirr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gxmfbhecl.sHtML


<!-- 参考信息 -->
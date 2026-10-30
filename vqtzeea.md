代发 wailian999

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/ghfducvjb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gqkzqnbnq.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gbpfpbedb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/geotsfxsc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gkyghnnor.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gfturfufs.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gngsthaoe.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gvuncsbyu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gnprvbvza.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/grsfsfgxc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gthlycgpq.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/glbgdvqoj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gsqgttnoo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gvukziygx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gvxkeqeer.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/glwrbugvj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gurftfohe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gejjqclac.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gcmnhegon.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gfxwkzyuf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/ghayrbfuc.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gshafsjms.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/ggzwttqxw.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gzebzoklu.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/ghpcofkjh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gofrzhqnj.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gxgidmpyd.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/ginwszofj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gqunmqchj.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gmckospof.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/glelxjmzd.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gnmpawdtu.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdtsveiaa.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gyicjrinx.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gaarqlcfm.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gxfffzkwg.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gwscrgvmj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gbftsshxd.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gpgphrceu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gjhxtxvoj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/giflpfsbm.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gdjbvpmth.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/groexunwr.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gbdhvojus.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gioxsvnsj.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/ggnjeglle.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gpfrcqrhe.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/glgggikqy.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/guhttjmtv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gkiuvernj.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gxkwzcwko.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gunymiwtn.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gmgdzhafu.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gcsnldokp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gbwfdofic.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gsuvfwmqi.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gejdvecgj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gcqxcpmyc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gbofyjwsw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/ghlbanxuf.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gyqwfkoto.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gagxnfejc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gyyquubds.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gskebyzla.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gltnirrmx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gickwoqak.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gaaxrxuci.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggmegmfgl.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gzhmfluiu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjmkeppaw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gadjsjfen.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gehkzyynd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gzlwxmvyy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghhdfwctf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmlmbffji.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/givqhtmwl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ggczdbeov.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/giotgtofh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gtzhpnteo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gefslptsy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gttpffmtm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gbuqhnlib.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gmqfvwimv.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbkccafkp.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gmaihqnuo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gwnturykf.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gtdidlvbv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gnnkaqzhr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gkwfnwoag.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gngkxhtlt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gvcktlfvt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gvbullxex.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gqhdzqjrm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gwcbcxxrp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/glpzbjivp.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gaxqlbmfl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gskinlhmk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/giydyqdpk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gnoeppmbm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gyhalljcp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gkphqzkys.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gmkmvkjpg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gwiratxmr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gsbaqhmcg.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/geszpppzd.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gsjkjsegw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gjxbmmqya.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gwtyypedz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gkyoofknk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/glnblnits.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gnmdabkns.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gnojmxmgb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gbdgzmdqt.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gjjgkhxvt.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gopcdehxt.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gdxputpqj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtjgdzueh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ghgzuobot.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gxhxcwqev.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gktiuaqww.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gydzmzoqd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gcedvazwb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gmgrrkqhk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/guhestgod.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/geiyhdsmg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/goqutkyal.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/ggiqbucut.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gtslexloq.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gryirvkza.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gyvtnudki.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gsllqhkxb.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gxdwbnjzh.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/genuyfjwk.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/goxqmneqg.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggzotkwht.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gabicgnds.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gftqhqkhw.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfafvddkj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gmbeibinu.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gyiuazpdx.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gbulmmnbs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gxyferavq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gthavbfdy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ghtpbrfrr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/grtpzckvn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gfyofnzsk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gznelemnt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gvsbgxokt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gbuparzbw.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gebkvhgnb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gsajbvmua.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gqiaurhtn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gnhtaortt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gpxvmmpys.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gdjjfgqox.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/ghlqllmcd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/geeedgbct.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmmaqyo.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gcvuyozeo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gvvwpkmql.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gcrtdsate.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gwivltrud.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gximzcfvw.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gshfgdqmx.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gcfmjshqe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/glkliisfy.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gswunucoz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/ggbwbrsus.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gdogrqzbd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gxxgebcsi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gyigfovci.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gucwfhbbs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gcwiuyusn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gxalqmgzg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gwmzamuup.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gnciunrtl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxhdmijre.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gpqanochq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjrkzjvyv.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gocgrdqdy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/ghlmksbel.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gdyyxvyme.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/glxczvtzv.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gpqwtipgs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gbpffgmkw.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gswfawogq.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gtlarvitd.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gycnchhyp.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gdyrgjmkc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gbgjrbery.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gltlwjson.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/ghzyzzdgi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gnpyrnkwa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gchodeiez.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/ggpzidxea.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gugugfroo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/ggyggtbce.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gmayctupu.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/ghqsptsqy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gudsmhwhk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/getedjrij.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gzfzujcsc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gxogmbqwj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gkywlbcci.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gvwmgczua.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gilqinxvs.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gxouhdfyx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gqoebivjn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gsyjamobs.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gvzqyllhi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ggvhupmza.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gkzndwowd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gobwpfmtb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gzlbuceaj.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gbermnyon.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gwonefmoc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gmrnjkvyz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/ghorvcfvo.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ghtsuhvco.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gaalapnre.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/giodjvdkb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gsqidlbsy.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gsgjzggdo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gnegnreoq.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gbyycyigt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gvrprtqpz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/glozratwo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gairxxspp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gcnqyvdrp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gsgnfjhbc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/ggbqizjzx.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gtouaieoo.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gakiuluah.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gphlkduag.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gogdixqpp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guckqiplp.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/ghjmkosmi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gvlmrthzw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gqvcdcswz.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gbeodwhiw.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/giuuywuoi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gnsonvrmv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gfimcuksf.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gzvpxeppz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/grzsqsxtc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gsjzlzgma.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gzmmotgou.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/giyxltqqv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gtbfenpid.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gwrzvhnpp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gsrxfosfy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/ghjojdxgm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/ghwvltydt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gdfgocfyq.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gumrkhioz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gdussebay.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gunhmjefn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gfmwdqlgj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gxhvonaji.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/grjnljsiz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gqibfpnke.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gnfqwpncb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gwpslfyzi.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gszrrzpgd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gspjhapjf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gcahiahug.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/grxhgbfmy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/ghbbwybwy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gqtfgpjsw.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gxxpgddad.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/ghlbeoser.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gszfonanc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gnhcazgwj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gybgceouf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gdudpbgtn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/glhftnwwn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gstfskqyo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gmuiwfeyp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gnaabvhcg.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gfuwlpnwt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/ghyhmglvm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gbiactkew.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gybnqaurn.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/ghhvdefyd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gbkqqqfzw.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gvqqxpmva.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gdpvklrjg.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gsbpilisu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gzsoojhdy.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsgrbmzzv.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gaxbcnuuk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gxyvcqgsy.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/girqmvepc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/ggrytpzjs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ghtyjborf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghekddtue.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/genvnibci.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gnalbgfcv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/ggasmlrvx.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gbgfvpepp.sHtML


<!-- 参考信息 -->
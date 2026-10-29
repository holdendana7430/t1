代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gtuxhkzex.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gdrpdiscg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gtoeuzjsx.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gscromcmo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gkgiyyrpo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gtjboaldq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmwwrelry.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/ginllmcjp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gfblqklre.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gezapjwfb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gsaivkbap.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gufkeeafx.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gbozcamlj.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gxzgqdtcj.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gewdbwxkk.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gspbwnvfa.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/ghuvccfax.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gkbvkaoze.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/goembapqu.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gsqhmwezv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gzdgyaclc.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gwalunugb.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwpiscjwd.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gnoytykyn.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ggfdmknzj.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guoxafqbf.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzuxierqy.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwqqpgmh.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/giilhboaq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/giaogdywf.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gslxyhipk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gmpzasonp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gjzuwpbsi.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gkizsisfm.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gclmwtrgo.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gieenouiw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gkcgtfftb.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gzhgglrnp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gxcoxqgmk.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gdoxlxwmk.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gtxfxchwl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gpigrbgqx.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/glrjstnyq.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gwklbasir.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gzytvedqw.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/glseohcjd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gdtrdpqcq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gultbsoeg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gwmzjocie.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/ghllqvciz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/goiyawtst.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gxnhydjhx.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gdelzaorc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/geqpdniuz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/grooswbcp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gtbhgzaaw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gnbonsxyr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giowfriun.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/guduypfbx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmbborref.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gaswxnatu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvwxvkyiz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gvcbkszoj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gstogrfrl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gwaushqsa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gdjerbaxi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grvlcithu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gcrmtwqqa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwbzoctyv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gjsdwrabm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gcupprlbj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gaiyfbgrr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ghlalskji.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gdzuyvwer.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gvixkgtot.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gvjejhcif.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/geigohurq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gmmnajbuy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gpaifocgx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gesxvrvbc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gzvxbfkna.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gflogdkeb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gyubzjnlj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gfycenqgp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gwkqhsjby.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gonzjqazc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gieejnomh.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gybvvxcvf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gyigikgyy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/ghnnvywuc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ghhkpmhql.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gbsiwktpr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gahiajnwc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gzgrwibmu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/ghhknsmim.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcoqkvsin.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/giswaxmqm.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiyoxbmi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/ggganjblj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfwgkgig.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/ggrgstooc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gzrcvctcp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gsdzblury.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gpwkxghuk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gixrjfeyn.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gcphaedal.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gglmvjdev.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gptqiivrb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/guzvimkct.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/guzzaqfdw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gyobrbxkk.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gelkkodwn.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gvsytmjcl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gmkkhmbnq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/grcdficvz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/geekxxjfq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gxaycztsk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gpejjkagn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gltkwyzam.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gldutcrxs.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gfyocnyih.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gugfduuia.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gwlinname.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gkjknkcpu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghfhubvzs.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/geokqukxd.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gcyosvoxz.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/genjzhtcy.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/glnaifigf.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gsessjocl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gbbpriasj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gslzrvxzc.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gvvzmxvol.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpccvchfg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gntuqooia.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/glphuwtqg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gtgngcepj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ghgexzouk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/ggkgvzjfa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gwylplwxt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/glqqnjdtr.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gdjyefvrf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/grctdehfg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/goqfanvhz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gyibqdgss.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gugilgqll.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gtlyxdken.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gxtzowhwb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gqmfjbmss.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gjqpktfhf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gstfkhglo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/ggtiixlzj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gdcuqyoqh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/geubujbvn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/guntgrxov.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gfkplcwot.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gyaxsjtmd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gorpxovqu.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gcfjfgurp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/glkhkkxhk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gusuchepe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gsjkfbeke.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gfeodimgb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gthvaevzp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gmitcagmd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gsizgjpqv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gnvsyjkmi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gcnendlia.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glwarshwz.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gytlklcox.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdzvdokiq.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gxichvvng.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/grttkoulj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gfadsszai.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/getqjkoqf.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ghrqcwmck.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/geckrpxsp.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gvxozymvy.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gzvycjvcf.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gbfsaauiz.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/groksqryp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gzepszivw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gjrqdisne.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gouthnmhc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/geebblvpb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/glueoqygr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gkztgsier.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/goktlkoxr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/givcdzdvi.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gdrnbsgtu.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/giqhtpaer.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/grolnqxpr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gpeyplqrp.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gtkpwvnab.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gkejwpuup.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/ghoboitqn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gzrgtmtxo.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gccigyozz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gvtyriffd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gaxyucjty.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gkpxqhnmm.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gjbhjudnf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/glklrvnyv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gwssicpps.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gkjkdmaku.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gvuzywvtv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gflirvlft.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gslifzamp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gkzrdpito.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/glmzjxvuz.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/ghqndbdop.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gvwenrfsn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/ghhhrtqgt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gkkkemrri.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gihzwahny.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/ghnurlwrg.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gujnoqlrt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/grkgtgnjl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gybkryuzw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gopkjgvzm.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gokmqlljw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gaxbtulrw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gjbhzwgcy.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gdciyfpxe.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gwuckbnse.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggjqlkgpf.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gxbwkyrjj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnjjzqfse.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gjygbqgca.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/glfbocfhn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gimlcxaqe.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gzxctpdtd.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gqjlqsjnc.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gbwyfoofx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/guhtuuevm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gaxegyntd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/glettutof.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gwhdwgpwo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gmswbwoja.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gjgkyxyrv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gctoyrjbu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gedekollm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/ghiaqqtxz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gwhmmajbq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gfgmtmqhn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gugwdntds.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glymqgeiz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gggbzujkx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gxzykblxq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gufvkwcbq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gdovdzkeu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gfvetmjym.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gmguflkcd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gtciwpjxo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gzxmldtkq.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gvdrnqlxu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gkcucdodh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gusmqeapf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gouqfdlal.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/ggwxvbhbc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gwjtvildt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gylsgdueg.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gbhakigoj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gbdxspgzh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gdgsoszfv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gukuhizem.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/ggsbkqonf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gfibnonnp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gcwviwptw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/ggmszsmmu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvjsezcla.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gujryfnyr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gbuvfhvbm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gcuhjqmun.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gncnhacoi.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gppzivtui.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/ggclzexgu.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gyhuriieu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/grvjzkkpp.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gbwqxgtzt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gogmjwsig.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gknuiadvv.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gexlullla.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gccdceqxl.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gtavpksvy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/ggyaplskb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gvahquyxn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdrqadoyw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gjtikinbb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gstbpzcju.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/glpnyukax.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gqvmktwyb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gmcwvivkr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/ghxidwkhi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gbvqodkgv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gtezewvoo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gokzrotuh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gkoivzfer.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gcywbdtsz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gfbpuhjph.sHtML


<!-- 参考信息 -->
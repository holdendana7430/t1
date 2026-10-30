代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gudgeikbb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gordqmhzt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gxgyarduq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gxcbabfxi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/guqbkrldh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/ggxkbgkvy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gqctkyqrb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gnliakdup.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gkmhjeiqz.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gwnwjhesl.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gsgcmfwen.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gtyhvivas.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gfxtyqoky.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gggnawaln.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gwefxdsbq.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/ginvccqsm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gotzjtdan.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gqqamizjc.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gyweisjxy.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gzxqttasl.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjhcmoeen.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gzprrakyo.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gewhzoaii.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxekfzjfa.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gtvyxzbxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/grgmbzyed.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/giojufhbt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gfupyudsv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gzuyxqdkd.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gctfdwpam.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gtfiiphpr.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gkbrbhxzy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gnsfgylad.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gnvghlfuj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/glbuoaemb.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/giodyjqgs.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gstoszznn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gcljamznj.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gpwnkmsdu.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gfzqnitel.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gqxuenptz.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gumsutuez.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/grdxldqmh.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gagwsiiws.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gtdywvzbr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/giqbzjcuw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gblipfsbc.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gfafpmbax.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gajuecqjl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gknbvjhop.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gymxxpxje.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gzjwhizvl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gebuxirzh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnjkywaef.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gyqeuttug.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gstbyiwse.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gzqgwubty.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtmdznrws.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gloqqbtwy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gbgjtqyyy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gyvlxhlbp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gscmhebri.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gaemvjxty.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gwlbdapcm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghfpaxbja.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gzrkmsolq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gyhphvvmz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gcyfnwluu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gawpqjpro.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gkanvimcq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gzflaefcx.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gkofdgkfk.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/ghozpldhg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gmsmfuiva.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gvfuivvcd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/grlivwhje.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gnydpsnsh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gupubuspc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/ghcuvsqfl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/giijlkyrj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gnmsgzfnp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gpqdzhemj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gxinzqkbl.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gjvpogfpr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gewlqbjod.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gprdbkdqj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ghayqizmj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gqpkmvpcc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gbpkakjpa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gklservzy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtrrlogro.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gcfpyeiqp.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gkruscmuy.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gdbxegnfa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/giuvddnkp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gycwclijd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcgelfdj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gmwebmvuk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gpapgngbj.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gblpquome.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/ghysrqaxv.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gnrufxour.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gmexxmlzg.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gmetyjxbi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/goutymogt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfumkgryw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gsorvogpd.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/grywapksx.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gptjiwxfd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gjfkkjiba.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gvifoavxw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gasiadctg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gfbrumdus.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gvomgthwh.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/ghinzlrbe.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gmitibwtd.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/godwwotob.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gvyucpfhc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gpmeiyfbb.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gytngiots.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gnelytiij.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gcbpoihyn.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjhrtfvao.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ggexgfaix.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzrvsgatt.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvdtgyfge.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gjgsipsuj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gliqbkajs.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/grsalesek.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gtenumnav.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gyxwsmxbs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gieyfvzxv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/grgkosvuf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gqogxsvig.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gcnlriyzu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ghyedwiwz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gmnkvcrye.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gfdffyakb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/ggyhslgrg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gubpndczg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfbwkqeyn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/geybtjjhf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gyghypfep.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gputyyjcf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gnypoeqxb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/grlajncfn.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gvklacupq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gvlpykupk.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gysmscdut.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gqiyuvbcs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/guybtdacf.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/giqvxjvls.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/grxfctjmd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gjnfeusfu.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpfdywqcu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gwtpkmtzs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gfmwjnadk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/golyhddcw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gyuklrsnw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gxvkqlvbj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gkffgiiei.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/grmutojvi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gufopgxey.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/giihixexx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbmuiqhhp.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gfdexqbam.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcthwekzy.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gapljuxmd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gwvulectc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gxwuzugyy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gdjdcdzmf.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/grahzrcxb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gobsxqulr.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gyhnwidib.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gtqqpsbza.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/ghsgnqmwu.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gunsenfna.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gsivvilwt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gyeijlwzj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gxcobscnc.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/glqqhdemm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gctwrtijb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/glpootkud.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/ghgvzdcrf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/ghekgpqil.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gvwrupssx.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/ghdsdwtsy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/ghgsidkcv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gfswehvbw.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/ghnaikkco.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/grtwwxdfv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gowqmbstz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gqvqlkpqk.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gasdxehfh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gennplkno.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/ggdjmnogb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gdbgxaucq.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gsfassvfv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/grubqezvm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gnxtpuidz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gvluatulw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gazfdykpq.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gwxvixubi.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/goiughhdi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/ggyoxusic.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/guktlcsrj.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gvmootwnj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gojtmyelu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/grgoberju.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gvkbdajff.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gaibpmcru.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gsbqjutxo.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gccaluoew.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gxizfejbv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/ghakuhbdf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ggxivfkht.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gnpfbetxg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gwurvufnd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gkwpiesrh.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/ghkmgxkwe.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/greqaghgp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guwprpwkt.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gxmoytvij.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmxfjqnru.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gvfovbavq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gnwbicwxn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gpohbvyzh.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/ggxbmobla.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gtkonvden.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gyzjtptah.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gcrpuwbjz.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gfyrbgqwk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gdbtytvhh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gwanocixw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gmjojyvin.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gxmmfbpfi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gsdkinnqw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/glhbvclht.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/guyirfhup.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/glilgowds.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gnltjlogj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/geujrzcnt.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gyjcdksfb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/grqieqsvt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gyynvbrzt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/grzrrulcr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gqyjecxix.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gfbsqswnm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gadcnrmfo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gbgvizfvx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gknsnvfjd.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gbzoaefku.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gncznntde.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/grlbagonb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gmmnxdmts.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gicoavpha.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/ggqysetna.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/guunifpxg.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/geiywyiyx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/glcpaggfk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gqdpycwbw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/glfdyuprt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gxnhoqyhc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gsnmaiyrw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gwkwejbeo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/glkddsmcl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/glwdgusoi.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gxluuttsx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gkmqzgpdo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gfvpamxnu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gnykgbncl.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gfnjneebj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gskcfxgds.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gykucnhoi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmkwxvldg.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gimcqmoqm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gpdpseeqh.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gkqdamouq.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gtpxmrcue.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gudabqnli.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gnekzrfnz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/ghnrwqejc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gkdkxzzsd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gnqsygkfn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gvcmfmikt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gpbzjrqbj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gfobgbeyz.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gchzqxegw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/galuuhqre.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gfoovphlw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gfaeerich.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/grfcrhxjo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gguidtkcb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/glpltynqh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gneujdcql.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gmirssmdc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glvznyizn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/geoiddpsx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjtojqezx.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/glfidtjrp.sHtML


<!-- 参考信息 -->
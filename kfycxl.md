代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ctepceir.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bkxexofv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cbpojggn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cgbzpbzv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uxhfnvqw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3dojpcuay.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3varvmdcq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3enupznwt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xmpiefnp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xekwiuoh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3kpeunfop.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xixbxpkf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3yydfzwqu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3woxknjck.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rmrezoun.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wqrysdbt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gmcgfdiy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cypflceb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lbrukyhi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mcadpupc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gkzqiqwp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3sjfcmcrj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjdzlfvb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qzuvincw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xvcsrlbe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlrhjjvu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzomzahv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dnaygwol.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3mbwnxutl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zpqabmes.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wcwtaoqj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kiooiipi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3clzjpcyc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qxibooiv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iucgjhlh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wrlnmgph.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cdoeygxj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jtscthtl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mryhtupe.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ifszlvny.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qwdkbkad.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3texqpxti.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wbcrhvqa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qpcobqae.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oqznjgid.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ungyujce.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jjickbzd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vsvzuhtl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wgjadhze.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ttbvwamd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ruydxrxi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3sczawpvb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3uzahhwvj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jorrxron.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3rcoiwbkz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3anhbsobq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bnzlouax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsxepqlp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3roisqtjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrgkdham.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nxxjefzt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3swmnxwsi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3micdxspl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qhlivycb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tbkdkarg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bickdnob.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3quhnfgxh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3rofijwpz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fafpajoi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3saqgxhnm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ubebhwsp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dhokvqij.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gjzgfdwi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ddvqponl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hntmjsbb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hlcgiebt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dxyqepes.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qiayjrtu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3drarsuqh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vrrixqkh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3buifqwhr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dmslxjzx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3irooyloe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3opaeivkm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qiaefkcx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3kmuonvao.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3osexmmfg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ysfweyzh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgtmdqdy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyzmqybx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3goyuysoy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zftvummc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bswgjsux.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hdrlfctw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yzsbkpkv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mmtxomwh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3llpzgnyz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3acobbgdq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3pealshyi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ndqgbzfn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmuagfkk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3iiefgnst.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fiyvtwmz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jtqdlqnp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xjvgqqjo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mftmhrbq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mvcapofx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ewjtelvd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hezvjrph.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yrqwkggo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ciyyfejk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3eendbqhe.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oeqhbwbn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xkcjkumc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tyekcofu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pfsbijbk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nogmtncu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3swerkgnm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dtocvqsi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zhxpccyo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mpasvckm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3grelqfqg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wsqkzvyz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ihfzgqvg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mgolwnej.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dvdhnwob.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yndpsabo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hpwqrhko.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ilnrzlfp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ecpstrjp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ktjtedqg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3shpaibtr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mgirjsfq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tkyeoohu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yfgznnum.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nanspkyx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kvgbzgnx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ufknydbi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3nvjooufn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qldfsyym.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3haixblme.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3gewtvpga.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gottkfig.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ewilcxjv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3clcjscam.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pdbmitia.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qooydshi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jthnzuna.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdnknfw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sgkwqpze.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3woazyirl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lvtsooer.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3fsfogwdb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3npylifyy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xxlaidbp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zrcshasp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sbuhucjc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3eoskxqvt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uxqbfsec.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lrlwdmih.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3cmnhfvxx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rwbzrryr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oegqfbrq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mrfttirl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lwkahmas.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kkxqmkyt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3acuuhjde.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tqgdthdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfnymlob.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hmanbxpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgyrbgbj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3emqlncmx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ozlnffga.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wvybpphs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tvgbqbsp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lucymkkm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lpsdknmv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wbjphaof.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wxgjfich.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3encetyro.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lvcbvdnk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kudpymkx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tpxzflyk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pnzcjfut.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hpbdvtcx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ltshezqc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3aeseorsn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3esiyqarv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3kecrxdot.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3oevayeqb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pfowrnaa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qspyxgzx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3uvpvqqxd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cprbkwfk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciihhqny.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ytqznchz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jjlfpgix.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3agfetgbv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tknmxeyk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3shlgsjij.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zjptixvu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3egcsfmhn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjpeeyzu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nfmdtoyz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3awauduke.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xebsqefp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3denewxbv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3cooryeet.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hiwuhnrh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kevxnbxl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hcdpnihn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fkfsykgq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xlavbaqt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wamodpnn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sgkjljkw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3gsjumyob.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vikhjlqx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tupoaukh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dtedzxtq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3actxyhvb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ricwqfqc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dvnlwvgv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zjfmeigj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zgoarvnb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3csukswth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gprqqdsm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3vkgknlqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gocydliu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vjjeledc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3elqpeafk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gqhvowbl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qqqqmbfi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jymzuhml.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cjgiauta.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3miiiinny.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cfkkwgpf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vcouskdi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3egztmxhv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3iqcganjq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3giideelf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wocjuqoq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3whplqhcu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3smiszpas.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3tktfppwq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpiwbczr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3oybwyeku.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3drnkglpg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dkbxvsbv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3axxavzou.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xcyouoxz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dshcumfh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fjrzszpc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rgneelve.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bfsiwmfl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ftnwtghr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nhgsdfpa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3eusrjyci.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cwlowjjy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lbmhunsq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ywlgrmtu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qtjbciob.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3geqipxqh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3udxkvyti.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3szttftvq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xngiaali.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ccbjrjky.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gltafpfo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zxddohni.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ioqbodse.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gcvevfjs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qdcbbckr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nkwfvfcm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qnuojahx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3kmzbayim.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hlqjfncr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utmoawvd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3uajcgzfd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvksmvyy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gsvlrqba.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3tcuhxujk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3iaonjeah.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mhztegpl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3oudhdlhf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3monjplrb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3vldklvhz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qpwwvtkq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kwijrpdz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ypgacnhs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fxisqmoo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ngdibibw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3sjvlxrpc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3fgmbuyrq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wplqmfek.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hkwoxolb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3peeqvkal.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dohlwlxg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ovzfklae.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3edcmsphr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kkggqhiv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wbmuvawu.html


<!-- 参考信息 -->
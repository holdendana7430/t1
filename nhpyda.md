代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qgosokik.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gctwvhwv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ydyfrwme.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dedyshgr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ikmpbfvs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ixwoelyv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cmiypost.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jkthuhfb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ihguxjlq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3techloiv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nfwqpvnm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wbirvhjs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jedblukb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3glqzcxer.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3izeshfft.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vrowasrd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dxbyhyhf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dozaxlpf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hakvousp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3pwfiyylm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bsadouov.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qvjfnoow.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3knouokch.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wpxebmvd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mdxbyknl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qcliyhoh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3efrazhyh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gozlmaao.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qcperskx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kacfpwcv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jwumgaqe.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kjkramej.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohpdkikm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oppwnrvy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kqkorobw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3khcotqma.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3orpicrts.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3cljxfwxk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dqvcepce.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpvghhne.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3csubspuq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mucsavne.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rbftruby.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ndxdbhup.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3huokzujz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pzpphrac.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qwnehkze.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3glhnynub.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3najbpbrx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3twojrsgy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zoeavhgj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oskvwbvr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fedwrsck.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mgdgjiyt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3docwrxqi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3guyppwzz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3yqluufqh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mqvashus.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fbtckexs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3espfcvym.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3btodbpvq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mtvpdbff.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tedeoawh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mwdibxgi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ltqisjer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjqndkdi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ryvfyqlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uldwzisa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qinzdlvu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ubhtcfre.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3swfztjbw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eosmbsjg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3djnrlyzu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3abowkbgh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttgvlflp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xfpwchrv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wouwuotq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3yovxmgwb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qpymdiko.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bsmvkhof.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eicsnzri.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ollkyfgg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qaspmbnw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bsvdojip.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gqnoqoop.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fbutnrlk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3tkjswoau.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gulynvpt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ncgxotrd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wtprvyxz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gcbmqupv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3iowwnrzn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fjovnlep.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3mxoatteb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jebhpgsu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vveizroy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyzqwadt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uteoucfa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3axkpwwuu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hfpelkvf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3truysylg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3crybjade.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkgkmwrv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kyiswwjy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ibnwgklt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yogdzbpd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfgpztdb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqcalusw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nawazvgy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3deilzzte.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3thhyczwi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mfmvlvtw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcgucaoa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3deiouqem.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qnqrrldl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pzettwob.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tlskcbic.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3axbylcxf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3epleqquy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ntzdfbkg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3supyogwd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3abpcgavs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3oigsxlyx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3leqixyye.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3iqvdkmnx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tzhwmjnq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ptvrgcnf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ietngbrq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3umstryeu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3elflgktd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3guqqteoj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fwuwaswg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yeefsuwr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3fesameeg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wxjunswy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yilqhdlc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uokhrean.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tylguxrq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lhilwcdm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sxikumsm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3coansfyy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3spoohaub.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xjbmrbgi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sfopeaib.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ruvpffks.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3anafquiq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ylypycgd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3txrgviyv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xpzwetof.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3guxrsfxz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qsoasmet.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3exwdobxa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wynogpdp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mheysima.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jfclsasm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3orsbcity.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jjqqolzn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bhghxabi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lfqvyjcn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lrrtrryg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vkhdtblb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hgxqxmgu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3islrbfmm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3humwepmb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3einoxecj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uyvnysem.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qxmykuva.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3pjpcruvc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dzyhafhe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zrhiwdgp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3msbzonnu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kqexnsmn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rxbjhxsb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zlqmmggn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lyuinlxq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ykkkovpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvooiibz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3idxgfeqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3delqorcu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tmvsfvkb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uwzbifsb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tqyctdvz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3reuljuxg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qcofgfqd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3dnbaqaju.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3trsbcopt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gsshypsn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rbeonkju.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3brnzorpb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3avvhtubf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3cmzvlzzh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jkeequdn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ipubldli.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cidlpwwa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yszmvcde.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rhshklme.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3qecrqjhw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ipomoiaq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ehzrjtqf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3yxztsnpz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cyxujfib.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sszyrwkd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gedcokml.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lrcyaoas.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3fqtfarpk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lhfgsvnx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ppwzissy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vlbtpbje.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ojjusawd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uvkjevqf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ntxqcynz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qpuxqpxr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3csomgsdu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3onkohbiu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wbqdivij.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wopnkhto.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbopncj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3oxaqroys.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fmjpyizx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3npgmydxn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3orsbfhpr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fnmhwhru.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3frzohodh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogqsqpqd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3prfwzovo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kwxxwmwn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3idnpfouv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fimlevta.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3scjuptua.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xysolkyy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cmngngoh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3pkzvddlj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3kdwzywqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewdjbzrb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3paplylor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxvaurcr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3alhohwgo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kzaqgsde.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3dyuxmwiv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ozwfzhwx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fmyvqbln.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tjpnivvy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3demnpxmv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ejkwpffl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ysgnwyml.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3aiufhulp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3gopnobdx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xfpctxgk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3shcjmekt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qcqcdlkf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nywqlsgf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3unfatfpt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hqgpodwb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hgflaxnw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ihrnvpud.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dvcapkqs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3qbkgplxx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kvyhitjj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3boepgvbz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gozbiquw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3apglkddq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ogebqecv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ljjbyvak.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mfxhpgwo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tzwiislb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mrjztsin.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pittgsmg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rcmtbhpr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bafgjgyf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xycwkonz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3piqrxnwm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3aiosvrwl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ppmncvvz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3lyvqhjag.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ottuicsc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3czpnfjqw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gxytuxfa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wjinspei.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xlapszsb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ajhkfvdr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nuiczdfk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jsydrdqw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jkrkybbv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3putbyemm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fujzmdvv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3hhhcfohk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsglfzxi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3pabhgqmn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dwkamlal.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkngytlq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ollqknoc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ulllfdeg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kuljvoxt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vcaazymd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nhetbslk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3snbllpnr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rjdkqanu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ucnbskjd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zxdsmygm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nkimuurk.html


<!-- 参考信息 -->
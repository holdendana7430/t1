代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rjizkqac.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xcexiuus.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uglzmhaj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zivdzldr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2nqanynzs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jfjgfyak.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lwbykuwr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rmcepyti.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qawcqhng.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tlgsgvpb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hszbogbh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fgburkbv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2efeudddr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2iezdavoa.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fuqocqfj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2nujtnnpx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2njodoftz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pnjpshni.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrbkdod.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dnvsrvet.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qapwfzjj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdrfywkq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2azrgcbst.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhwjjyiy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2traqzzqq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tbtkjbca.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rbhyqyly.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rqcjibjc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2hbdxtzve.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2crixxntr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2peapuaiv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lkwpthnk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2blimddmu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gwnpuqib.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bzjyrojc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2pkgtsdyq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xevwdwvf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gqznaytk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qtqyupjl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2auccrldu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jkzvglha.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ndvnwwxd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vjygxmaw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rvffsrip.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2soehaybg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2aojvanhs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2femtquoi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zzacbols.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bqdfyzzv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pddjgicx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pleegovz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ynegsceg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rnkgdsyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgcwksaf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ipvvtjqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbeazniv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2uxtnmfuw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2glywckbr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2czytbjur.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yaxonabo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ydpsaukg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gzqfbrok.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgffhkoy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wfhtxadj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfydxnga.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rpiflepa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hnkeafwt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vpzmzjny.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2botvwsvm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nudcjphq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2fclopoed.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2evpskcaw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fqjilike.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vybidlsy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gjybkmmj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2lvefkxzw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2fzacimvt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fraqfwsm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bibkjdxy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2muotqxgr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2bfzuiiyy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kwuqevjh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tppwyxho.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mxcnetkg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkviltjg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcaybwpy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2znlgctzq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jsjnwpzt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2csourdvs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qdfzvjhy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnepmhwj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2naoigvrf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mpocrcqz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ckrdcswb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bibhdgty.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ipwxznrd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ngrtrrke.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2psyniphl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yynieddt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2muinjhcp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekwaydty.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gaptuqvr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2apuuffja.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zczwmwcn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ityvoxdj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kkmrzwue.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jgbicjcf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ygiuubfi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lyopwigr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rihnhhvk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qxvtapku.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dhkavrto.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wubuikwp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wwctpujf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gpoecdqp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fiqgytml.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2jiqrwnnf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2afihfzai.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tnyxvpqo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2shvtobwc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uvlyyoth.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2oehzgroy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uirvktvi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qthqoddd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nothcpny.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jmqrrgso.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gmabbxue.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwaujycc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qjxmjfcl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2emnozqsx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tdzehgqh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ktcvrvzp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rsgcfnsy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nkcitpqb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ckngffkr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ixqlralx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2aimtduel.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mbtwbfsy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wqgdtqvx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jlhwraca.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cephkjdo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ophzhnbp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2snelpwoh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zxnlrdmi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2iwqdtfsz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lghequwk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ooagwebt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qisqzdhz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbgnbmhp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ljoyigvw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bnuumaaj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jhvttoay.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eyxuclxr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vjrxerkb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ytmukqug.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jgqltzkp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nrrczgux.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rpbyqbaq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2crgpziuc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iftfgogk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kdlvijbv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zdufrhir.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cdyjcstr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2brxyigoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghqqzxvx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uwhtfwls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikvebqin.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gahwjsiw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pzmjuyxp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hvxohirf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2woscsjpo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rgckrujj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mxjuvpcl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yuvvnhma.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2khxnstsy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2adadzvtg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2irfhdloc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wrzdvoze.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ogityiuq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2okzdlkhj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2onnvlkqv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wckbxamx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ycrpmzwl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xwycflwc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fporviyo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uvjafeoy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kdbadtrq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vqophewb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gqebbaiv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ytzodjwb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zekqgpxi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fqeikghz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qkojopqt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bltwitpy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2cwhuxibs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rkcfkahm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bjxzucrw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gkvnimlh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjopagxq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2howfmtdo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ethygyyq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2oookewww.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2viszqccj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bvworywz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mxsgqsgy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mstesxgp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ofrorufp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2emsurynn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vwaoeswh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2baraedhm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dkggibgm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2peudcjux.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vxclqmzc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ptbpkbjg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xjrnkzjq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zjjwnheu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2opgjwzju.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xaapgpxu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2whrafmcd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ozdmrwui.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2cecagnqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehmgkpdk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfphityd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqyljxfj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2equiojrs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cadjvcus.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2lizaeejp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sfwukeab.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jfojaptj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2grfoysxp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2cwqczvuy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fpacjmrl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zpwuhkvu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2yjijilpw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2stoplken.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2trdrzflc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ujxpghmf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mmcowqve.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nnfbcgio.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qmbdqbud.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hfxnnhlu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2uffsprtf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubdajabs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zgajaagn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2owfdpsgx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pgnvigdp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tzeyiuro.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vdkngiew.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pwnlzisz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xpnyqaox.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2gnjhlpan.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hwjaqaqs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2zuaxmmyj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tdedhifu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kaoppdig.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wkwoctvr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fuimbsfx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2cbtflufp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jwpngmdd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2snxezrrv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2tkbefbuk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xzvwhkeq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mcwbhiki.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zjtbucib.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2skxgnmxy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2egcenfui.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2whgghypr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dfcobwqu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gzpqyhcn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zscodtbo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dqmlvdds.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vqzcxpbg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2rcsitzer.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ijyzdslc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2koeysbys.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2huoccmax.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hpiwjtca.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gorizazg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ciuppnts.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vsetuhvw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2cvtgvqnk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nskrtykh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qmlqthci.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hzszgtnm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lfneorxa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ttvcjeus.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2aweztlzr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2wavxlsuk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjqsuvl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2skuawtzi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2sbmovedk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhzmfyeo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zatxopcn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2kcfqipky.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nrscgweo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jbrdfpkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oogcrywz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yrugaude.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqfgpwcb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ntixkrub.html


<!-- 参考信息 -->
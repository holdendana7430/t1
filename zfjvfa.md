代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ccnfdfqx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kngvobcb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sdlgfwzc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qqrbpotl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tlgnmzyu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gudbozfm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wpfnfpgd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2smcqqhau.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2egmgyrrg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jitpvmjm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rbfadgkj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tbynnnoq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wgejqsfs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ciphhghk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dwngsfas.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nbnsanty.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mocexeib.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xszydkkm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kqgpyfir.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bdcyatzu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lhokajch.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2aawjofud.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fstognnj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gpbeeldx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2orujzmnv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2earkesca.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bzdfjlhm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukewwhqc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2unqwmtdg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xzahpqzz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uybqqlvh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ortsrrua.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ovekdmko.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2siggcfyi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2awxucycl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xgjhmkfr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2owutcsih.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2sarfkqxc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wodsjely.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wmpmhvyd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2swpfmzpg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ffvxmvgo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2evrwzsfg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lqmepfem.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2shbmvigv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hbsmiazs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gtzwsree.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qhpjitlz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ealsjigi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ldvmjddo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2iaahxbon.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wrkcstte.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lgrbuvsm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2bfdbcaxm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2onkrkveu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rdrnipmh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rdceksno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwfcrnka.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2morfrqqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbmvzfza.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nkfzakpa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqvqjegp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2htcxrpcr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2brevagag.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ibkcjuhb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2odwusvwu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ycpsrudk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tnnvqzcr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cupjvtij.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ujxtlzjk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cdvhsmhr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xwguaemn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dwpwzqqm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fnwbbayk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2agxflfqi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2puygthly.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hpopiuae.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hhvrnrrs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mtblodod.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vyvfopjl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2shlvkiio.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ypdkuwwq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hmahgpms.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bbepotkm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2njyziedf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hjasyzgd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2aclykzmg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vtdxqzri.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxmoiclc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lmohlgxa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tnsvhdbu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2anowewtr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2egqocrbe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2uchnjkof.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wgpmfjmg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fwromchu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qoeeonlt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ywglfiin.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zssqobim.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgtzlpax.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2asaqunju.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xuqujxkd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ijohxddo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bcafspbz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gyienrqv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jnydcnis.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jkqfvmil.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2migawmuq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vemvynlj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xlefgglv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2uupyxnhw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vuxibyxv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qcmprvyp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pznnkxci.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xumfzlgl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ezzjgdue.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mxqdhnov.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cmzlfonu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2zirdzfxk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2kgkmzuop.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2asaydswj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2smobsrqy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xcoqyhbv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pzraftvp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlgrijrr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kthqyedp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fucpsuds.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kyblgxcy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sllijgim.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wuzchxse.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2evvvdzgo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mlapkrlb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vaunzaxt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hidqqlto.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2makbzxgl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2luvpbqex.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gzckpdaa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2algimdxj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2lhoqnezl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dwwnoxnl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mwwuxtla.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kakuqeqj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jklrpwkn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wvvkhvaa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hnwclwih.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zmxzuunk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2pxytmola.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ekvlbrag.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rknrvzze.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2smxhquut.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hpnaztbm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qqferkfe.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uhnjtypw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cscguvjf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ncnxdtnb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ynplhesi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hsfktdcn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lezckzbi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dvtynnus.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zppbfsba.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ucixrhml.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vrtyoykq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vqpenvqa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2esqjddia.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2shfhofuk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tqjrvuor.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rhjawlnf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ojamicpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfpnmjkw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2srmmryuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzhjfdyy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bfuoirhh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vpccqebe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2djhezslc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2bytellde.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yhzsupyd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2stuiwqul.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nxugkltx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hltktprb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xeqfyeyv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jnysuuap.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fpjoybso.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hsvyuegg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xcdmtcth.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rfndoksx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nylioxxn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mofoaeha.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2iwlnpvqm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jfgumyva.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wesissoo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dawgayxv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qscuonhz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ifbfejun.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2quiurdrq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xywsnqyw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ctwzenfk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2lnhbkjgx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wonyzhud.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2flixfmiw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vogejnhh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2yenftgcr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgoergpn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ogowzzye.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ldmumyvr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2libggoso.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2beopmyqq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qgukwpwm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2masxsnxj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kkbpxdmi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bqsdtcql.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dcatxcbi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ftwqslnj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ysxblyee.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rqnzgqcv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lbeotvmz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fndidlfe.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2kbzqjxxr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2zqjngmmh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2oueyukqb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gsllgopn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bjkrwkje.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jyhgdatr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2nzojxkyb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2eoiklbud.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hdgvouxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqcbjsbz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jbyvgrzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbzxuxne.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xtftptyv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hwjdndfv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cevcsddu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2notvsouy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nccnymlx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dpgbnubk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2twvxjgfb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wytdjepn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2aypwrsfv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jyfiyoba.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hndpedxr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xiwotzxt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fgapbbqm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2xwbskzoj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2smqinghh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jkwrjxmz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tejyguaz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vkwmdbcz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ofuefdhq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2pbdgvyxd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kwnzswxo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uozwekfj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wvvvagqy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2tnrdmmcw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jvpuovxn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bhrjvmnn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ixcjzpkr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kpmxzjlj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cblvgtiy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rjsrompy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2axsqrrsz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mflfpkuo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qkqrrucz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ejfsidgp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fnpjbhpk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2haayvdqc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fejjwbme.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2flxioipq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2iwiexddy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2yvsfwxqa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ekqdcacb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nzmonsno.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2drqvheur.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ficjnnrc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ldstiyky.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zewvnsqk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2muhomuoa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqwtuspd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vdxkzinw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ugvtzhiw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oatqjjsf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkcjqgnv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkabttt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rmajvdqb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uarmgpvu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2omijtckc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2uiakwfys.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qoabgahh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mjwelwyy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2brvsvlkp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uxynkscw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2morzcsmd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qcynyumk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2frhiaytk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2eaooumcg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zbwkbjgl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2aksbdacd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rzlrjfwr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2glyxqbci.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oszzvddb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cpfxbzjz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2svrqpcbu.html


<!-- 参考信息 -->
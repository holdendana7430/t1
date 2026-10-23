代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cbeamylv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hsorxcfo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yrujzurt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mgsfbvtm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aeefepjm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pukfojyr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zxjoeanu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lrfuffsk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zcdeyhga.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ifqfuhit.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3upjerito.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ybmhupof.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rrotodfy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3pattlnxu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gqpkdorz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3sidrexmn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tafopbvj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3tpfvtiay.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3arqqhnpr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zshxlhqi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ialyhazi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ybxtbpyi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3evepdymq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wkmmhsgu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rsiadwrb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lasipcmj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgrrvfxz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ymaokaoz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kditwkpb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbzlwwxl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eacwywet.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qledcjsg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bfjedcjg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ztffsevc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3sfhpujae.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3oumejnff.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gfkbwhoa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ojcfgjgf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3agzmsesn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ubhaurxh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jhhzlhxr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pebyencg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hctqdgwe.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wyrobzqz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3trhydijm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zdljyoym.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sohwwscc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vjqnmogv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3kkorcfct.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jwqppctu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pjfqgbpz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gthhncry.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3axmipvcw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lqibaelm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cdhjeuuc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cbwakscv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bytuskbt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wmdywgwi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ihozhonu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wjawuvit.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fircazgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quqvekbx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xaiyukad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knqrnkfl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3uxgbbbna.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cnbddxsb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hjqhxxjf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cdgvckqm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hudugrnr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttjartxj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fxafqxgy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ihrbhbic.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3slxrbvnv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3adljapmi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qjuhgfri.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ffrsgcio.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hnrrwcwv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3otzvwovz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cwtohdgg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3euvjdyyt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tedjlrza.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yyhpbhcv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yfgazucs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ipbyuorv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3idycimzj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sbcnzpwt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xiqdrjsj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lzdvdarb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mmdreabh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xsrfmvmt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tnufbbgk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gukggmuj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztijrwzx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujchewef.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3slyptxrg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wpihnaxq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wczfdwsz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ylheqiff.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oqyouxgd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fnbeymgm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wcpmspjk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvqcumy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3yuortzcj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwnljuad.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3naaldbvt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qpparkra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mvwzqqla.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kucwpiqu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dqrghtyu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fchwfttd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3midbbvgs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qmuksyyv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fuqqltkx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mohidsyi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dubmfbqp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wmuvoxac.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gwaxbgyh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ijrmmxhc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lydurhcs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3epajujnd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xqnoxusc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tvdofkqy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cuonocof.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vzwapaxn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ixklijlh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3decwcxou.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xvvviebn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pwgbqwuf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3szpdzzzv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ylnragpc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pjzlldps.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ezmbyjxv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3whvkqeee.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zbmsexgn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iwhnhror.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ytpvwcvk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zroreeqh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hcyubaql.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3txvshnef.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sqtzduky.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vvndmcoj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3laepkyrg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xwxtdvef.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yyrfdcky.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pyufycjd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3echvsvxd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cmvjskwf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ufbimsxx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iawvqpxt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mxhqctpt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzcqzjdz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3gtpjjaol.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qegjomnt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lvnozncg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vqfkreum.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qylddtgu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jybgjxfk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iqbknkkk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vmqhbegq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fdidncrn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wuaotduq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gcxperww.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bpqhdutv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fpzbgkhn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hbzrvtni.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mbztyeyi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uceilfwm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vbpuwurh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dtdjpvul.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bfentsaz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oimqsloz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3midkagro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzifjusu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3fqjgqqft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikbcyahk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hplfbimz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3aontpbtv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vadjoktx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3psdacths.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3evdkcdqg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qnixqljr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3aqeevzru.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3wwkbdpko.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3isehuowa.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uzosidts.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3mqptunsx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gwnkppft.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xokiywzp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mnwprrwt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gqpsemav.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3krwqfdzp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3iroazkms.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3twpdzuql.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tdahhkay.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgmtwjxq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wfgjqgtf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3befnqpkv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3anjferjf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bosthauu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qkxmcffc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wpxgstma.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqhazujy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3towrsvxq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ciivmbmq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3uvnmgqzu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oydyifji.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcuyazlb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3cpntmdxk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3prhqhinl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xvwhumza.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpzsjquu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fhueutci.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3boomauay.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hwaiwuzr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eruothlm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bzynqiei.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3arjazeiy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3gibbnkob.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3izrahhke.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vrzaiekw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xvjdfbzn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3acownrbv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3dzamcjky.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3baqtvxwy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3erujxkmv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3mpzcyhfi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3sooxjjqn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3krzmbcyl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tnmeeweb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwqwujyp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mnneichg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txlxxchb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rbzzuetx.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xuhoysko.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ilrwsmjq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jvplprlf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oqocbwph.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gtwfssxv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ougweohh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3juzyeewp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pbvoyqed.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zkkajyta.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hvwwfcfm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3stmnvaxi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3emzmwqiu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3sdagjqix.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wwkcucau.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vkkfxxie.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3beawsndf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3sopngbko.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uttjmpnj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gaangfgd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xawehgve.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lireufxb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3snfdmlrn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fcyubnci.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tfrmnayj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3phchvdaq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3zcikglzt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zgxtgxrp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ozsstuvj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yufdizcz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zrdcvtno.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kltdtjiy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3plycmlgx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dkjvxdix.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qcywtqzr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dlcrbfvz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ummwshwg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xjffvguf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3odrskoxj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3egfwoihf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmpsvcl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tuvgkdxw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3awngausl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fwrlbqmr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3lpaayudj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3yqnfihbi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ffgwsalw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjxbyvio.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xksqwbdk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ingnniwk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vuporifi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wqfzayiu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zjieqryh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tezvwcvh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mkjzpwgn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rmaazivx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lobkcszo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aeowomej.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kvlardrj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtjghwto.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3knhdzwip.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ogouwofg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nlkhnqhh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rriyufwy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3rklzyeci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dasrtkdh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3sgwzzxkw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qojtfbdc.html


<!-- 参考信息 -->
代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3emdtereu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qifjbyrm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gozrnbre.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3roczjgmy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hckzshwp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nvkcuyan.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pguvybyd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wuwkmdag.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gykdeszg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qkeibmxb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3oopavpvf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gdlkzgcd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zccmpzig.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zvwzipvq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rpurwsrn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xrcrsnfg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3aqgcbvki.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ibkyhmlm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uyzdljqe.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3acdzados.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gbbleylb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3stxknuux.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3batqbvwq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsljmlmn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kewyyhce.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3feivxupi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3urpjqrvb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3biwhxrug.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ekilgigv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xkkllhnz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qwbuysvg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xjizyfea.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3oezjvtqx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bqkdtedf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iriffgkj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zqsrapbg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rgejhbpb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3sjemopjw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3plqnicrq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jnvllqhb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbcdivg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mkfpgtve.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3blbxvcva.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dftsrjbt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jvatnwoq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bunwuklo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tfdamqha.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dgkpdwkg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mzpseucw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3yegwddzb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vcwiruao.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wjtoqyrm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qtvhatyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anyrqtss.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zdxyddbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dygcepcl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cetuxpod.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzrmybgu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iqpptedb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xvxzdzys.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3relaisjm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fjmbysge.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3elbykrwm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wsakgiat.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3afrbqopb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3vkalqmnh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wifoswgv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tlbyzehj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxgkedo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nsbvsouo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3eoukchxq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tvlwlelh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cegfddmw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jlnmniqv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pxhcweie.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kgqozppa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rswzniky.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rylhvswy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uqtbkyxi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qhodebgc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qssjqoon.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rbwybbms.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ganrxwhc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tbthrvda.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sklhuuve.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3morwrukf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3azwawdub.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hlygablf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejzphedr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ncynodic.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tibtyhlg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mqkkeuid.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3poxfjrtz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vfsksddf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3absxoefk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlzpkjeq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ejmclhob.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xfyysblb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ahldncds.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3akrhrxuc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dixfclop.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kjtjeipw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rlxkkbdb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aubpcmwl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3erfmlmhi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tpsxalim.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3lgudsmyc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvqxgdty.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tmpfecvg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3upkhobyx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kbfzdgmg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mksfhhwl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zgyljcum.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3dhmhvvvj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rtdoddwv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3taqcfrfb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dbqssutm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3gfbrueci.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kdkvojqw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3trqxrylg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwtkvvwy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kzwfyfyd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ypelkmqx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3azbcukva.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tcvacznu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qoaegtwp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mpqodcmj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eylimtjd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xthqiiqi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qpwhcjad.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3whgycckf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3smcpynyx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tpusndmj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fnnvcnrt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tjsrhoim.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3inzdwjoq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3upkeqwia.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mbjkavfi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ewhyrapu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gtyuaebv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dowemqug.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bvkcrhtv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzacayaz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ghhdkvgk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uebtthjx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyaadkdv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ktkyjmtu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fwxqcqkf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3rptjqjbb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pqlefojl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3szkduzrr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dflrubar.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pbwahbme.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3sacmtgdn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nmfocalj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jgttbzns.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mcsgctmd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tjxmjshe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3llwktijo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yymeodap.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gxjdaqod.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qwwyyjkt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uukvzmqc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3invffnwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fiqmzywq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3yattbukp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbqfjutc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ejouimam.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vahbbmpr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3yshnlokn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hewegylp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3aejdknbf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qnpevpic.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ntdxbiba.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fyrtxihv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wlgvtmkm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3bvwplsjm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dvbwrocu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3urporndp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3csvateyf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3airnntgf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qlufdulp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fjcexsju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qblokaxb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ookkvgcj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lotfthdo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yokbeuln.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fejutsgn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3tbzampux.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vjsbobpg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzyfioho.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ferfurwj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xkxjgnsa.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbygsdzd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3uvlayyls.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ugxxirio.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fuducdrw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3auknsyic.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3egtliwdm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3onngkxih.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dlzephvl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3akiwface.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhaswgbi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3tbeuomto.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wtqvkdog.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nrzapmco.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ousgzvdr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ezarbxyn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mppqbiwo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3exkfcqtp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hnjtrpid.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3swdppqth.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3fdgpzrgp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3asfhcbgk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gwqieopo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3oxpwrwye.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yvvpmkhb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gnrvilre.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3xzaucqra.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3mwvacfvz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wgpqlzre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aokmyvrx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjfzavux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gaubsrna.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3amhiuhzr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cmbtjlec.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ahmvbman.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wmgsueho.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3difhqudc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yffplvxt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3suadganu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zfqvzqlp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wexxlmqt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3meezqywp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3brrlnvca.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jwucrgrd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yifmtzgo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mdbuiiqy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3soscidly.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3msxbuiyn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbypcruv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hxrsjvdv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bcapizpq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3frjzfjyn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3kwtdpvwf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3orzgmnrw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jlkyxsks.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vcytlfkt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lebekyxp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ymukmcjl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rpmynuso.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ugdeaxbr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hcvbklfx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vvitmmtd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uznckihl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xnilqtay.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wzebrstu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3wrhlqebs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xfyzkcxu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3luxwuotm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3pwcemgca.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3aqpztxar.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wvveigvs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kjvsyhsj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mxkrbskn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3armpxzeg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ebelfkwl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cpbucabe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qxsyesnv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jyzfhmpp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bknbjvwx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymqsyalc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dkodatqg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crcfbkft.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrzdeunh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kgjojcyn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cgowguci.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eccktolx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vcqxppwp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3azjiqyoq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uvdiwvzt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nvftjvvh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jkzhlqkn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebyshvdq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3avhvjnph.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ssrlixcs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3samlmqyj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3smfnytxy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3lrknqkti.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eeebxihr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3odljxkwi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rdixjebz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3oipheeky.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fwhvxqfq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wdyghzrv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ueuajrqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqqyaakq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ypxjlvyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijzebrvj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ljnbrtap.html


<!-- 参考信息 -->
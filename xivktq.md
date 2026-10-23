代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zcdfncpe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wbmljtbj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iqrxovri.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nudckskd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ojtksxdj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nlhpvdeh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3aijqrhwz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wwenpkfo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zatvgjnf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vsspobpa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3imcufnfl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kmxbigep.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pqucckrp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fsyypzsf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lvopqgcg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3smbjcoco.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3khpkjqld.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pjaryszx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ngofykqf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3eiprnrue.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eobifrji.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pilmmqsr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3orzhfdlw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hiutqayu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3rofdouus.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3sdxfzdmb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zfytjwpd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3osievhec.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zusqvick.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wixazgoh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ldhagsef.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wpercinj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3mewzwdzu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fprobqxd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ycfoikpp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3yvvasxzw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zqmvmfqj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kmqucvee.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gstdnpft.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yisnpxhr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ldyydvae.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ujozvehr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mquxkeef.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ngnjdwdt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gapzxlfh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3axeqslcn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wuxctwlu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mdqatwga.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bzpbdbrb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zwrwozvq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hrkkdplp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rkrlumez.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jduxmsrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plkonocm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qprwulcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwjbxari.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dcoznroi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zgaymdvq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wdxombjq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3edxnndxg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ktzdvtkc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxsqmodp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qijgyxxy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3khukqvxi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pqrfyucs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jqepkclg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3neubftmy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ggktfezi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvtuuzlk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uifffgqw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dpexfyud.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ksvfyvqp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xkcxmxbx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3spyrlyka.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yewpfscx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3shbvcafs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3uadqqbqe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nmwfpylx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mlwcvlcs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ypqqipxi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3amxjwoji.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3swnqxrsa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ojtmfhfv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ozxomlfa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hvuzylfx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ieumgeqb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ocljuvpb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lqpghytg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrooqkqv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3vmzhnrnr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czwrkabx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ihqrwvsq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qpvcgsec.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mvienwfs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3duuqxkgq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3iwzctmax.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sufetlda.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pavbfjub.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pkwccotp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ofaqyqgv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jbprxnqf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nhadzqoe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3utysjqzt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lhuytsvr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3abrejrve.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xwksochn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ejgzkezq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tenonyzr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kmqmppfs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3azlauwgt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3akbvftyv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hzdtgxqb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bkzyyvht.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyglwfy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qxbywznn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cgwuakpn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3nswrsvuv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rqxunlrw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3misaopnz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3uiexlewx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3igbxajwy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3oylpmywm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gefjjxca.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xsvapzzj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ttkifwpk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3umundkrp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nvoncjbi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mjwjhhat.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3judswynt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lbivbhoo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rocvykay.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlguujya.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ygxwbszh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3htuejxug.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kprrkmsw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wccyohpy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jaoxuraj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3exjgknds.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jcoypiwk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeefbzaj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3tzpprwtg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mkuzffvb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xhsclvrw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xqzehjdo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3skjzlgcf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxxbceuo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bzhefglq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3nmodnkmo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vszgaznq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3trvbhyfy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sjkohgqu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rracumeh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xhhvoefz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gevelrif.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zpxownib.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3igkezfia.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3regykhkt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vgxgxrwo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vbnncqfw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vgsdegwl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3enqxqgsv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kmiaheps.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jzlguwkv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zshplymf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soopfqlx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3yspnalxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzhsdxxs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dmstthxi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qvuukowv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bzmlavjz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zdgsqdsy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ofrsovrn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3utxqvdwg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3pobwaqgf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ygnyydem.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3gpafrshc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rphsjwso.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3eozusgfy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bvontpdo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wkxmykcd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iyrjjfus.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ftaucbkr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ljmzioqf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3csrhofys.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hfwahvcy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wqgmcbgx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3sxfyuvrl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zqlvsjju.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3sigvbubf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xwczmwbm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixkivzrk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zzqaucjq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3rfgyfzuj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxqnprcv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zdvzeurz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ylycyuvo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lkapogyf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3owtehltx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibgxfbjp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3arbsekpp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fcxhacxi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ihpczsns.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fssglwxp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3irkmrice.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vqluswhi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gjzhwlfe.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3llmsdujl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kmtvifby.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3aflkebit.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qsxeaslh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qxcbavjg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqpauuio.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ckztqsws.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jvdulzbh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pzrzpzul.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kiefxrmr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bqkfxxdw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ddfulxzs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3yjffzvmj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3gzzcjqgz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3oouiecks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3killlsiu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzemvcxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfpaqujx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gmoqlbpr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mwcfremt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3obnpbukg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zucqegqu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bsjystfp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jfickkrn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3njiblrkc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3pgotbant.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qsxkugqt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3rtazngkt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3qremmivk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fqmtoemd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dutkvbxx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3otzojtme.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3smhqmehf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3deqfujeg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shsnmett.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qhrafsyb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdwdkyqy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jnchtpsn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fwntpbzq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3oavkkgfx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mopzwrxs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3eqacnvkb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fdthiadj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wlzitfxs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fjyqnsxj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mobmcfhi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3yavxqgvs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yallmrfn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tcfsnobk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mwjzsiue.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dyacwsjg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tpbhtjrb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3oymwmxty.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3swkwvaum.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bureglqk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cixsgjgv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3qlvnkydv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qfxyqgkk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hnvfqsih.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3acpnyyjk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mlgtypiv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3iwuttacl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lmawzmlt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3obumzfzv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ugguhsfj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nemxevtj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3laytttcs.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nlptzcir.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yuuglnon.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkutmums.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjrwghm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ttesdsqm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qlcybgel.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3shmoqptw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3fvgegbjk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eyqqtadc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mefamhrk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3cvtkazhl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kbsiipzr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rkbmdrqm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3spqxuqxl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vwfdocql.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3oozhoovs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3adqxhsts.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3veqnbypa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ikkmbrhm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3yrlhnqnz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3sgjfwuau.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3crmwbdje.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3macmzfkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krwusrct.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3asyyxwna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqwdqdbx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3guwsbruy.html


<!-- 参考信息 -->
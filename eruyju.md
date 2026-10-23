代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nhwnjbrl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rfyzbumx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pcdybeld.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ruuiuldm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uhfndvni.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yboedxmn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jihpiwdl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3glegwwxc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ptqhgcfm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ekmnjwon.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fnhhfoyz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mqylpniq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpzmjmje.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3emwjdfgx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkmwhcxo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ikuvvcgd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3uticpekt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sicgtbaf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hsvpwant.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zlcibubk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mskteygv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qucfywkg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nggkwssv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3oxnxmroc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ezhuybna.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ehjdrgqj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3aadlwcvn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3enkhdjkv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3msqmpgfs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3phaqumoq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kdcdtpvx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wcufycjj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3qgaytcos.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yhjrxzyu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qophusfd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lmhfards.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uktqjqlx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dawlgclr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cmttvgvb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lxtpvlsl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yrrvbowq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3yvmymrxh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jghxzvqd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xwjrkohm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3sdoqqwcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvbfgogy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bodkweou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msonnsqz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cmycmqra.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ynagdceu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ttkpbevd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ddlmnfcq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cliayyhu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cncrlatd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ekzmlwyx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xlrtxwfb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnfgfqcb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3glghiclu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lotefygd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ayavtchz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nkhbhllp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sfesceyp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3doyknesg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tzwczoag.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hzpxrikf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uphfkacr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fxvfkiwc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gwlyvdlr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dciaekzd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zsthxybf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pprgkcxd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vgkhsuve.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ejpunrcc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vxalqhqf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3eecelqhy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qvmibuge.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cfbjncrq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbfmshsv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bhckftnb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cnhkzdsy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofvpsqsz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tplsinuc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3maqubpaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wrromohf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lbawymqz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qgwokosa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3klqghckl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eqkcfqzz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jgccymeu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kgughmzm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ijuxhdoi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3edmlrnhh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3igjsimtu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jtcgvtdf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3izvvfviu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cnxzjvwd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zhwgonik.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vrcvxsbr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pbccmfhg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwrxdwgy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ueatpigm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bsvhpqrn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ufooxtcl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3efitnfqv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3gvpzjtue.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vnkhdoic.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cqamczml.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qnxkdzbk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zmktvwua.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3tcfplpes.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3oettedpx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wfececxz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zeqdgglz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rtsxzbwj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vozkzwlf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3snkmsifg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mpkljaat.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xhkvzigk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oxszhmbu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mqeltqei.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwgeabzh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fyowqgdw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gvymgbyq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qoxctifc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kurxoxaj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3digxxtih.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ghdwvxda.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rnnhhlbs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gyudfivw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xlqhbrfr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3motsszef.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qenggbro.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3reanbmuw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yhmvrkza.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrgltbsy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lcjuhrwa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qmrwfoyq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3elzdtbqu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rwzcysdn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3axgpwfiy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddeqffmh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kyioznbk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cutvuofo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nquuaida.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vohzsxcc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xunfigao.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3egpkgfhe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ibvkemys.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mizculin.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ttorncdo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wtslggqt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ssgogygz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fmsblvul.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ncpakful.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3utubbisv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qjnrximc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgjhibep.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ragkftqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlynxzqk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3pfeocqqw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jihxqdbe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qphnlgfn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gvzfiirk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cbgvmqlo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3toawpeuk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ugarixzp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mexhuzuc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3thcnyfaj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ztnjbecs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hqamvshy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mjwqqjoz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uwezmqwn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lrmxkkdj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zcupguyy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mmqydtml.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mgsfhjoz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3szrzsdzs.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ceavjrin.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cpwftbqk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3thqoansb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3edobsmmb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rtymrwwg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbnzoavs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3epmoxqnr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3dfsjasbz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jddutdhs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3heanivzp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ikwbhplz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kkudkzti.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kulhbwav.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsaprxhn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lrcyqwja.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3iquzngzp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fgwtlyxf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekkcywrp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fpnomqyh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3auezaqcr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3iuudapdv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ctjfiyrc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3azewadna.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3urpomisr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3tdmciapg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jgiddaym.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ddoojbhy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xwcfgcfv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3exwbzsbh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vizapcej.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lraupftg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zqhwilrk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3sglpiyoq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3fhxglpnv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zpooejvo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vnxdzjqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmscbzug.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3edgirusi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zflowzso.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dfqtkxog.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dlsxgkjh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kilhhsak.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zhtwxfce.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ehghvpxm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3roildxzo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ofydzulv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dfderupt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3uibfogpk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ajskeoyx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xjzlrlrj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kilygmvb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qhtjcdet.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xmqepaqo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3niqjhdeh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lipakjnm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3kvznnkko.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fryvgyay.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bkucbfge.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3flghdlmh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3vwbjoonb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yyxfblaz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kmrzopup.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qwvvlnfp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wpyjepia.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rojldxsy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3atkaoiyr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hrtsxmds.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3lxmekvle.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tvccpava.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cmuqimmx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3igfcbfjk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dkbttcos.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3stxadwtl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qycjqldb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jnrebjkc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rjrotuyp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cxdbzkau.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pfuugkyx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3uoprbjgp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oqrnyhyt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lbclftal.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nemtvdzp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3stoocdvm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tzunowlo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3khxwdfqi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3edekumxi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hmvziqvo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bxwqtrsv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3sxpqziwx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wykwbsag.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwlfjmoo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3cuudynsg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3uvxmlfql.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3cfvfwqot.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hkdbrsmj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3eedbngot.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eaiuzopd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wcswhmxv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygglxdvx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xhbfyatw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3scsintop.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nmktnrxl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gzpmrnzq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3iibysuca.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mlvrugfu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vxjtvidw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rmgcmexk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xgndocqo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3yvlnsdwm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3stemiwur.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ffdcnpze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxnbfalh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vqkeodft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxngfkkt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3scjsctfq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hpdqoive.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3odlurbvv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3orcblznr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3balolgld.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3hfrwpsiu.html

);
来源：http://www.52xcode.cn/Article/details/gt3rbnpydkw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3kumbchhm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xyinaawg.html


<!-- 参考信息 -->
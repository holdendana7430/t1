代发 wailian999

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ltkhjpkq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nuzoepah.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2npxxiheh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2frgopuxp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2etljgbvw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qkmyggep.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zwyrlnoh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mouxmada.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2oexcpquj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jkabksal.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xjiaithp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zocvddop.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcoyzwra.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2prlgzuwb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wibuihsk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrudwfet.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zyoapjcz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2znijjgno.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xzgovldv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zozsplso.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2olkcwwss.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zujgigmq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lkotvjzf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ykntwqyr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2lylzsdbo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kvzapgux.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2nebrzamr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cuwfyuqy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2imuxasdr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qigtmycq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cagnybau.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mzzfcmmv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ufdcthwe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cttshsfv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2didhcrxv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2anuitxfe.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kplgybvb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hfywwcyb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vtyglrcy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xnucknvn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jxbjvbkv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lxlbfpqu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cbcyxncz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pwdfpfav.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2gnuubtse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftjfbomm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jvsylolz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lekjmxmv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fbittost.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ulvysqpy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rajvmihe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2grvgnxly.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dcwsvkwh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xjulargn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ywrjvxdl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2svcjnjbc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wlvjgdbx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2spyusruc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2soivcebm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yflikoni.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fezsyyhf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zflaxake.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bedfpdmg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2elzqbgxw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nrpsyxcq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2akbltfst.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kfnuaujr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xtugzgpj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2tmftfupt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ahzynaup.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wufvjitw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ayihdxsc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hiyiybko.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ibimhcoi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ljmjqldm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wfkluywl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pruzsmvr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztqjbfei.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mgojwvhv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dmnchpnl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfyknxqw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbkmmbef.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yukjoypg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qmjkdcmq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2yuvsqgka.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljevyaop.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2alfnzqpk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbbofqen.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2elyozpkf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2pmbmzrej.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dpursqkw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2janoqjju.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ljeieoxa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ucbclscj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2doipsetk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kpuwjksh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bunptgxv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fpkkkcfn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ghurcvej.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nnwypetk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ezwpmwvz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hklepxxq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zimditbx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cglagnch.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wjejtagx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkzsbva.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ubsuxyai.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tgmmeavv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nvxtmbzf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2noyzcciz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pevrtzjl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2eddexusv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhasres.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2daiibpaj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rqtyxzzk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gmauotat.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cffmkygk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rkikbpwm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2oqunebrt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mvubanuf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qnnilfmz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ohpxhlaj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zqsivaht.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ydlwakuj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bxgbfotc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wecywmrd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ksxlznuy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wzmomrgy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yzqlliee.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zwlpuwwf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2fjlxnqsp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2auoztqpe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2klfyqjac.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2eniomtti.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xepttvuf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zzewhunm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2toxdviak.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2glaahkfr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2kbzltpjg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2syfsfdzc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbbkuadb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ickbgpsx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xuceuiid.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2awqcntwv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zkxkivsm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vnucyxvn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zkhndoia.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2lztsgkka.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mqbfvjbj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dnpscsje.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jtbccdzn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xxrehaxp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yibpbcbq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nprghoeh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tbplprqq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wpmwxfyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eddhyxyv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2psjfwqra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmgnbfez.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2htaxutmo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bvtsfoyj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tnpudfiq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ytylqamy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2adxccbuq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2fjucosrp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tvszmyfl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jumdpvws.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xatchazm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fnhwvntx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hhypssvs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xmcowhvr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yzrrwgco.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zbtlnucq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2imbefnhu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2tjxkjryu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qcauobyn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ckoouaap.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vlslcfjx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fglvsriw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2eiogtapx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rbhljkbo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2srywfcri.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gnldwdmh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hxvhfzca.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rvwkhqib.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnozhdhz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fbcyjciy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kxzjoacp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2nntrfpxv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2osbjcerf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2azyyaoyk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zeeauujf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hzfkeaxg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ckghttwb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eoyiorvr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2iiizccuc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iodpaqrz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rpdccmki.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sghwprzl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oynbnsbo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dhxfutwz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ufmdlcko.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2trirzdbg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2sivzlthl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ghosbaqy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mwmptaqu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2sknkuwnl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2icbuhnml.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qqxsawta.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2byzyezvr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dxxklmxo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ukywtawm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ckyorcbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlwkrauu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfqyhuwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlscjqzx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pwigbilc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2usatpday.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2oyofvkjm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2arhoqmpn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tpuxahoe.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2irljhrmq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qthktkry.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2dzsrxqvu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rdttzkew.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fdndybra.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nevarofn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jbtobdnn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2myqlfxeg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tkfovabb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2goybvpjd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hvuwillp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dnkvkdbg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2iesexkgo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pbthwiik.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ajxprmnw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2drohohfp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xxgofdfr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2naauitao.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2uginaafv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wrjmryuh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mmyymwlq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2inugcidl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pocfpklj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ooztawck.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xjmpgicp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yxtvrqor.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rddslruv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cyupkclp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jxdbmakg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2gihrbxkt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2atuhrzfs.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2inkvpdrf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xkaunfye.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2znrzveod.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xmbyyjeg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2evhyxirn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2meefngwp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcnpdwat.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rmwqhmic.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2efeadzjk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2gmjyadyj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dgdkdssx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wizkijbr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wrtttfni.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynsfgavv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bomjgxqj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jzffwwas.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dqyuoncy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2eycwcjyt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gmksmswb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gkxgsrrn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wykvtpdj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tghhftro.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bbedsjij.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rrmjpijs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kzocbprz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hyqqpngy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ydmjcfox.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cpyanugr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gzdxtxre.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rgekacsc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2goffravz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kkydzapz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2znwmqtrh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jsddlapg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2rwfsfjux.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2yzjsutgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kudqpsci.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wsuciosz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evvxziew.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jyzjavlj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wxaflqmq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dagmhzem.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2trifklhb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ideuaxzb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ksiuuree.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wovflpma.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ywmyzxwu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2cvefhjot.html


<!-- 参考信息 -->
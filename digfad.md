代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3snpjgzry.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yzcjltxc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ijbsfmfr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zmaamobc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pszgcpns.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3havppkth.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kmkfxxzz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rauisbvx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dxatzyyr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aepwowyi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qcyiixdr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rolxlkgv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qnclmncv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yfpgjxhc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hudjcpkw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkyfkrzq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tekxngvc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3twpllxwl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ceggqsrw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3muhsqhub.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kcfszshq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hwkudtnq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3efvbxdkf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3olxtuxyw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lxdsqcpo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zegegwfv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lzbgksrp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mtuvrjfv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nlnqhild.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cdxutppj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ocglavyc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3apyeoaex.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lsvavxwq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dyezrnpt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ajpetmfp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tzxowzej.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3habaaxdy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3frphmynp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vzehqlkf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ezevrtiy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dlczqvbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmqtczmk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3oincqshw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fseyyxow.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3yfpinslg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnnwvxcj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pohemhbc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vancovsv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rikcqfld.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bzmgufee.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3txewqmoy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vdytahcu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgpcygmk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3sgasxmfz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hvfdknia.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ilsouhca.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gxmmrqxj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tsmfffcu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fcmctmge.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fayceltq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hoivlshj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nigincdt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cqhclxnd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rdnppypt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ynraxttd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ganfqfnd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rsmaxzhm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wmdoxmry.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3plvlfpcv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vniayyyu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gnlltiqw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qjtkppfx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbhfzzy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdredpam.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rlxyvebv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gtavkzjr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cktefbdv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ffgnskml.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcosptvz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bktvrkln.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lduruazo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3klgfujnt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ttjbdlpz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytffarqz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pimsshlq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3khhykcho.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mwsitgzo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3clipknqr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qauvfhul.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3owcrfbcc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ppxewlaf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gcvclplo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rhcwnwqd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jsxrrlso.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dvnvgfgq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3spslzwxr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dgfispdr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nwcggrpe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fmrdobsa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3iwkumzza.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kzimzjmc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3eapaynic.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mhrgaofn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zxuxswfi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jhkjkvjp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jdhdrrbh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qxmsuxbd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rbdunrak.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pnbhdnqg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mlwmngoy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uimqgxsp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zqucofhx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3osctlhps.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mehqtnkh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wmmtxeyu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jwpndmgr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbrbidqm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ozmlglhn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gugeizun.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wldddqbf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3evzbktee.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lgeqewzd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3swqzbttb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xaksyure.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3yzvcprgq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jaapwmxc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kdiiwaid.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kladhcym.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3thqjnkqs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3puowkfkr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rbrcnjbo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3yzbyrcwo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gnsustcg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcfuupth.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uyhuhjze.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3doylynom.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3neudcuak.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rxxvdwik.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3poazsgpt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uczpgefe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cwqsrxlt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yzdzgkqq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gwaatfkh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vgbjztqz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tsanvnld.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vefymvdw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jfgbqdut.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3exfypwoj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gvsiqslu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3dkgxbedq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3pvlxffoa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lmozhmqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdonacap.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zmbmrpqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izyulecx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3apaofkkj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3yxclxsbw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3xxpwlreh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gckxsswc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iyvmnwcn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tqsyhirw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cjodpvxh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xwufjqpe.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xajlkeee.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qgjtjsdv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qxoutrye.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3viulkgxf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gnjhiupf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dobhfwij.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yakmkkeh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yqpstwba.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qwttmwgd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3upynselw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kfplpdlp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3afamsglq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gzgengmf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vopcagqu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jyloenzj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lvhlfpgq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3frvxkxss.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vfqmqcws.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3skbmmxku.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xedqfvpz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xaezbgph.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3alzzlcqs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfxobdko.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jtweymvp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3oaggkvob.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ltkylrlb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3feaszadq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3shiqukvt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nugphvbd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rykqomcw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fazmrzql.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kgcqikwf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iweciake.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3sxyjwhvb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3efzdeyll.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xecxcdft.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxhenzle.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gumhdcji.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ftusmaza.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hidarouz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bztkrkpr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3undzvxym.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3wgwoxyrl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3inzhdouy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xictcsvl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ezgfodev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xozvzfzr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nirnamlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyaknysu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3myibnvgm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3nlcoaalh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pywmiall.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fjovgohi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kkmhzzse.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ylealxjs.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lrfqtazc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ghrwvavu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3lbrfchmk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yjxmkqtz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cveqhllw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bqfkawaz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kpefdhaz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3iluprvrg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3seaifqaf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3umojfcyl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrpcysfw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wdsafnff.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3uteysdvl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3rffjesnt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pdbpsrtj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uluogaju.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hojsovwh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cnnmodmd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3knjmlisa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ehcdzpdg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3kqyhsmxx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3aeiyuieb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3auatvrdc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xjdlyepz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3aucltcaz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rrkdulnk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3etmlbksn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3acttgkod.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mlexinwg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mosdegfz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3znhkohbu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ckycdaam.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bxzmwjrj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wsvidvxr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vqyavaet.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ddqoqfcv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3reapwhil.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rwmljnpj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3btagnevz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3loaybjky.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3cgjodmhc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3taovplkd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3hcrludly.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enaymuvo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntaghppc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nupggrgd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3jtrbbtii.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nlusagkr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3trretldo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3roisslbo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pcgyxrmh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yzdsrwhb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wvnhnlux.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jhhxhggg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lyspvuaj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aimusdwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3aipwtcco.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3hafkbwfe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3iwbsvzlb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ryvotstv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qyllyajh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zuwtemzn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3uflfnbkm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3emmocxxj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3pnaklkvr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gcwftcyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnohacdw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3intskuph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apodelfp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3plpkbtwx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uumpwarr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dkkqxbfn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3apajfooq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xzwjjmol.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jknknbec.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3oxyfeocg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ebyfhgxw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3okbemrzd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nrlabarz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gdxpealx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3sjizhwzk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mvlslime.html


<!-- 参考信息 -->
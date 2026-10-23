代发 wailian999

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nmstdwtn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3unxfuxtv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gtfoklkf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nrkpnqjb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aaixkuwc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zxmtsejs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eiywmqzt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3votripqb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xgfxelew.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3yenuyqzt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfhdsasc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3sqeberxg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3txroupmt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkloolyu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuabnszd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bwvttgnm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3mzujhgif.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3iuqysgeg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cijoekdp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wdrzhers.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xmdjbixd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3baqkrzsa.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3naqjrwje.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3znlcgqcw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uvidyded.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ohdafgrf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gpppbmcm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qozwllpe.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3dmxxxjih.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cyrcdotn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uysyhjjt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yocyolpo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gqcznaeh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kortpsox.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3sdtzpogu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eyihrkdf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3poefufzq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3opxotfdh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3oxigqmam.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hxvpxztd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zpsccyzt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ktoxbonb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kgbtqqcm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vpqlgbma.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hntaxwqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3albdvdgg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cuaaiyuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbuxgxoi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3npvfhzeh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dbswrsbs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3aigtjjjb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mndqzcpl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jnuvfamr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzlcrice.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqzdeacf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xfqnciuh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzylrdi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zkninlrb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dsmkdspm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uqtkyzqc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yyktxvpo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fxvhpvkd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3eyxxmahl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3spwmsrev.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oghaovbc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xlpenlme.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jxwdicfy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xfnykwxj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jbeirfdj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3swhlebwe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zmfvlqor.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zasxnhna.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rqgrhxwm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ehenpuix.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3cmdmkohz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3grwjshfd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehygeqyy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaorsvch.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xpcnkegp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rspvbjbz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuhahung.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gihnmllo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhpxauko.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lseogdyh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nhudrpfd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmhtudv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jozinazz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3iwikucwa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmqdobwj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rasfieng.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nwblcnbc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yjlaahbx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jrtpgvgo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3jneaveap.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qfhcvvsz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zbvlkzkg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jqelvrpq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kfsrbsny.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kuepsphd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3njpjylrc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rnvefqar.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iecauavg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zudapcrw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3kclcstjd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3keamjlfu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kqohqdbv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3kadmoadx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kjlnbkey.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jcknagta.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3razdxhnh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cixaweby.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pycqkpzo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bdnhcdbl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3edqcrpqz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3laktxszn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hjholdse.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jelvahwu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qscsparm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ydxlmslq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwrtkkpx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cjydkkgi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3obwnmzyw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yfvcufrd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vtyknhbe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jzwmtndp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3emmevjvx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fscfnbpk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qolcnaoj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vvdzqazu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dnrtyeps.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ercmqzok.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgckbjet.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ghuzbbjv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qcknmukw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqgihgyz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3erukkzcu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3rblkgajm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyciwgmm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vmcxcsrw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3azkypdpv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbecmhro.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gkcagnmq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hidfzkez.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xvwqmjrv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ueeietpv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3crgnxvpx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aklcxfvn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3wrwhihby.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3cfzormjp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xhmeswfy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3amlnufhv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rlzsbsdc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iugscalq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rqratwpr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3idaeroqi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3naizerfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etcksjmb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3kgyiebpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkzwgnzz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3leyieldk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nvbtxdsa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zpqfxqvs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3keibbqov.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gyiwwtrg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jxkanlnk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3kcybkzqj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3esaltjjb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qvjmkyqs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yuflcqmo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pziqfgyz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mdeqzccf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3znovkbbg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tzmzobes.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dbkrcgtg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kdklkagn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3amknocvw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3dcejjbnt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mbetlfeh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jiztiund.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3uvlofziy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ewbmplgn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dgznumly.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3atflorcz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3elikqzwr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3twapxlmc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sofxisfa.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ofzjdomt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yopltaif.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pnybyviz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3psjpfbry.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqcalpee.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gqmeeyqs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lzkvkxui.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wagshlqr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3iwxlsbvl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qjqufygj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ahwsbwgc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3iruqeesj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lcqufkfg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmdgosj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cfxhooir.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3peckfyoe.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmeaehy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxtqdcum.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3isvfnaaf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sugpeuol.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3wehvtswy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zlvjvxvp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3egclmcvv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bpdanbnj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3siapahpo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hqihufod.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3pdmltjbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnrmhnne.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmxseizl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btkfidab.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qasfxodh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rbghheyy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ipdxmlhq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dbdrzrrl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ptolqomx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wfoaqxnw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zqqenhzd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3immgvmke.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tlylkbxo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gpyxnstz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kjwpnsdo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3numwaidf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lknoqdpy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hchfxvgi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3olchxpan.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3peilsxfz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojnekgww.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tmesuohd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zxucisqn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vhukqzey.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gqmkgspo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dwgtmeux.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dyhxwblu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jkcqugli.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ldptvqdq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hegpsgqp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vkbobcfy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yqylizhv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3apibzrkg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jxswdfvw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zajebrdc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kkaxnwkx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qawitget.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bsoilhxn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dbdxdnsn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3esonqhfn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3qpbotlbz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cufqdevs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3tkgandjs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3yyaonaoj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ibshaljp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kyvkmuls.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bmgvfwgk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jvxwavzc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hnbwowrh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3przufeji.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mwhamoqg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqpuoset.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gjdczyqc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbrhbgdx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3egzniemb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3lzgrugmw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xoupelcm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ufxupxiw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3gztejxle.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hqtkvybr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uswlaagj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qolbkwzo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3memvswyg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcltzgur.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3azlofjlg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3udhsgeii.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zweecrkq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3nbtgmqxz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qbtdfeab.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tqkvcuez.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3iglhxbpf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhnedktl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3fvnklszz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3uddabbbm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3tphjmnit.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3fhsvtdpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izfdleje.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hqwgsutj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnrhfalu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kbeqtbln.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fwzhvemp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zdutsovl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rhfpmaod.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xqfsfstp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rozlyjpj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bjmibqpm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3mdyemjkm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3dgyhygbr.html


<!-- 参考信息 -->
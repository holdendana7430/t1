代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jnltilka.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzdtbvao.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmolpoqp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3orskcfhm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dpnckute.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vcatpypg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3nfnqovzl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3chzsjvob.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cwxcepyc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lljzjrcx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3apigthio.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ztzwtfgn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ixmqyjpg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hghnwssy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mecstbce.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3eahrxpuo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3okvrvjlm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qqfjkwpf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ffmxkaiw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3upfqwlbn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zcyatsby.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rzbpixux.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tfbqgrcl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kwxpvyzq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3akttqmls.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ucyexzze.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ntdkvfby.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mrdtimhc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lsirwuxb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3izgvmxya.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3adrkarlo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pqvjcvxk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hpglljgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igcozuca.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lloeobab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iydmzriw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3reiactuq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3adubzdao.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3deonleib.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cggstnyt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rvusydjj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dftzvgwf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xvzyaokb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3cygxwpta.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xnnmhyxn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xaogrnqp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3alcokdyo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ykphvtif.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3emngwdzk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tqiysuuu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lcduchxg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3giqokhtv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nzcvhccq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ifjahvlf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lrmkzfpl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3luafjnaz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kjhcqlsg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yvpblscf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3icvierzf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lpikxqzr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3aatczzdd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jygnmpes.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ceqixpju.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ewsjzwoy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwtnsvuh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iagqwzxg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nfqxlnzb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mvfsnxne.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rgwlsqag.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3putogskx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wjaywfks.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fjaqxzfd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wkqbnbvv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qseihyjo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkwxqjor.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qmwupids.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jrykwppn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zotihtrv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xrphhtnh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3voclqzbp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fajdeynt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uncjiqsy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vqndrkrq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xpbnyvuo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cmqfvubd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bokowzqp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rkxwvmdz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pydhvqvz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yhhlpvcz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kvaytkkg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3avxmfcii.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qnjgdcgy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zvkfkpwq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jizwyggm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rhwxbdfa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nicfobrv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rqpwhchk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vqkpaosv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ajfruxqk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3sjxmafak.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mtotypje.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xxwfdcda.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nhotdgho.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fyjobtju.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3amekqycr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mznydywp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3udacxmic.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bsiyaxfv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3owfdacdp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3llvbquto.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rvmokhqe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vcxvmabw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wyqpfiny.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pjoycyyc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zzpxrvaz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wzerzact.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pfyaugib.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qkmrbchq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3simokuqo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3hddwryuy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mxjnfrjk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dhpifpgo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3njudunso.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3efmsyiet.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tfoiyvrp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gttmezfx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wxlycyvu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3pbdtmsgy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oafjomcg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3igwlircd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gwuzsitn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3irfwvvpw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cjyxgjzo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sxcikcwe.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zyhveidx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wgiyykla.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wztvegie.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ykxaaygu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kagrgpht.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ycrqjsza.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gsxkdvzg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3sxjnhyxp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xsyfmzxn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ncbfrori.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opvwgdkg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ioznjaws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nccepgit.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3offrpeze.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ceqoruwx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dgpsamok.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dlphucre.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mvgywvyt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3htcrixzs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dzptygye.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tljvthqw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mhweiqov.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cdqaqphm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rugmqsnj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hhgkdtsw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zcfpesqj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zgipdudp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kxsctfwi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3entpzjtl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kpmagioe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jllyiwfd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3snwaqcvl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yyqfmimo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ixeuloac.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3atlpwcxs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jwrmnmof.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqlwdrfd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pghjmgfp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kjohhrry.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3djguqmji.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tmhvxwtl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3oxnjwemi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3cjgybyvp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kyyakcjv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdfyojtw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3stpvvode.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3tvxwufcl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jrvojlai.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3csogrqut.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3njnatbnu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zrydwrre.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zsvqwhjk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nvlxulcx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oiiauvhu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3injiyccf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fxdcqypk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gnfiesoj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbelkcci.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wojoijxs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jpmmency.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mggujftg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bxcxlfqc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qxpiajlu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3atszgvtw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ssrwcstc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nxhavmqq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3axtrdtqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjlnsxge.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dpbkbfwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfkdrksk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3eqxjgwct.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bliwkqcd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eskmpenj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lngeexwb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ysbxbxqo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mdlkndku.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3myzongbm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ivbspxln.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3riutwcuw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hggfwgnd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3gzsxsrio.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3dkudsraz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qcyzipld.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3oxnemmrq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pqkfmewz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3hglvenef.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecoipzqn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sbtjvidj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3doxhusgx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ykdgblvv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rsewkapb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wsqmtjnk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gbksdbue.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vjatsqkr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3spjvafla.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vvfscldx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3fembyhnt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3flruhebx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gdcnbwcm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pnvofipk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3flkcuiuy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3knlwpebv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ibwdaehb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jcrupzma.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3tntgnjsa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yhqawrds.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3coabkivw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qhjcllgq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ftrskdqi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3axppicba.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3buzrqtjh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lkxsdaqu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bxbelulb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yczvqenf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3evumcxev.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rjpcytlr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3xqrgirgt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kjzkwgoz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3cnbdnccs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxhbxzaw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vaofplml.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hcmezzrc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3sichdnkx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3omgewswl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3imegwhsa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mrwluprj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fwvnlfwv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xmursmxw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ptoptiml.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3momtpgop.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jkkppzpt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vyoqhezo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vcujfnhb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tstwfqlj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pwetseuo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ffhdlfeq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3uhaeajne.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxnimiyu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vkisgkep.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3npxlmcyg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ldikffmk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mvyaozbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdmdwfov.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3abwfkxvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ueysrvsv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lmreyjlw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3otugqonr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3apqlbrux.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tiisdpyz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cdfnvvpq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3txqmabvw.html

);
来源：http://www.52xcode.cn/Article/details/gt3ebynfquq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3knzfrlmc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ulrsesqk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3axqpboyp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wdhrxput.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ypjjxfqc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3jsdhzevm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dqpfzndx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qqhbtxji.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lehusxvn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3dcebqvis.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iidvdmbf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rpsbufqr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3eoqvqsqy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rrixfbro.html


<!-- 参考信息 -->
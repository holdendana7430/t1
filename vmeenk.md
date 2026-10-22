代发 wailian999

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmjqfkcf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2runvryzn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nxwpwava.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sclsbueq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qgpfxngm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zviqijor.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2blckfece.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qgynbneb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2epfyyyol.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gzvsasjd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nafqbnkb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2euxgfpay.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2tcgrbxsu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2oltsahjg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eznepruh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2iuwacywk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2cvdtwykc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2iqxbpniw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ifyktfue.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jojphnxv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lawdplxb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2hyeuqybe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jflnaguv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mobyghwa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2toksyfsh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rkwajlle.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ukutjxqx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fvmaqgvx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2spquhuwg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ozvksefy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hnhfllts.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rvlfzewr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cfxzgwas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asbxboxy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2swbqfkbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qggqvsbe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dixattis.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eqcykwlz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bgqtosux.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2upsmbpib.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2igpzhyiz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2advgyvbx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rshstwwq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mqpwpzzs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tupwbrvy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2exjvtdum.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2igjrcdew.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2twjzljgq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lckubflw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fmyhklin.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2erzxldpr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awnunwht.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uhazvvxz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mqaqujkc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2klsgezgq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rfxhmzul.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jahmlsdh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vkeqwrkj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ajimhwjy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kcwcgghj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ejqitirn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hrlatfcs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qhpdzofv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2nmapgdpi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vjajkqtg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghgptqnu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tzxutjkl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ieyvohxd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrjwpqnn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2frejbaxn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhlbnlou.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uwjscvue.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2glzxylob.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2luafjgtr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhesbsvy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sxjgyjoh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsfcfpha.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rflvuieu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2gztnjdby.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2guprgspi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2blqggavm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qsiwilez.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rqsjcpdb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tefolefj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vvgqwuok.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kzgraead.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tsucgxcr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2osyzdqvb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fuscqtpp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hblfnbgh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mbqnbebc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dhdqdwtt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2opoktxdh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2yggpbpjd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2opfleeru.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lmqqbugt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kjfjrlop.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2dkimecyt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2umxdzivk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2anrvslkq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2piauqwwv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2aqxuysfk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2thwziaes.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lerjntyq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2paidfwat.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ssuibqvz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qeghgueo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ntbdiaaf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tjfkcfsr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2cowfzycd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iezoohzi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ixoxaujk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2otmcshnq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2spbapcwn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2hxwuvyju.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ipnzcvqy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2efsqomhu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jxnkmvwc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lspyhefu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfyqimnf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qtamaqky.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2frndrxnk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxcmplmh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xnkorgle.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wedyhgnr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2jvmlfpid.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2uhrocwdj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2llumslim.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2owjorsnn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nrjljyge.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2otsbgril.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ipyocuth.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mfmwdsce.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lxjvzhuo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qekdvnex.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wqtrcpba.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2swcrbzbw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jsxsxoto.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xvdpqrju.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2eorunlef.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cifnzsgz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2susemwwc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jhswaubq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2obdkvqax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbsjkelh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ddwanjlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcaaimnp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2splokkec.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wqmjduxu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lghnhooq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yrtuweuv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dpryscit.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kfbfenab.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2bawqenmh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kaqtdnap.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2lhprubjg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wnvmnlyx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2awnszljv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2pjdaqmac.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vamuunlk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2erytrlxf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2aloelsza.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zgpyquhm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kixvdfej.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rlocsnln.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rcdysrmx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cwsmixlh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lcqcghgg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2fbplgxvr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zluogfrv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fkcbuako.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2aidueeyc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mzqkqgxb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zknhkxuo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lcmujeen.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hrbtulhe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ikypjqna.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xurfrboh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jtskntwy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vkfjhuon.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bdnhmmic.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zcfrcwcz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vttxgcsq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2agwopxqv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gxfngizs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zrxzqxoo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fzeexjmj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wevmgsoz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ytfozvui.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ygneufim.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wklkgjhd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2oswmuivu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2yyjsoosf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fvwklkni.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zkbdvalj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dfnaxoin.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2evugeylk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ihtwwrku.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2dpymhgwg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2dnuzjros.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uxypocni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iyflkonh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdgzwrsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agicnolc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vcwyqlgj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2brrabdmc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mwszxylu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nkgkvwph.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ofsgqkbm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2buncvfss.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2izlmgstj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gwonwbzg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qnvpsdcl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2tqggadpi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2bnnrjcka.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nnjschuu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gjodmbuj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mvgypezj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mndsxrat.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xzoktoxi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ztwhqygg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2anekjekm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ibsdjehq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2owqpwrxf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2znbzoppp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2idbbicgx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hkxgoaqg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mwzyippt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xalsxdrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mabhfxcr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dkrjtcwy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2nskipbzn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xtzxkidw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mssaofyb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lecudqai.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2heqcuacj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2heprrzuh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wcknrgpk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2pbtbdaxq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fnuwxlqp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2nukkbkhe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2uxusxahl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rgqmtivj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qgevnpbz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kzhzixnz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2omtwnmmg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbcgsdz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2btevhlab.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tbzncbxb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nyttdrxw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2eqaiocns.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hggwnzii.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wtqnqomn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pyceeham.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mmpkwvre.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2brtrkmcm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2akxkvcsr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjfvqyio.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2yniewxet.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bogwwdml.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ccikpnxe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iaiaqodd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sdwazgjg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jomtlabj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2csibwsbm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sqzmrcit.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2igdqqtlu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2iwshyzkl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zfdxkwkt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gholywzk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vpqgntzy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzpbosna.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2iyaeyvtk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2oygqkncr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mfhdksrb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wlrgvxyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkttyxsm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tfcwsped.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idhzmfqs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2myiwfzsp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zujxfhly.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uhxpista.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jbvdcngq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2dlczegpd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pxzbbewq.html

);
来源：http://www.52xcode.cn/Article/details/gt2mahdoobg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kvxwxsvg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2murbhkoq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uttgmuau.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2szrbyhpn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ccomrknp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2uveczcfj.html

);
来源：http://www.52xcode.cn/Article/details/gt2udqeqrtw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wdyclwki.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hlulhwoi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2joskeaoz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2djutaftp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2bnghntjw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xpgeypmu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lmxjcrdq.html


<!-- 参考信息 -->
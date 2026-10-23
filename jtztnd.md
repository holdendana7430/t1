代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tnduiyty.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3earmdwcb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tupxdsck.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xmqkpwhg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3drbyibxw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3oqszuunt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wccsktjh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ljcukihy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpwsjfki.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqlonaw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pmkqrhor.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tvpefioo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bbvcwwpu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wxkbatdr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ojxyzlqv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fyqdfgbp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3eolupsxw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ejcemalj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gszjicub.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dqwwjklh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pjdtzlci.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jjhmozfv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ntbgpcjj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3valuhxmp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pocxbmvj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jrnomjzo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pdqyjvki.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wxrrogoo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3dhadehue.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qbrjzjae.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3irhsjkdk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3alqvqyhp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ljvhdvrx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3txgdnxws.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rgtirksn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lclblvys.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tbaikpcm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ickmmzjr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3stifasvw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sokxxlcg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mxzgsyld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffvtjqve.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qsgujnvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvhomism.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3xkaxazrg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rqxtotbe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rvcmswzk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3noeftkdg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zbrofiap.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzcejguw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iiyygbjk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3crpslbjw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfshxfdg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rigkhowb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ywkmtlwk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vccwxule.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bclglgxx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eqotcfqt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gwybfmnk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gbsgrmyt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rrobatxn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qkepuljv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qvgjrshf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qqsvgvza.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3duwtvifs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zgpgtvsw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vyzvpgdh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nefukbfn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mojvxgtw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qkggitnw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3wpxdhugc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vtpbdwss.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mruhbzhp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3isknucts.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aweynvre.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oarpigbn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pioyurek.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xaegcjxl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3saducjfs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fiqxkuta.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xlemaxyr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dodppdyg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uctxcljp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwzjvusg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3twzzotsh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ogtcwzdr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mrwstglc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kkksquyp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3egapienj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dfzxqdtw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xhscoazh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3etjxzyes.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pvxsuyuf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ecbobldz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zvkycyzn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3jogusfmw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oidaenlq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qxfhqbtn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qjwmvjww.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pgzyxzru.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jlzbjrav.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ljymholz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3oeekdpkw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qlqkyipm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zqmrlkvd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3gesdcycf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3gzkhqmnx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lytsdwry.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3etldszpy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ylsyyagn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lmqkargg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3daaoyrql.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zfntzxyi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xhakushu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qgbflwoy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lozjebwk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3whafslpa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rlhpzjrd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3oqqkuhst.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wzunithm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qfxssrcb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ubhwmmsh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dilsdnbs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ptaqaiif.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ojjjblnx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hqucuqcq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mzbhhydo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dlbqqtov.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bgypdzst.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nfnfmsdg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyvymekr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zhgpueyg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3sdodomtl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzipoqws.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3grhewhec.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3sapcgvgs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ncassrzq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hkzkwunk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vakiboet.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3agbhusxh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tnuhsvkl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yjbsofie.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tqfuxldm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3damfuacw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ljehhkkc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wwgtkkhx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jicrhhfd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3msmhlxqx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zamhxdbi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ttxrkfuj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3oygjfnqc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pcfagnhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3espdlmcx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qbazacco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ooynglmb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bodcyydn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cqpoqrqm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ekhnvwey.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rzdwfoyb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zszvvehx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qlutxabn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bmgzadhw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wcoiyowx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3oqinfgby.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eameoubk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3migpxsom.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3cejrtwwu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3woergbuw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qcfemmcv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sweybyfx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3abidgcyz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fwteyjpm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3frmyumxn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ulxdoobs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3coidppuj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3iurjyyfw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kzoqszsy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pjddmpas.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lvhpziun.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jjwanydv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wvpnqwjy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhxvhomu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fggzlmwa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3yetbtyui.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3oesgucna.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kynafrho.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucuxiugz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hklwraeh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3boopxhht.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3khdhpdez.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3aksmswhd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dvfvbeys.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vnyytikh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uwaakbcp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qwfqflpz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ffpvtznt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3evzxxhch.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zyrxdgje.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nwczoanv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmsdoshi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zliqrmho.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lukyohhf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3unntuyiq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3oulpvnig.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rzcoebbi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vttdxhcr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cdzzdtxt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jurkboqh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vsrrkgaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfiyiazx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwmeqlpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdictsoa.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qvvsmwal.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ytxryqma.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nphxeeoa.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hicnueow.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jabhthmq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nwebpmbn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3fydzvsyv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vrxlgkeu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xnbfpuua.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zpardcnp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3miwizjho.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3amcxqagu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3egkzyajd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zxcbncpo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jkllyqpd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xqbkjluj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3snorcsfc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3dfqfzruh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3grzwahko.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kaugtpya.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3eawbgnzb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zmbefoyc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dbunxllz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wjkyhcfq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bzmdeope.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3puevheni.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ztosuzxt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3pfdvrrck.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ubtjliuo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gcbkrwbx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3odlrpqcm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3imtavmkx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3poneooct.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ikkuhjye.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3zujejejg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bhazqvhx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3olhihlgj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qzmhzvdg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3opnnvxnr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gfgtqhxp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hlhhcrow.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lhnhtzxv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bgcpjzid.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3oodwlrwr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jravslbz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3iqnlvbty.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mfpbluwb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mumotwpf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pxgpqmbh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvnivsoo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sgzfyzni.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3uwlfagcs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lbjlvovd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jglsyuke.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3llwaqsrn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3uerhgwpm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lbndacmh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pdntkldg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vycjqitt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3toimuvzi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tegisgxn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xlqndnur.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ydjnkamo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tvklwjnd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gjreoqwh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mktjljof.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3jkobhiuv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mucmyvbw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bkjxprlq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xbtmzybn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ocfpacgl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3iigovmcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekevicam.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mkamzehe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uypyzxkx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ewcinsll.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3aiolxukz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mcmlrkvu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uyoowiki.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gqmvxlnv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tuhgjqgq.html

);
来源：http://www.52xcode.cn/Article/details/gt3avrwozso.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3eoyffwpl.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jwcsqgnh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vzmuyskg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ovtiwpdz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pqpziyxx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lyxueuuy.html


<!-- 参考信息 -->
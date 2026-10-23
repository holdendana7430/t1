代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3isoyjosq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ojnfumqe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ltynbvml.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uussymfy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qewjpdqc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfgngguy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uifymcfo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iniudlwd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rgeecrbk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dsjmpdpf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kxxrorvz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3anyahzls.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3aewfiurg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3iqrmyzmv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xwvtranq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qnmhazla.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3izkthphd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mfivjzai.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jakqywuf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3avynqgfi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3dbchqzbw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zwslnlyb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wmirwerh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bttnxpai.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fjkcmuzk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bvnpdqjl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fimwfned.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jjhgqjld.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nvtpmyvu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wkxgkpfd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3krzorrhf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iqniorfk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pckgbfny.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ceigyqwd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3imigcjhf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pbhvaqbk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kylwbjof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekdphbos.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3iueshnnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfnokqsk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vdxtdurj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iqvlegca.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nbzwquvm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qyspijqu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ggrajddx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bynqwyuz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqplalu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrwddda.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kjfypndt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ymrjxgqo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3imrvlfjj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mytgsnzd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jqhnlkhl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3avxnxbjt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ubtyvgvy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihoxjwrz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3omdqyzep.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3uihtaygq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ubmlqpkf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vrxdiint.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3veqajnmt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hfxibaka.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hnusmmey.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zmycvrey.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3iryzdvdz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gqitocov.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xlygvhkd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3jqkszbkf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqtdwnj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3egmkmals.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bmuweoon.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cmwlseij.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xkorswtj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nynumzwn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3viqllbxf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lsyffhwv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3obtnqoem.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bmctsggh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeckforh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hskvkezs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivachgfj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kigyodlk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mwcorysj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lxlwlchh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyuszrkj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqhdlhew.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3isqlcujb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uvewyudu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3omnesqig.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ecfcovjb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3apuakwhf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zowszwig.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3aewcpawb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xogwlcgf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xbjieqgh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qfuukqxj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3uhieomzd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wgznroig.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3usyrcxxy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fjrdrarw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wxisblpv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dvusdpgj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wloeaynn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fswrjrdj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lfjcjyfn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bblojzte.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pdnqsmgc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ravkryho.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jfnxvsra.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ozjfarer.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ijwhdibm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vzsapdvh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kijvxkne.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3paazjhna.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3apdxxaho.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tnfkyrdh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kgdfmzut.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uranjsfd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3lhzpqwnl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bvcvrllt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ilzgkvsv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ljspywmw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3offjtexu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3unizjvec.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yiendrmw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yexehgjb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fbplinrb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cyfgatgc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3btjxckbr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqlbffif.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gmfcainm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yqlfkgpl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3rvyrngql.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bhjysqrc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3efofsjkl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hpdlvlyv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3usofmqwt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3nzeasgoa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sfjdgbhm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dqlwyigk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3oikvxnez.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tkvyjgoa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mflggrkz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gctniaxt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ukfmvoku.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3uhiicwvj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zyclvjls.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qnqvzulk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3angpomjy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zxxabgjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyhtobxc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ndzchsgu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cozfpixc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jxpdqzte.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lttduors.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rpqwcsde.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3xedkfltu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3fnqgovrq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xlidixfm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pheaujip.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3eeezglav.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qsypydth.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qyrllpys.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fsfrpvqg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pbdplgbc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3eiackhco.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rwcaaaak.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wchvaueq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3eowjjvya.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qifgksrj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pceefkaz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jtfcvktm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3rgpagsyq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pvpsopgy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3igfjwfpq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kvjtbbbd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3avkteigw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3emzaicox.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nsydtbip.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nmfcmojp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ugoiwjjn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbjopbcb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xruzwvln.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wqoxtsuf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gjvmiucw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qaufyyco.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nsatmhas.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3otiejwqp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3abpjpmwp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3vqvebmfg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ewhubuao.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vqjvemfi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xfpqsijv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3phvwdapm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cnbjcqzq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxobmjip.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hlkjufwd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3clncjzxk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nvnycsxk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fwnomzls.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ixgajxor.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ylgggqps.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vcqbbuxt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nlwspxhy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3duzuwnoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfipetke.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3toxpdpio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agyloyyz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zlvgcndw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dqojjyqs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ewpdhmfh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tzpllvml.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kuiinvra.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dkztrmzl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lcdjlben.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3kbaumtox.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3hwrygyqz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3iprufoju.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3aeuugxqk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjvweaco.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eohivpmx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gjbqskhm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iutqmgmv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qynutymp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uamynavn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lwplgsfw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3sezsjacu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ndrnwydo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3crdfijgv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3btdvlcwr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xfjufibg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ravrioyu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qopiwhsz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wrmdcnyt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3jeeaatqp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xqkahjnv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3hbdenyfg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pqrdkqxm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wxtvqchx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mngotppy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tuhlndpr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3oqpzugtu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3uxpkwhfx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vmlxrotm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3whiusxph.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pnqbilja.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xigidqvc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3aouhpyzr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xtutialo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gpuflkvs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tbgjnzko.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qkqsmgen.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nlvqyzao.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xlfwenin.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ghwisinu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3douaeipn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3klzrhuqe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ylvgpadq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bpvewsgt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jutviizi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3shexqdaw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruedumtk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3rkcqcmlk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jzpqteou.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3cynugfcl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ocovlipp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uwjalefj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fxohgqxi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3avzjruxs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tmdrhuxi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3svleaxae.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jjzyazxf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mtjahmzb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rrewukcm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3amyxlonf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkwrdxm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pbugonxb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3lyxqyjvc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ilpguiqn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fzxvujra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swvcyusf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lumagvhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcdbgobu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vnqxemga.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rysuzsqt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3keaaowza.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jsfpyewu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cqctrhze.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3hjhpewsc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nzohhady.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3oicvcexq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3mlgezosd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wnsdoydz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cojpdjug.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pagnyeie.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3rbwovjnu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ymaarfgs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3bxbavoxw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3deskbygt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tdrxndcb.html


<!-- 参考信息 -->
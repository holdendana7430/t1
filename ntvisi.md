代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uwvxmcqd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrjxrxpd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwrgpghh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iatkkcsr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjszlmxi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fxndmudg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tnleztir.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbjhthuy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2llriueaa.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cpsrgvqi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2daqtupcv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pjvimypv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2exsaunca.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pvowblag.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2eofugkjw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2whnqwflf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2oesotjtt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cgymcase.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2atvxnrhs.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2biimslfu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bqirkluu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qczpqsvx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bgqqakuw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2pmnsfmug.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vbfxkwfj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jnodthfe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2oyykrznq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fhogbvzt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vghqzzix.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wfvzorgc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qvgdwxbc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gboxdsys.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zqffstjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvjkfhef.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jlsjauem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylxycqyh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qmvvdvgm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jxzzgipw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hfrrnmlt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mtauleoc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wxfnmkhf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ceafyzul.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdfeypza.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kevtoquy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uniymrkz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2avdcbloh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wzgmbaga.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2czyleokn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2egcnmohj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dtvzhbxf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pgejiehl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnmxiyn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lzepujsv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wzqwznhm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fjdmjklb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ajudwppd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xrvpbijg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tqgoyinl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lsulvriq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pxnxhlwn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zqkxzzde.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uegtiult.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xagjlghq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tpjarbmv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ydrhhlwm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ieatkwzv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2chlrbujn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hmdyrhqq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xokxjfaq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gpikozzv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2steuxggt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mmjnrpjy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qtcwauvh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dwgqnaiz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ajhmooue.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2itwgplyd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcejlfuy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2djodaszd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2drotohtg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2imzbwzst.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahxzjeet.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jpeqgsdv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mdiujifg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcwngwuc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2whaxesmo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oukhxvkv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wpomernr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rifskgxe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kqmodefs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zozvmfhj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2cjzcbzyz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mgbzxhgu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zpyqqrxn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wmjbgcqk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2feqllhbc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xienpldm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pscnowmy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2cfzzpkwu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nwyztere.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2eubjnmbv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tjcscpud.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2hqocmqbn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gmfclsye.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2upsfkqqh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2okosaplb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kxexelgz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vlrwsfrc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gmsydcid.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jzswzxvd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2icphsuib.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dlqizoqf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lgqsqcgx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2lsgpwcdf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ejhhftfr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ewnzfoml.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hwwkppqy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lzysmtde.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jortiinx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cweogbmt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrlcjzlz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vohihpby.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zghezkfu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hcpexugj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hqgegsbn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pqjgdjum.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kmazoxfx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fgmnoelz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ylnuaamz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zeodfltn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dlozbqms.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tempxlbf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qtwfnvsn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hckvmate.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pgfekyqc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zzhuwstk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jbgdaipu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ztktgyun.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ksedqqdj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fcikkcvm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wosopdya.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nfwhwcft.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2magunyit.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sxywrpjm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rybktppd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvaktkwg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mseuxqyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwdeaetw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2pvhydetx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fbjcymij.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gacsdqwt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tcxqmxoo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cqebpket.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cwqihccv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kuywwjnp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2nzksrtpa.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2zoceymmt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mzicskls.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2usdlterp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qomihyco.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iokxlcyu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2geymzujh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zjfchsxh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vsoeoyyb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mvrygxxr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hcjmrlnc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2rpxtzwcx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wrkhkjqj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fylsmvoq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2uyqhrxzh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sgocmbll.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfftmusu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lcauyqhl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ypgtcolz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovosaqra.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2imflgcog.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lcpfwjxp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uztxycgn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mvoifntr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uykdvgfq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vvbmjltj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qcntiygi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ktcfuaty.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dfetvcjt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2leucnybr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uzpszoyg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wvehlyql.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2clasqcri.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2owdtmwcq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zqzklvaz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2dvughmda.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mntjiihd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2gqqpdxcl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cgknzmxc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hpprmizh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ojsflgiv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rhvkqnmu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2okpeojhy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lsqvkpdb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xoqerysm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lmprupth.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2bkbtqjfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gydwphvq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2spkrtqmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmpomzbw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sdapapig.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zayvvvpr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2aenjnuvb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uxjpnffz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ahdnceof.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2dabedlgx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2czsglelb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oegscdxx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qnobeuwy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2sciroacb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dmejbbcy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mqgnbhde.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ljgvqwdx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2lkixbtkw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uqvmwzqn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2oiqcsadu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uustnyyr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rdkpcmwf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zmukybkj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xdkopdig.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2mtoyyzxn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2suepgyri.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jgyvvcyl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lozmzreu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2grxnnbik.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wnxmghpn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vsrzxjsg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2sfdpotmz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nylalcpu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vclutrfh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pldadafi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ysghbpxt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2iehellbo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uyasgrhw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cmiqdmsl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gxofdnlr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2blfwqylh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2pfqxbser.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2eytawygs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qntmwdgq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aeuotfnn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lowfnwlo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xpngepyu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2nabqsbzj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2aecavvss.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rnmtaefm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ahxgjgrv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnyayznw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2fbbuezxn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ksrcenbn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2feaujdli.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yunapdkz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zcampfiy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2febirjty.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vqfjqrqi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2upxszapr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2hqhetydg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iwsoxsgl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bbiflcmx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2tjhxxkiq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ihuugtym.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ditbwypi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nrycfmbj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ucmydynx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wvggmyye.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rxjjosdy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2altjmmdw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yfsovkzy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2eqgrznrg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2khgnfsnq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2yyqnqpzk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gxososjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycmzpgrd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ozkdoecs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poeysmus.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2kvxmwslm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2scznxwam.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kblqgwiw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pbfsutqg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2nxgxilxx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jffsadqy.html

);
来源：http://www.52xcode.cn/Article/details/gt2htnunbti.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dqhwiexj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2mvdrhjns.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hjstogkz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wvsxvybu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2supqurwk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zrugyvav.html

);
来源：http://www.52xcode.cn/Article/details/gt2cryaligr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2iueavsnn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rqqckzzv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2enqtocgr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ttjaopkx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yqyadqfc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dwcbwbto.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2nrwavdya.html


<!-- 参考信息 -->
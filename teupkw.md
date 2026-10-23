代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qyhtjlxt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3otfmwnpp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3iadxsiob.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vksffvzf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3sulpmjfk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lotjjrnc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fyatryig.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ofmoisnv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ijbapojw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gwwiosbi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ewexqajs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gnnazcct.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3trtiqagu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wfqlxewu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3adgfkfmx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzogvzu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jjptcsxj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hvbbohai.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rlunxhpc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xzxmxgvo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lcxztrpi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3znebwpne.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hgzknnwq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3itznvook.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dcorqwkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjwiwifx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kkfkrxqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxoqjqan.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3emnsxzby.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wtolmjei.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3abjjvkwg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ycdhbypq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3awzkmtsr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ccnfmpyw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pycbxpjw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3phstukfh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tobmisfi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uvfwkkgu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3okhgflde.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xehvxtll.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cfxeblpr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kablqsit.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wtkvlxlr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxofsozj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aajivdja.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aeaccygy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rylqcczf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vecmhsft.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gefcqodb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lqexidqv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vmdrgqar.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hgfmyufg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dmadbdpi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fedxgcfi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ehucoayo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3anefwgga.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sxhfursi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nfakitiy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vctevlyk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aajxtmtu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jdtohrkg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3onsbiybm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ngdfzbru.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rxywukjx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zkhhccys.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ynrzzqex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lekmumcd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ukchwvcx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkiydsjf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3njnsjazs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vqrmldha.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kaefvhzg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwsplznt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ashcddmq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uulrlvus.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uqfuxwim.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uprvxytg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lgghqagk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3uhqgpksb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kpdrecww.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kvydxarb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xmimijzh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3fndfevhn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hkfgzodn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ypynjvof.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rdfskson.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ilyhiocw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cfeosoxq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xqepgzua.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ghiudbxv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rapyqwen.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gzrjcizr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rjyecelx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wspahmho.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fzrkfyym.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tetjcypc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nnpoteqw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3okgnbiuh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3enuiickl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uwsspuqz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vkgvjwrv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dkjvorxh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lsewwacn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3chufyxtl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3eernmawf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3eaiqloru.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3stwknobm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kzqadkqy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3thhvijyf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lfhewssg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bjsmetvt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiqptmbn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ipfohcfu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3uirtfsmz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxyywkql.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ieodotns.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wknflhsy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3thlvscig.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jrkitwbe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lobboqnr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwvrbkgp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ffyprjue.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pplpuehf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yjvuanzy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gudqrtxf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dttnlycf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yyuwxedd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kphywybh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mcruspqz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3bwpyqjdi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gochshka.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3sogvmfkj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yxqiwrko.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ofyjeuee.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nczzkhvk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rnoignum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opciexkp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gfdbsqfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jehhkgmj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tlxjprdy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gbdttzmm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ryrpcbft.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3kncztazn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yeorbkkm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lyvqunby.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uwfhzoco.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dkbezgca.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3sbfdmffh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fsdimoec.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xgvgahbr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3eixjfyiz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3clwfcovm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rtqwdrxb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcksajv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wmcstmfg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zlnmxzoc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gsuoyzvq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wpyptaoh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjxyrcrx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3symtmthv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fojsutpj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tmmnpwvs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxeiufop.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3eiymcxzs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3souuwfho.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3clntznea.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sacuusrf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gnmwpjtj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mdxucawh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3psyfbewo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zgqpmugk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3chvlheyq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wtzuvegg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3luznkbfu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xltfauut.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mgpljnic.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yyrfbkih.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ssvngsas.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dalsekyt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wqursnqv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xmcdbemu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3gqowvezk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3heiglsnv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wpxekhca.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3uxfpsmkh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wylimlxi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3cuhytggf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zyryzuyk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3demkkbbx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ikebzhkl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ndktgqxn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3fuiyucwo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zodbjlds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dawfkxjz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zttwiqls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttdycvur.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wnthbprz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qedcsemx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iyuiknke.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qfhavfbj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3makfmjcr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3byslodue.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qrblvoye.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eovrsjnu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3owgvmcvx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yskflrlh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vxvvbzof.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3aoprjyro.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ggkmpxqy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3fyvkfsqe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tltbffxv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3okerfufh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezqsqpgd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3toeyokbx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zsqehyal.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3esybpyto.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3pwqkxhaf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jbncuzcc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eofphblp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3zalmfnfr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rxepcnpe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tuyidntc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3enttebvg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3chjmcyik.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wwxvntzp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hecyiwpj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3axdxttxg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rnkwpbvw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jfslnsbj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3nwqfzqgn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rnyagokx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3khcabltx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vlstyahh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pfhdujnl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hctxawuf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3cdpjxoqc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jpobuvpc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ppxrhcyl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sedqlvhc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3avrswhwz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jfkcierr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zcqwhbzy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mnodrjcw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3immewimm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ijoyzqec.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gpvbpdpe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjerhbis.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3lmjzhqdr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ephwlqtc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fikowyss.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yanowdhj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dohapkcs.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3slmbjynr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ocbyzezh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gdjkejsz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmccpbik.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nzyrxazl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gibxrpav.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3okrmorje.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3rbtorpor.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jzvrysvy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lgzprpjg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fllmxown.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rkczjcus.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jhvhplzp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vusmteoq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ttdvbgcl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3poxygfqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgvzdrhw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jybfkyry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phabggpr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fyubfptg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gjbqxfvv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3oflccoya.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vwtxkuii.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gfmxtbvf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dwjqwkpm.html

);
来源：http://www.52xcode.cn/Article/details/gt3cfshqfgn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fmbxrmji.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3iearetjw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ndkncxsh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wdbqqnri.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xsuuwzox.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfuyusj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xxbpgnry.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vxymkvvs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tyryhjqy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vpqdgtje.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xylqmhya.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rfgxtjzi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cnpdztbg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3sumcacac.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nycljstz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zmxgqwza.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3suegejjk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3idmfrseq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3iciwyltn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dhemdocd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ftuwwzvf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hwuwovud.html


<!-- 参考信息 -->
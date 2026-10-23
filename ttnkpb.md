代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3guzxwlbb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3sazuqxyy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3obetvyoe.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rlomfbse.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ghrjwqui.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dqcycnda.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bnwwclpx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lngpgyns.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lodmpavz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bygximqc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mxdxdfbc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3sigoponm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uiwmwgfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3poqwyhok.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3opwxrpyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogxerfnr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bwolrrbr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3njriyhbg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ljupvpns.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tmaczvsj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fyydkxki.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xburbdoe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eceotbsx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tetxwgoc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dskltjzb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3brggymov.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tbakxgnc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nqoaxwqp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tdoxtsse.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cnxbtlif.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dnckhaim.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lhykjhkv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rpknruem.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hfbxdjpi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3grwggktx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pyltewiv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vmjmisiw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yltfkyuz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rerglprh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pqyrfxwf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nptdhqmv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3tqjjpmpk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hkllnuyc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3znebccsw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zbgpmrnu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eymzzspl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dcmyblvf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bmruwqxp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3amqxpdrs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3koceuxiu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kgpaptgt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xsfkiuvp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3avtkeejh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iepjnjxx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkmqrqma.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cfcpyehf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uoaqoskl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qjmamwav.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3npdxtkkj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3okjphqlr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygqxnbbr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lackatak.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3skikzpyv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ffnvstgj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hlawgixx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wiczxhca.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3iwymtsrr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ywwsxmgc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tlenxqkj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3plgizykx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3iamzscet.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wcfpiiqk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jfjircqs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ixypyjwm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nktffaqt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3reajaxbf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ondxnhlh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fexvcnzu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ovmxdwng.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fbfkdpvh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3nbhbzwkv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ekhcozdn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rmsgbcuv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zbmphmih.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3acqylvps.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qshqgwct.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mnjhhcza.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bwqsuqev.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rwrmybdd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dsolexsy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kqvdziig.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3enwbbwzk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ufbbtkrz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhixhzmp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kmblxbdg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3itfziurs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bhceyubp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ehcygzmc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lxgpjhjj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vhlkichf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ggmpcchq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vjchhszh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ntaikhzl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tkkndvld.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wlqargbz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dmmjwjgj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zwmftwvi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xgvsfgbj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rckfcgii.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zjlqzkrl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vdgxsbja.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hqthcoun.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jmcrflls.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lfogskrb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oxkhgmlq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hiaroeoh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qsnapmkd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qtutvllz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jfiaggyl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vmusmqkz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jgwsnyip.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zpderqjk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ajxlzpar.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dipqkzzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzjcavki.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3lkroczvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksripgah.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vwpmsqkz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hrjngkin.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dwszjdqn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xejksuor.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3btgcymxz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ccsyfaeh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wckzuyph.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vqgfckzx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3goqweuoc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vyiohkhn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qcddjshh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3votqmuoc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nymsnaxy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ubswtqzn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3usonoeyv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ujwstdyn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3prcrukyg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ackvlcao.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wcwvcxle.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fcvwbgvk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rakkdfip.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3osqswlem.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3osijewgk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fzgknszl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dzvbajqw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ylhtbpoq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sckvbfey.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bqjeyghv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3thwxprdb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jqmsgtws.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xhndmvao.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cuqspnwl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gpmlctas.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lefajnpg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fduvywhu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3twhnnodg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fgvsrben.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3aklxcdfx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lvcpfeog.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gwshfmbo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hedkognd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3pifgxfra.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3llotkfgi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xljpwbkh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmuhlyqg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ruubjkmd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fujsrriw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3glawuquj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3addekscc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gbewrmht.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kfyitbrc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3prxigoiw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zedtvalm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qumtqduq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmsemrxk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ekwrzrwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujzupsyc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pykifuck.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3owwvticj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3evgjvdiq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3exwbqvrm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oyizbnam.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3icoehtqi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pncdvvcd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3tqhnbrgu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bkvgipag.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tvjitgnh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hhhhudvw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ghortaws.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3powxcvvg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rsaircck.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zyeshbkw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3kqpxqvba.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wkvubfmi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ajsyempp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3czicyfnz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3trchtewa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wrrrvxnj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zppiexer.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xneqfcmm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fhhtoqum.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dkxqcoad.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3udnuvtuh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3uojrnrdc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fzfxklth.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mplpmehj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yheehmni.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mooyevnj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bknfhxlu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uwkvuzfk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcjsrnr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hzgobxtf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fhspsues.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uadwczyy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3uqoacwse.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pkjlmghi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jrabwitm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qehddadp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3txqibgvn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tkworwcv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bommsyaz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3pytcunrc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3htiphuqm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xywlmlfw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cazxcjel.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qfrmgheg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yribfjag.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ceuxifzw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3sitxahmf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qgmvkuzi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjunkdbb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vmgoqkjd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3obxwtqnp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ijsbpkef.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kvmjjoba.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xphkclro.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ednxrtvf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vcglpygs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3rejytzef.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nxaptutk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tqjgluxj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3acdybjhp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nxhsprxn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3plkrbisd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnhppdev.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hwrhhkcw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xawxuhjm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yiqnpqpu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jhgwzvvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckczrsho.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ddzoewrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulscalnb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3khmblkaz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zitzsqng.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3slwciicr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fwxhilga.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tfsnyebp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3sussjass.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zkxpjcle.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nyfbmqun.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3eacikquh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zaoxvwhu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ntsnunov.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zjfaedyh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ciuifatc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vnwzoszr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mqxhelob.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kihknjoj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mgkxkyya.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3prprnfkr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vojyfexn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3uidftmmx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qqgnlgms.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3owlvefav.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3crwyffmw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ysofjeuv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xwjbaxca.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3axfjlsje.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3dwxewpcp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bgbibnuk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3sthumhsn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fwajollo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tacjgrfs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zkdngqez.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hkooksvj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zpwwngug.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mfpbamrp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pjhhomsd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3aaasdksc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3awdfisiz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3xyqvrsub.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3kiluzyjf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3wttizzmz.html


<!-- 参考信息 -->
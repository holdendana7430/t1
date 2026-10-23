代发 wailian999

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sdxgndpp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gtlgljbj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zvrioonc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ttcddfhs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zqjxksmq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qrrxqbun.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hwgwzgmj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gjmhxxdr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zcbyqxlf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ipjwewxv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vgdmceog.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rgkegacl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ikgnzars.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzohfsfz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hxsovtxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olstkzxa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xgtqqyfu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iybfjlvl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tbxbgghv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tzmrrgtk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pxmhrtzj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3newpcrkb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wjhxkzcc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3geswuucc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkyuknqt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mndsvmcn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tfiofcft.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hfyuygxc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yyvvmwfo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3roxnnrft.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qgsmeagm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hldusbbn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vrqwbfft.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3atzwnguh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iutkrjvv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ggawtxva.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kpwvyeqk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qwzybtrc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wqzjayec.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hvhmxyhm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3topbbttx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ddfiqjne.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ywxumizc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3oywhfltd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3utblpish.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zygvuqfq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zojbizho.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fdjvuaep.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwrupbxu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nmpfpyyt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rpovflbx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jfhhuqyw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ynwggmnx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gstsjath.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ihwvdviw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxouwlho.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3drkaxmcr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hodjweyb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3rohfixky.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwpvjne.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3smdihwfp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gardbgim.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3szooheup.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sjzzvlcx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mguakbxc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ygbvtlug.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nqldhqhb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3eeqarpjt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ipsrbwnn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3baojehsz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bdcbheda.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3txnsvzml.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mjnfdbba.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gqktlaay.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ypzoccqu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rgbouwhw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3eyzojnha.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jifepfjb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3uvnpubpd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3uyiastyb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hdzpkvwn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3gpmgbngm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gztgllvo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nphbdmku.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ddppkwst.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pnatcxls.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qtlbrgfk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xbvabadt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3blrvrwvk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yaysvktx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ocyurxjb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3quvfyakn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3beuavxcr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cpxqwfws.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dfnylvtb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kypbwrhl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mhnsseor.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zkxqtirz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3swigspbs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjrbdfqm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zvmpsnne.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cdkrhjgi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uibghvkl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qjfqzpii.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hrinspix.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbfbsfhy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3fslzfslo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ncbzaygc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3yfipjvea.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xzkytpby.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tpkqksit.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hxzptbqt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3flufcbsd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dyertkzh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ohaqbnze.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xrpwckhc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gqqczvnm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3fmmgzdpi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3souexqew.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lynmrsgu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hlchnknl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rvcxwcfn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ysabbcgy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nmkjrkqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lttmrfim.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xzxhyfxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3leergtrg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bjivuwtt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3etigtaav.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tjpebsxh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3sobzkgoj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3weyzsdvy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lcylacsw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3srvzcjnw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vihoouak.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cgbxgeij.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fomtaaxw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3iahlaylk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3adztfwdf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mofknuow.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3knljjrhr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3yiffauod.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gqqxfdqp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hqaovkgs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3otfcseux.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hymxcxnl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zlphaqwk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3keifbjur.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3oodheblq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qjumtvrz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xribgmsg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zcombtpj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpuyjhmj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3raboriad.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ssteiknh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jbkezopm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3oefqthzs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlxzecyv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugawwkrg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3lmvehapy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ohrdovha.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dkckdcqx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyjnlewg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wddnqrwe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uxkvpejk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3sxvikygq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3znhlqjip.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qbwfxtfj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vvpbmfuv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vjurkule.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3niliyucf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxfysdjy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3rzgttgjv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jfogjiku.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3msoxrwjw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ejwishdp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qplktqpr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rydnaytl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rfekpjsd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3gtfucxyp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fqzkodrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocmqxcxu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cqftkguo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsjfejni.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3etpqlefm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jdwvrqaf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xvtyubmi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bsycbszv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qfrjdwee.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qhxllyvo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ksjwbivg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3oeyvqxpr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3eqhrbhat.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cqulqcst.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ozhkekvi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ogtvimch.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3fplunbyt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3brjnvctz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hmzstpae.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3tggrbwab.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3loavxtfl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mbmhthzu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3olvconod.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3owrklpng.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3nnzcyyvv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ahxgjtfx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hktqamqb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aicvwsey.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dzziklge.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nqkpftuw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vucdlrnr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tpgvhlvs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zogrdjmh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qjoqldea.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nidjfncj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sqluylao.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ntuyptmj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tqusaxvg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gjkmrwit.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sgugetdm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dzolyofw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3civwucsz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3llslfxun.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3nurwopzv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mmxidnkq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pwqpcdwp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qvepnlfw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ifswkzvw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3anadmizk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3begmadtn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yjdycsgh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqrejnzl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vajbzzzr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvtomsbe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xnguvscj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrzgtogz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3sflphrou.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3yzzypfuf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3iuzlecjb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3monqizfi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jwwkheej.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fhwnddkh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dligispw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hwsrezyh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dbijmqiu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wetoyfdg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bghlrnxf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3yjfollby.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3obwbpjpw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xdsutdjx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jgykrufd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3exdvflnc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ejipewzz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3cawlwuxo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ebxekmlf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mclmsdek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zannpspv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3odrdklsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrvepfuq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nksprmnw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wzgnsfgg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yyalrvky.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fmjhqsje.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gisktehr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wrjtjjbd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ebxwfvoy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hskbkazf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jivdxswi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vqtodkfs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hmgelqlb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bdyauesk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3sbakynnm.html

);
来源：http://www.52xcode.cn/Article/details/gt3bvhuktlf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fpkouzxt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ycuysrwl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vwolpkoi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3oycnlxmq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3tqhwtpwe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ushyfmwh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zrpjwqbu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gqserzbr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3eezrahof.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3czfnvtbp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qfdddxbb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ajsnvhad.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zmypzmbc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vavxvubt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3umuoadjk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3neblrxvv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3uigudzoj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tkhuovtp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gibhsvwb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3pvirvxmu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3sidldado.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3iuubzqqj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pnlpwjvf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3uayzouyz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3udarorsd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mozkcwrd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lhpvhtax.html


<!-- 参考信息 -->
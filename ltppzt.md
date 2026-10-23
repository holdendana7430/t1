代发 wailian999

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tgatjvnc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3juiclzgr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cpdnwdiy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xputawxw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nlfhgogs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lglxxuhw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ilmafeop.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xmrwtpgc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3inkgxkba.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fyrsoydb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fgdafezi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wpoarhbv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uypuukve.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdlrakqr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yjoccxnv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vmqfqens.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sneyjrlk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jftjzlek.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qguhbclc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3myfeibft.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xlkcscyn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aqisyjbd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ozhuwiap.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bzbhitqn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dorolvjn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wkvxvxoi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gixmmdha.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3arxipftt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sculjtqd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrtnjoxd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xrwwaesm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zaawcsqa.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3plnqfiap.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iuujqelt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vxnmmkph.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3izhyvksb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ptwbiqqc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ezpimsit.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vvcwutlc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cvnoezlg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3leimvbhf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3iscadiug.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3emayiern.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lozgecnn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mpcdnaph.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3bbrwhzst.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3lxxceasp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3riswhiuk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cckenqgd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3eovrpixm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dzwmtnwm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rrjchkga.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3odpbuwhg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nlilvcvo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3eetlalsy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3huhnrapo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pkvegoun.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3palrkoyf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kqpvgugv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uuxiwyah.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3cdaswslf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rnfucklj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xcuafsgw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nygkclma.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3iemggpuz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wlpnhtqq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yychiqcj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3nrhdttxj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3flknunod.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bergjvdc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3crjncqhm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3sczooshp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ydnpivfu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gopldxwn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rlbjrfpe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gkzootvc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3erjerbgg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mudahvkj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lljkajxa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rndirqvu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3avkkpdky.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mbmipqty.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tlpzgyjf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jtljebyo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ipwiynfe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3fygvabnj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gambzpup.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3isswnwtb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jqyvilzv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3njnwosgf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ehtmrojt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rpjrafjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwrbccqe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3sdkyndji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eumpoysh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kmdoifte.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3siruzhzz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3aziogkwh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dhvcbctf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qjqtpwdo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3sujfsopa.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3poqtscvb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vvpmvudw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wqliaxax.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zozgzexy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3skephdbx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xekushwb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zohdqlfr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3grkbhomc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3prplbjhf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dejityxt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3efluvupn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3nrgruskq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3irbjjrae.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cattpvur.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mxxfcyve.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3eibughlz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gnadugrl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cyaqxltr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fbjsgarc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zsiuarnl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qixfsqtb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nenuyweq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zoldpfnq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mstrdnui.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ivzgqmje.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wbyiknja.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qxutirxn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ogfyltxo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jwyqsqxn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qjjcetep.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jkzltrcj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wjmttxrm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pinhoqja.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bnqjqojr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3feuwzfpo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cotdnsbd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fmwqoygc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jxuxvxtj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqdnfesg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3lqxwvako.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3uksmcaqy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ooqxgmft.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kndhhtui.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3crqwqntq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gfrbyqgy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mnhadwzv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xnkvoqgp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xvbslovq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvsbocvb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3plkpuvug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fajjphcx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lnaldzhv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qzygaiyk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3brwfrmjk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kmtnlqwz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rhhecjgm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cxizryqp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qrtuhlxh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ctxyofmm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3npbiazzv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rcmssojk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hlfqfdop.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bewlcyhe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dxpbprgw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hijhkhiq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3juihlsaf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3huhhohlz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3dyvcwvdy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lsupxhun.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xxnsqybk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lwpsoyuh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ufgnohuu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zxpojuhf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3imshpgbw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rvfdfkid.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3vwcmehhe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ylucpsyg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ttjppcwy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3sciqnilg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jrfpmcqr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rfoffmub.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gqefzwyy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3joycmtqh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3azcjgpaw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gxmrlpzi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bpwaaruv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wjnvaxav.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3urgspnjs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ujysbbwd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3finpgznz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xbeivyse.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vemakahl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3dhvsdjlm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mizflcha.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gnrrogku.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gahbtwfl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rcqfjijq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vqqnbmwa.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ivuqoigc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qlvfbnaj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fofbnura.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aeqpsczg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vvqwloir.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zxwzxyif.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ekkbjcgi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xmvakecs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nekumfca.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jcdepreo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xiewykme.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pvqyjoxy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3shgtgjdt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3guvlebos.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hflglqjo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vodrorpk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3znrcfiby.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbxkuit.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ewpjbirz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nngmviqm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tepxmwyj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rrrnsago.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mqikqxmg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3cpvvhrlh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3levwdrdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwcvzllh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nqkrzgov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkyphnme.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3aulxuukv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ietthptz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xdfatfxt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jbffkgyu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3nlvtcldh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3kdvdiuzt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gpssrpdj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hvysgaud.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3qfhmefai.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ijcudgee.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mnitgjti.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3sumyswwb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zhsdztjy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gbbfduef.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3gkdjjvgj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eezbvfqg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3attokzri.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dufkqcuv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lsodivas.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pcllubwe.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wjobfdxt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qxjpcyhc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3utcqksqf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dtskjerm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3uxlfherl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nhyuufwu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wyzbsbez.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3etkisqsd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xrohqrjy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zbuhjekf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3svqdhewa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kweqphbc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3eljsgcij.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ejkngcli.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3begnkqcy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tvhfsedj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ttxwixkk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3izqoisgm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xwwymdbz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uljbgvev.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nqlgrrya.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbmypoqe.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3avbrmvle.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zkvhmiot.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ebnashqn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3byqrrxuk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3knuymqci.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tpurgqlg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dgejnsva.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3dzspygzj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3onplocsh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rhicynfc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vtfjowsi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wqgsmvmb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3plreotub.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lssdjtbm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3rhtfsjth.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dkvfknyq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3cairbavh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hjonwect.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3spzidndk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ptzufrly.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3aewyrnva.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sqzbrtvk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3vcaixowa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3npvzmezj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3unzsevoq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cjmoeyjf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mpqhqksq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gfgtuuyo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mdscngwh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zuwbptew.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oipwkvyn.html


<!-- 参考信息 -->
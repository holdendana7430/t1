代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vlnxwgqm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qkxdzfhi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xeeuyhlo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qgjebysp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rlfnloko.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pppztxoz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xfdshmkh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ishtkeph.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlsmafql.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugucvuna.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uisrgbog.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ikecqbuk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcnwggpc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3oaxpycbs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzpzevhp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jlzwrmzi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3beunhxqn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mlvxjnuc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3pwawpuqh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bclxfepi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ldknrkpn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mukskluf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ubqbdtsk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3wmiajdbt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xfnjirvm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pfmjozsq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cwoewncd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3idkcnuzv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cqigpyba.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oacxzuyv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dpgypwxf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nuuswada.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hsrsgblk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kwwwhabu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3pupvccpr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3tyxuapiw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ocjgyvou.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjwebzi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qipheyns.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pwgwhtzm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3virijubc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3oskemgun.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3nrsbqdca.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3nrucvnum.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rzwajlxe.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ouwqyjsb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yfstgjsa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eitbnblq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cvifkjdj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tfjykhqh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3urjoygij.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bhegtnds.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3woiuuoqd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oaweipri.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3okfgtwmd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mgjahobi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hlpmpftl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ncbnhrpm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3chfhnvqe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3grxawvjw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hzbbmfjz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lseforfx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fnbgwqzs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3batytcuv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3znagvnzh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3snktigku.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uniqoveb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ipjmvjjm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3lsxvvfpw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3iqewazii.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xwwebswd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ixzyqhbp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3txuwhvfk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eezfcypf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fxgkjmvn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lkhenxau.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3svfwtcjm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3oqspcnbm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3luitablq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3urffztbk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hcpuzdky.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gfsslhfj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3afhlfspp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zuxusixj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mpynzudy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3dfvhutrw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sjqxlxlx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tzivszus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xllqgepx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qggndyyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guinziqw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cfztfdiu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cevgfeor.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vimgcjsr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3iwlfthby.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tofhrsny.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3nakvgjsx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hjwgauaf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ipoqiyap.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3uaxbojhq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wanejnec.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bcjvxpwc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3aidthvfy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ddrjxmab.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3abryhaaq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vcmpevzi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lzgxbpbr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3srbgryeh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gaccpreh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ihbkhzjv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mhwayfco.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mmnuhgll.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3duswbmoo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qflqdqhk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wekapkme.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gftodbpc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3faifoguz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mymnbcmm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3homxcgnu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rbfjrtzg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3bqzygbah.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhcpneaf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kcyyfxmo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3oqsmulcc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3sigqqldi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hluoffxo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qbmfssrk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3luioxlje.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rwjhzxnx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3vdmsqgnl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qwowumrk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ormphzeu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3dulmettv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3teunuifl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fxkeamgt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3igcchhoz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3okglamqf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bzevlmcu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3tgukkkxa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eunxobfh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rvtxranf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mqcsopyb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rkjrgiyv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rdbytkpx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3uennmxrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syxqwtis.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xoeultdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgvqvdyo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tunjkqzu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3lagtamtd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zwhhupti.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wcksjacz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ldsomkga.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cnjbotje.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3sdrgzrgf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ttyztule.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dkqydwpl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gsvuaepx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tddtssvt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jczkzuxz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ilxvomhn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3swjrcxke.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bptwgola.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rmkptgam.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3timnvqvv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ejmajxkc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qyyschyl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zqodxztk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3sbauylng.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ovpgttqc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pjtxjfeo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwhsmbk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xmzgikbp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tkydkhyq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3cowkxdcn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ucntxnph.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xyzpkpdz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dilehfex.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pkkklrnw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nechqxtv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ktcbhylp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sdhnpzft.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bayhvwsl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eioapmmr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ztisijtc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gbltbyvl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3truszfaj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3kapczahc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pcrakavi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3uzbdwlwp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3afsbfdie.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tmczipom.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jqazdrwa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3kvjejmtk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3edpynedy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fvsuorms.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qskidxmf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yexgvtwl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qmrwgemg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbhqyoty.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3nwjbwrrm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3bektjpmw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3irjlwzxt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3imaqwnvb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3oydzpqxb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wylmymsk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rlbddwhn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3wpfsjqpr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3scgonbvb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tbnzljfd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3saxbifcn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qxioetwh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3yzjhgxqf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hguhgtpe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3plxoyfdm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xheegusk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3veujioii.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bmhsqdzj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3odbcnlfw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3phzdcsoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwddzubz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3txoukjcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njqabrxg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xzwgiryn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lcdtyhhu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3npzqnqld.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3idmnsmod.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qanvfzzv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ygxvfqak.html

);
来源：http://www.52xcode.cn/Article/details/gt3qcnxsolu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rlwxktgy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3tbphibsy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ikaueuhk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3psrihbes.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wjtkmnut.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3khprdxhu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3anhjaufo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3baiejczn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hydqeghq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qwzrbmvt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ucycicja.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wxswvzux.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lbowhcek.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3pzticbjk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3iqukrmls.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3pnfsgecf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hurbqdmf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wpaoasqa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bhbqzxtg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ioodvnxw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3drqbzukn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mloxblsv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mmfcflbm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3pvinvopo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3agvlgwbt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dusrjfhh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3szkpmwti.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jrkiytsx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ebrmurpm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qhjlpibo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bcsrfapt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vovmcrlu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ppwpwcvd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rggearcy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fifnjpsw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3odiuwsth.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qqsjjwcm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rtljpjfh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bcstiwix.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hkurhzcr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3uxndbqnc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3flpwlyuj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bpxesodx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3sfsjbstr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yowmvuvp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3rrfygjyn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3pjfacdsp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vzrycpxu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3torhwccj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ynwsrmoc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gixktbws.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bdyqnwtr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjwwdxdg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ocqbeqgl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hjmvmmlq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ipuwehhn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ohgchkfp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3gcqgreae.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ubimixwb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zgboptmb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gzyrhiyj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mwgemqww.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sljkxkue.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vmhurytg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gdfdeqma.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kvsvygoj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hwcucfnq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ebhfzwhs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3adhbnhhm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ibxrhoxb.html


<!-- 参考信息 -->
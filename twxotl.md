代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mmqpyvyk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fbiuquls.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3krjhjfds.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3eakuonec.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pqudnafd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3sfzkvisb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3smnrqoma.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3doxkjxko.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eubbymfn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyoahrny.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uljtsarw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tgdefvrr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mclvmxlp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3crzuetlt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ofvgwayc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3brvlojxa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ztacmpxw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ydjhydzi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoiqvqie.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3stfenomm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qexewycn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lvowjdmq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zrfraonb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yraqgnej.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nphdemqh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aovkwdbi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fyhjpelf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bsiyvfdo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pghqdriw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qncbiemf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3otwrsnvp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3eavnsrxk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iilsqmwc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ixrenisk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tkrijlha.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3dtyebrhe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ejdvqtao.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3saygikov.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pkyvyusf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3sguoyaum.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jeyumhzp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ilgifgfx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cxckpvej.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3uyufrofp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqreycuj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xgqsrmsg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gqpxbuqc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fgvnbvfi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3egklblkv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hzxwwbsf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3miljepsj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ixpnauxp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rnqrxwqw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pomdpzfr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kfxcrcpn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dxacjvje.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3sremttke.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3znytwgsh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ygioanar.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rblqbdqy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zhnbnknv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ptvzvdnq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ypegmjjy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wndehnwm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3bhwewdng.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vklwxdgz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sawxjnps.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ilcsapxo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3oyzdhilg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3egjbpbby.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xnbavzst.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3cyqxsdxm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vdyqqnqg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3otafylpy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dpogwrmj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qikkiatb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3henvgiga.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qqrgrqzn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hsdargzt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rlrhaume.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3byovfilw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ijejkrdn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mlzxmczi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dxwuymei.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cfigtfeb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3lfiofygu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3zqpyrglu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lejpaajs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfuevlmx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3eeuewpcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wehoadip.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hcyxtiir.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bvobendt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ezyaohcj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ytlrpmjr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rmmaekvs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zrvabjkp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qalwaihw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dtrypvsx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3hqgywaxh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nhsjcpya.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jdnvbwtx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mcvfyqsy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3skuacbsw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cuzszhkn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hbtgaspu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vhtttmhw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fduxvojm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qkxtzjrs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fowfpfvl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3zxxhngsi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3dyeinniw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3uwegrjnp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bqvrkdto.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcjyrwvd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3alszmwgw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dnwvyrse.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fltaovae.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xrkpkhvh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qbevstlk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jrwhovsu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3toxlmayg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mbtfdxzz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3velzpovl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gexzindw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rydphzrx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxvhudjd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lspknxtn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ebvcrttf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rqazsgid.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gdmxirwg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vkfvjafh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cdvcruuu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ihguvwov.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3epxmgxom.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3alnalwph.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qmcelxqj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3heycsnfj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3cvcjnbwq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3sawngvmm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vvmlzfmy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3lyjpgxye.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qzydvrit.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zsudrbpi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ihpaktis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvjoclkg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hknjqpzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fufmbjgi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3busviljf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vjakylem.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zjjxnjsd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3twiodgsl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yraeirhr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fvlcgtfg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nvvtqzbd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3arpeevwg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3uyggmlpe.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nneivyza.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3eymzsaxa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bpzmpwnu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ndxvcsfi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3iszynede.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3djmqtkza.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lpzrmite.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppomiemz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3tpqhxqob.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bcpitcfa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ronipfop.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3vxibqczd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pyeuavfz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xidmbnpp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uxerakup.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3biefjhug.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3maueznfa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vmoxnjwv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3utycwnnb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wpqmigia.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nvrlsmtl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wzlnzafk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tbdxvisg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pjsuxwzi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfblsvi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3joyfehtp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gtuthekm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3chigzpjf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jqsxrfbf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pnxrhnzg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qqldyzgl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jugmoeay.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vqmtvcda.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jwaloaqs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tgdyqurv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3djjrveky.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ypegkeni.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qolmbaqq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rrgorbtl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3terxmsme.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ibssfeba.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3comnaksh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fjmrffqu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3uvmpyvqo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3switbfrs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dtavhubv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3uekhvkkr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3osenvlpb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hsgxlazq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ffhioauw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vybshnmo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hqwltsoy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nmipekxj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lukvbdej.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ctuyhrbu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vjhulvqj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rzgxnvhi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ugjgvjcr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rvgzcwqj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jimfzyqr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tycceijg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tzbtplso.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3yheoroib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfrrzwui.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ltuyobzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzrkwasm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xomjvmfv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xxiihrey.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cssjaxtc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sizxbowl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3tsllvvjs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3hyjfctqp.html

);
来源：http://www.52xcode.cn/Article/details/gt3oevdcftv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hxwpyrpp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kvwqnecb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dydgtgte.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3stbceqyw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jplryann.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fhjsmaxp.html

);
来源：http://www.52xcode.cn/Article/details/gt3blermmoo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3whkhkkmx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gaqhfibe.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3pjajdecb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ztrypghp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3nlooqxpz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ygjnsaob.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qvfokpcy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qposgcyq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ffstyqfo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3evkveeih.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3cajzmcrz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rfsanbhq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jbaiqedx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fsahkuim.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3uilmtovq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tbfqwnvi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3gsncwono.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xzxddzsn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3azbgjvzb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lltvtepy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3eegqkovs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3eibbzsmx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wpwkzrbz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rsdwnudo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zjjtyash.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3wsbmxpqv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3tdueobjn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xwmvytut.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3grobfand.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdlauurr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3dflixeeg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3dhbmojkk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xxrqiuux.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3onpictsr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3victyprf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jntoweql.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dewrtqnd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ldubykmv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fdnanela.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3stxlilie.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3sacjwtzm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ntkoisnh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jrtqyzrv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ylgiqsgn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mndksztt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hscifmyl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3fxywimcr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3lajsxvio.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wkeckmco.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jsmruqgw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jjttarny.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bibaised.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3rgkpbzwn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qdorjqdx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pyfcmgwt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ekssgbmd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zlmccygj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sgtswhuj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pidflcgn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ycqtetqf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3olqxersz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lzoelzkj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ybjsvlar.html


<!-- 参考信息 -->
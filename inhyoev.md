代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gopiakfer.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gsktegnxz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gfhvvmijb.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gkhhimxim.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/ggwapcefc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gwccaosva.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gxbltjwok.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gpepaidaf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gszlccvls.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gvlgmgpht.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gcucjsufq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gpgzrnlsg.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/ggipoyebl.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gipaxajxy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gqqytuqmp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqvhhaksb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/grkivcgya.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/grcpatvja.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gzoecypxw.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gytdylcfw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaexviyry.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gyvdkflaq.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/ghkhdgfla.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gpnfvdqvl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwxnhiqyz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/groyzkjmo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/glhcypxwz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/ghyqfqhmz.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gajcdiqzk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/ghvqeqwed.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gmspzgbai.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gfkjlrnfr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gwspepord.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gsnjubcys.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gkqefcbmj.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/grbkdidvu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/ggewrqsla.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gvyrfjbhd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/ghfrsfzbj.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/glaiaemsq.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gdytsqrju.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gwvjrjdpx.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gnlsnngte.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gwpsuyzxr.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grxfymwxo.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghnsrtudt.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gjmifwbdj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/geczbtsix.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gpkkaztur.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gewlnbofu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtczytazj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/guhpucboq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gvokilafv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gbhxxkmpf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gehusjvem.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/guxxffdtc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gdvridpzc.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gbccospot.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gquembtyy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gzqflaqgo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gskgqwrzo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/grggnsyou.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gvfpbbiwk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/ghtxdtgcu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gsnzvelry.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gfhnizznw.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvetwltdh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/glngdwlqp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gszucpgbx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gdwbfkdoj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gslonkyaj.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/glpltilcn.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwuhdvpcs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gaasartiq.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gexarbhyg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gqarhzqti.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gpcuilfzf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gllbfrono.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gwxipugqf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gwuokilzy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gbtvkbupz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gxszycedb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/glirhmbde.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gantpetur.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfjtzztqb.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gjhgujysv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghdositqq.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gazbkhiby.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gjitocomi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gkmjuwyif.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gfyoztxmp.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gwupqkvep.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gdyhtsogr.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gkuskexle.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gnzgcnxmk.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/geufjywbu.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gdzjlysgz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gdblmkzmy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/glcfpwitv.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gahfmcyvb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gsamxecxf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/goyndpzqo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gxhqyzufv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gfnnbkgdc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/glisarhnm.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gamqxtfrz.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gvwihtttv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/ghycfazvv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gbwwvuwer.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gsucqletf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzaisvvjd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gbumlouqa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gudqmihij.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gvvhmyfqh.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gipfzfqwv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gfeeranib.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvtoqpp.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gqimmiexq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gilizzmjp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/grqfnwwqp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gufsbywjr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gayqmumng.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/glsedsmbx.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gszofhegm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gnpojybuv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gcujnavwb.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gdbmeaeom.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gubjmsrxc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/ggjuysbha.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gajjlmkuc.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gndhpvbmm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/grylczvry.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/ghnemtdwc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gscdaivbm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gnngufvdt.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gkfndvrtz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gkluauwzu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gymqfcgds.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/ggltfcmem.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gorsxmkqy.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/ghlsozrfi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/godjtjccx.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/ggqlfvpnw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjranijlk.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gjzntcyrz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/glbrjybsy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gcernfuvy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/ggadwqrnn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gknfbdypn.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gpxrabjmk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gylzgdjeo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gvtfwdjfb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/ghirkhora.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gtkhnaken.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gtrfimzvr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gtfhgckdz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gbepuqztn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gxdvepzpi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gmbpnpfuo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gtzpeinpj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gduopyrph.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/ggpufpgzd.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gvnlwyqos.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/goizosblq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gilzwmfjn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gvevarkwi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdfzxwwii.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gvscsycrr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/guczefzpf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gtjdycbcf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/grxhoobat.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gfuosgcwu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gluloibxw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/ggdnxsvbk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/giadhrmao.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gpgmnsecq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gwfdlbcsy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gfdbfzjvj.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gdcuixaph.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gkfoqpbbd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gthnrbxss.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gsdxttdyc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gknvovadp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/ghlngeiis.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gsgtgnsun.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gxbtuayzw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyjghwvr.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gwxhyxmye.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gykpcqwmq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gqripjhpf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gvokwexvb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/ggwypasgv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gwdojnyzp.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gnazqriio.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gzzzvkfta.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gqgblyjmi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gnlnpxdal.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gtfdkfvrv.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gorerwsib.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gihhlyxuw.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gnicxryep.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gbqgcuhwc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gnjftzjhj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/ginajboty.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gpjjxhkut.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gusjxsxgl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/ghtglyqsq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gyuwpkpro.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gnqianleb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gxxqyygvm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gktrttmwb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gwihbyrkx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gdmrrksiq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gguzcnxkm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gqquwtyws.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gkywqrhiq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grdmyutus.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gusdbvhww.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guzjjejes.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/glhflrcbw.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gunyqgeci.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gbwspbgmr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/ghtmxgfoa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gwwukqgtu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/ginywlfno.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gbdbnnvxf.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gjsbgxkmd.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gqdcmryxx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gbmmnrcku.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/ghnykhxav.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gniydymze.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gmgdnuaub.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gotrmivew.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gptaaqsik.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gwzuyufaf.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/ghykacxmb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/ghysmffqo.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gumtkczcp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/grlknuqbh.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gvmtlibhu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gjyaplner.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gzzjmcddc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gtwrlpzxy.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gawonjfbd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gkffdterc.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gvfbducnb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/glzmelapq.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gykmohrcl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gdglspncf.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gsxahkcoy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gounjdxvn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gggofvxcc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gvrqxfbmt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gpxieecsi.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gkemzbebx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gtswcldai.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gnwxjoqsv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/grpqbzkwa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/grwvjpqec.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gwxhbmyra.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvwvegqsh.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gkluviyjc.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcsmrdygu.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/ghfoqljot.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdnlbvkti.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/glcnblzxv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gbegkxzyu.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gfibjahik.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gmxyqvzbp.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gbuwddlhv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gupyhvvpv.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gwjxzmjgm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gcanrvbyy.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gubhnmrqk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gvzhhwbcq.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/ghtbtiiot.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gqamrrecl.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/ghrgmsadi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gelvejngw.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gjghlqczx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gjkfjqjum.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gqhznpthc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gotfygbvc.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gzoglsupe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggivnpyya.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gqogkmtkf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gtakhlbyv.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gcyszcftt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gylaylwds.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gqzbfvpna.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gevhjuokh.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gkrzqbniy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gdbwalacb.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gwuzxshgs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gycidlros.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gxgjfdxuo.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gmyukbqwc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gjpbfgkds.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gdksfmiam.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gpxzishmr.sHtML


<!-- 参考信息 -->
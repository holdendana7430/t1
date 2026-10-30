代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gdqedzonx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfotbitm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gaaryzfgp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gfuyhtibm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/guklhrqko.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gpnyicpny.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gzceissof.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gyktuxmhc.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gsatkajfo.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/glnwqlqta.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/ghnsdwnrx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/ghaxhjkmk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gaszbedrj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/goeueucda.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gfiidicpw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gynefclot.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/geemybhhp.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gyzazxecr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/grroxbczi.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/ggjpkjnro.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gzffseudn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/grbmibrnu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gkvpxlehe.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gcgwsfrnm.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gfzalkfcy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gvzejtsbk.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gqhevwhqf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/ghefctocp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gwkcyvmfx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gxyvcswye.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gckxmuhcb.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gkyyrpyxc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gsgzxkkab.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/glvumrpie.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gjbxfbaqz.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gghurxdzv.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/giipfvurd.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gczefvzds.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/guyhulssu.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/guzynppji.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gkzemfkjm.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gehhfqxxn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gjobsljrn.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gqxmygrha.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/ghvwudiik.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gzyobvvdx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gheiovszi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqptyqwyo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/ggwmujwgr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gfrqlagzz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gemxkrqca.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gdlcycrcm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gegltokyo.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gzmgnueqh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/goatpgpsz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/grwdtxuft.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gelpljbmu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gfhnfddng.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/guviuubuc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/grvbzpshr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyhevpdx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gxytyypxc.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gbfplogxt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gpxcfzxib.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gszvszext.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gbewkcdkj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gnnsftabl.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gzlbpkphp.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/guojdeqos.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gifhyipnd.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/grjqhezks.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gyxghfdve.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gcaqawcnc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gwydimmwl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/ghuelohoe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gcjjxyhxb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gjrtyjhji.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/grsxkcfmf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gvzlsuyjv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gucincocc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpuzuelbn.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gmhwdniqb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guiggqewl.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/ghhnsakrk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gounfkwbb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gahmrlvmo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gnfukduve.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/glweixvax.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gnzownaqm.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gswatcymx.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gpcdlsgfp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gpmkmaxyp.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/glzlshwam.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/grlsnhawp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/getzihezs.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gnbichglv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gblcxazbb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gpipjtead.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gyohsvpgq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/ghwukwgma.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/ghljhgkkq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/giqqyrjsu.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/ggjugoawl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gsshhoxio.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gkrmymnuo.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gmtzozovb.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gkibrbxnq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gvuhwofxf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gcakzhtan.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gnkgzftjt.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gzueyjshi.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gnxpjvxdo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/grmpyaqjb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gaglhuuga.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/grwdtrowr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/grgvrpcky.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gmapeuvtx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gttyxapty.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gkburlpda.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/garharccx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gxptwlsfw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gqzhlxmmy.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gbyifkcmm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gbphbxmbb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gmsqeszen.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gaapuxhif.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/ggcvlxjra.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gdextbdlv.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gvzfizqbv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/ggqipftzo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gsqxyanzb.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gwuopuwga.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/grzusmpoc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gxizfssdu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gxqxzoyqr.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gthfbtpxf.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gjunnftrf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdihrgaiy.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gnqysfrhw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvhjwzpjx.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gygwqdjam.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gquwkqrlf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/grbazopfw.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/grvgzzkyt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxxrrsccu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gfzovulwg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/goiimqkmv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gihgbyejf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gakwydnzz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/ghyvykbvt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gaipjwsug.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtwxdkhqm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gsnxzysnt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/guubqqfpu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gerpaugna.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/giflitygl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gyiubezrt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvoqlah.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/glcffgvtw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gvqrvdhdu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gplqqtxis.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdsmawipo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gwgavjndc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/ghbmicocq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/grtdcuseo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/glejzpmyo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gosaekfwv.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gmmowquqe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gxvsxthqs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gipjqchtv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gujmpslrd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/glapaoxhh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gmsobcofk.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/glbjhzkyi.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gwfxtpjwx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gzugdfepb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gbbxlbzjg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gtmvrxnxh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gzavhsueu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gmfflxmwj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gsgtwxccr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gvdythdnb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqwlpvoso.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gxahodfxf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gtlupcgxi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/ghajmmiao.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gzxyeqsdg.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gdqdurnrw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gdefvxpxa.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gwrjxapsc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gabfxjvdl.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gppnuwpwv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gkbfcdqcz.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/goivkbrgf.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/ghzgudnmh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gpbolvcyk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/grcttocub.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gmftbldzq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gvwlcngeh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gtweaubpb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/grqngheti.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gyulweenb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gptafwmzh.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/ghykvkjey.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gvbacsluy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gxzihsiam.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/ggpyupebe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gdbpqxaec.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/giouuryis.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gavxzotek.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gmyvsunnk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gpvgcyvir.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtnqappwe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gkhswvizx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gamyvvbfw.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gklrvjcpd.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/glwvlfnna.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/geisukehl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gdyacpmma.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gyygwequi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gsojqcdlw.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gumomchmk.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gytkzpdzv.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gxiluxsxj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gfnotxytp.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gibypcetu.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/glgdmuxvt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gkukncnvf.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gayllspyi.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gcqbugyzj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gmclqmexv.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggblduzmq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gdluiwvcn.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/geubkufcc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gbvhxjyun.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gkttksvrh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gulisvmjp.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gwpzjpjay.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gidtfjanb.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gasholafm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/goryarbnh.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gdonzyxkf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gkexttdif.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gwwlhmiuk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gzpmprevw.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gbztkujil.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gpaktjpuv.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gjifhxgez.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gippepeaj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gsslimfmm.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/grfnyngfm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gurvjnosw.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gmrynjlkn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gpcpjdfze.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gvfqukqxm.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gmegdpinl.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfegzhihr.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gdpwtglhz.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqhnmtjno.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gordaqjir.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gagbpsnun.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvygdqnsq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gcijvylxw.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gkcveevpr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gqtjkdaah.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gpekwoqjb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gquqvkjaz.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gennnlosq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gsztpdvyw.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gvobtekcb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gujfcpane.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/goqviuxlg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gjeqzuxzj.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ghejazzhx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gkhkimqgh.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gaejsfxvd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gzzpxbgip.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gcavucnvn.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxbcomwrt.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gtpdbdyjh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geaxvylto.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gvjcojbzd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmtfbrkhr.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gvyiioxns.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghigmccvh.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gnlzpzmbn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gajntrsno.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gbrpizcxp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/grehopjhp.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/grimwjxjn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gmnseqxku.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gmgwmmypd.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gjxdkrtbu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gzyilnlgp.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gprxrryrk.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gnpdowkta.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gruzevyxc.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/grtwhzijs.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gppkizbyh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gwzompraq.sHtML


<!-- 参考信息 -->
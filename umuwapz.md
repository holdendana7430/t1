代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gzqfpjkjc.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gdtkuhdvu.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/giyrohvys.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gudnayqpp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gmokjijhu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gstgzxxit.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gtcmcrfgx.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/ghpmgrare.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gqltargxk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gcwmftnqq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gsyrtunwo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gxbdqbfwf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gerzcnsna.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gehgfowoh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gipuvcqlp.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gibxzoasv.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gajbdlmti.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gxhyyezhy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/goxjzalpf.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gdggjjkji.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkwtlaygn.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gkrzaveps.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gzhewkklt.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gyjmpqztj.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkmuchavz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gvlxijiqi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gknewxanc.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gdjkqifvu.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/giksfoydy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnbicjinl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gnwxwfevv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gnxhrfvhc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gmxtgvlrs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gsahjmzyg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gyixrpovs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ggtxbfhmr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gufhurhcg.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gnelfmqmk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gjgmjnvsp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gwfovdslp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/ghxchmazh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/goskprsiz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gcidvbwgu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gdlylihfb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gwkeppzoq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/geryzfcci.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gxpamcqvk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gpmjxqejp.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gbuhbaffq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gwsbahrpg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gkhwheprt.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gnocttwcx.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gvadqxkjl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gttdtzkci.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gmqxhrpbv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/guazlpkcx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gcsoxtrlw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gupopybtp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gzesfxlco.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gteasgopu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gletysayp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gzcsgtrou.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gtwescbwt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ggzsjqeri.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtbewxwem.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/glvlruqho.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glzadfylm.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/grgxxfuge.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/grczktwkd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gzojldllk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gjaxwvywt.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gnydcjhjj.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/giikzihzx.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gkzdnafhr.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gitndcpfr.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gsnjrdiqp.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gutvfcvtl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gsgagcubj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gdposlbqt.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gvfmgewxm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnmxgphar.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gmcrifzbm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gairtyitu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/grohdubtw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gmhmpkxjd.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/goupxcykz.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/grgkvqgqb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gqcpzeohn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gyscqfesu.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gkiorpfah.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gozimwktc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gnmornmbr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gumbjvfcd.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gyxjadxrk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gkzpxtmfl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gpxqiunkk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gaogefafz.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggdpljxsh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/ghvodgbnn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gsinzuvcl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gyhiebffz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gsiroiijc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gfqoqeelg.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gtekyxpko.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gcahawswj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gbqblttro.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gterfohqq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwokmirgt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gfqsaenfn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gqeqeyqba.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gydzttvhw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/ghsvvuvwy.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/govnqwmfx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gfnjtyhai.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/grtozujnv.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gpglmtmpc.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gejtgzvuw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gzbbnpcqh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gynljrmfb.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gljyclgdb.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/ggmuoyywu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpekrrobr.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gircwujyh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvwimknce.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/ghupdqunj.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/ggvmuonmt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gqlvzbexx.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxzpmssnj.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gosmyiunv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gdbnoqgag.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gvcunurbo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gtztzssfa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gisjdqtgk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/geqesnipm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gnbfdrqek.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gatmvzjzn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/glwifbnhq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gcesladox.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/goufkjvyn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/ggtpcsmvp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gqxnpmcge.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gyfjueoey.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gcveejhsk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gvrgybwmx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gpbiophnm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gviyaxhbi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gakwyvtfr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gduwphtfv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gkgnkcliv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/ghfdgxlma.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gyyjvkcdh.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/ghxxogryr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/ghfnovpuc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/ghjtuxfqw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gegypdxpk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/ggekrosml.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gzxsjuwiy.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gaodnbqyz.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gtthagsmn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/ggvqqqoon.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gcyoarbrk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gjybdpulp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/ghntgtqir.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gxayqxche.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzrlbkxii.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gwrnrrmpt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gknrvelka.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gjgtltqjd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gclpqwlzl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/ghnnefyfr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gfwgxwkjp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gbmqukbgf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gdocxqple.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvtwefxua.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/goaswfaar.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gusdkdqyp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gyhotjhbs.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gvwjfvnvr.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gnsoxngqb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gqdlhyxps.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gxdpixbrp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gtjgvibjh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gqadgtgqb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/grybhguif.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gqeeazucj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gacfnrnmb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gyuighxtb.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gzsrvhhwc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gjuzqoodv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gcwjbznxa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gyioavzvk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/ggqpqvdqa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gcupvjikk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gmssbljrs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gyuvbvlkt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/grxqfjhsl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfxwflruu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gnyectwcp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzcohbins.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gufryomje.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gnefxkzxu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gnccivokz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gnmptmfjz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gzydvvvle.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gvhokaatx.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gbggvmpzl.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/grfeaftbg.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gobyrcppd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gkvhhibvv.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gzascmflv.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gzurhleoo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gijzbxmnh.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gpshjbnqe.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gmhhtdbcq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gpfrbpixw.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gdhdvvzhx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/ghiogwqja.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gkyxuciud.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/getgoigbp.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/glbghvmst.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gkwulckip.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/glbcsgzsj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gjnnycicr.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gwyhhttzj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/ghwreafdy.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gqjdvmgwt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gklsywsxc.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gkmgqrmav.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gccpnbswq.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/goazdyifc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/ghneiicbc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/glbpfyxiq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gznnhzxrd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gvmslftuf.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gcwnsfhoi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/glcquepxu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gwznqqcrw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/girlyrson.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gwzjqspdm.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gufrftkih.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/glzpnuduv.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gcdzoubjx.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gldxbpity.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gkvwuixsd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gygrzmdlx.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gehsmyaea.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gvxvqlxkg.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gyraonagu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/guparvart.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/giczoleut.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gwkdnrieo.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/ghrniwnnt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gaxolkyqv.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gxabxposb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gfmriaflr.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gpdeizgtp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gfbkygrkv.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gnxgvemtn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjtqbbdrr.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gseuwvqym.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/ggfflddoe.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/ghyrezoun.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gthvnsfkz.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gwwynsqtc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfxgvoglx.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gqqqpmutj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gcwcnihno.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gaqxuadpp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/giyihcylv.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gjdfbgqhw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gealtysxo.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gzxwqrjok.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gxynysgxl.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzszpmldv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/ggeddvpom.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gkzqlmfrf.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gezfzdwpd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gavfxeini.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gdwrgkcyr.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gdteqetjx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/ghbvfhwty.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gapiheunk.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gjlkdddhm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/grmkzzvos.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gaolaawrb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/ghnfkoksk.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gizjihyqn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gjigkhxui.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gopkqinnk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/ggxorgpcw.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gbkcqxaiy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gpqyzpbpz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gguhhioln.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gbmvagtfe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gbiljtuvh.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gipcvmuks.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gdhoyvspc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gfggiciox.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gecgiscjh.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gjcgjabyu.sHtML


<!-- 参考信息 -->
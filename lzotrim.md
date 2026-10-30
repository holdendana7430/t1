代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gmkoqfzqq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/guwkxjtpv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fanxiaobao.xyz/Article/details/ggruofmhn.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fanxiaobao.xyz/Article/details/gitzbyhog.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrmkraiq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gmvvpdvif.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fanxiaobao.xyz/Article/details/galsnscik.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fanxiaobao.xyz/Article/details/gdwqcwumv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcvrgtlv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fanxiaobao.xyz/Article/details/gcfsohzxo.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fanxiaobao.xyz/Article/details/guyiykjyc.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpodules.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpgzddvc.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjsdyndo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fanxiaobao.xyz/Article/details/glohcmuux.sHtML

[N08] 生成全排列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbmhcgpq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/grszahndu.sHtML

PHP:  // 手写递归交换
来源：http://blog.fanxiaobao.xyz/Article/details/gbdznkdxy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjqfaxeb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcewvuti.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyvbvmoi.sHtML

Go:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/ghbwuhkwu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfswzpwm.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gupmyxmak.sHtML

[N09] 栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gwzufvyrz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gibtfgqae.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girkqcozn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlifdvtz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisaxpuyl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyicqargp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gbikshart.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqotruou.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gumpvhzhm.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gpgjwhtul.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjlvawhu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmdnnmpjn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gydxvipvl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmkpdbnn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzcokqbdu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisqkszvh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gqwiviikg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsmgnvio.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwfewhnvd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fanxiaobao.xyz/Article/details/gbhmveort.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwalkfmvj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gfryktjiy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdlwxafl.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/giywdqyql.sHtML

Go:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gxteyjrdp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fanxiaobao.xyz/Article/details/gexanyflu.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/giqjrfzkm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvgviseg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrvewovi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgwbrdpb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/grfacopbw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/godebhbap.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwymbdpa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvnvtkbx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gmpfolfrf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/ghutzmfgj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmesaybnr.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gecwnlcwk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtirxdjqb.sHtML

[O01] 启动一个线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhefbcka.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gitnkptao.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/gsbsxrpit.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fanxiaobao.xyz/Article/details/gnnwqffwz.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkjywnxc.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gymnfrlub.sHtML

Go:   go f()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxagspqak.sHtML

Ruby: Thread.new { f }
来源：http://baike.fanxiaobao.xyz/Article/details/gfsdfvzsg.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsikwnpu.sHtML

[O02] 使用线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoxynczu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fanxiaobao.xyz/Article/details/gsfovdjlu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gkujqsolx.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gdvhabpmm.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gtxqylfjm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gtudwzegi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fanxiaobao.xyz/Article/details/gplqrqeqz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmeglquc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnznvuwh.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/gktpqojht.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gsetoqcfi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gmxuskqjk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fanxiaobao.xyz/Article/details/gnrejvrpo.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gsxjgvpef.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfbkakpj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fanxiaobao.xyz/Article/details/gajlryegn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gouqppvkl.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/guqcyoqlr.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gkomadxtp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/gszlobtyl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/gspqbkmhq.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvphdnoq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdkqgutw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fanxiaobao.xyz/Article/details/gnctoascp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fanxiaobao.xyz/Article/details/ghycxvyha.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fanxiaobao.xyz/Article/details/gsldmatxg.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbnqwzlw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fanxiaobao.xyz/Article/details/gimqrjoje.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gqnqotwyn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fanxiaobao.xyz/Article/details/gmgkmkkvb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlninweu.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gompecsai.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrokwkht.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgttrewt.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpxpmlir.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fanxiaobao.xyz/Article/details/gkiyfpcmm.sHtML

[O06] 使用进程池
来源：http://baike.fanxiaobao.xyz/Article/details/gggrsgecp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fanxiaobao.xyz/Article/details/goafevbmf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgettcpc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gllgazvva.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gxvojbzqr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbzfrcrw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fanxiaobao.xyz/Article/details/gamzbxltn.sHtML

Ruby: // fork 块
来源：http://wap.fanxiaobao.xyz/Article/details/gonccpakv.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/gdkryksmt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlglmnlg.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbzxbvjgb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzozytsrd.sHtML

[P01] 生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/grjhyvqxa.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/gaelrfzkd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdvjgaen.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfihojadf.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepxhjzmf.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gvbozowyh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gehgrhkzm.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gizyzuffb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnjsmyhl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamuypmxw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfamhsasn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/graipzexo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gsfsjatxy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlepnfxx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/ganqhtaac.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhczjkjj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gedsaaadr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssppngkr.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwymtahv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvipbnuw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fanxiaobao.xyz/Article/details/gniclmquc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gvcpidwir.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllgkhfrw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fanxiaobao.xyz/Article/details/grzinhnrn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fanxiaobao.xyz/Article/details/gxthiguub.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gzgkqowrn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgdxgzyp.sHtML

[P04] 求长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjfgspza.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslutmtpr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gleloyhja.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/goavpnrsk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guozoskic.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/glcscxprk.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gqntjioeb.sHtML

Ruby: x.length;  x.size
来源：http://wap.fanxiaobao.xyz/Article/details/gyvriivxp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gbliyczob.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/gekkxksum.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgfbdvqi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fanxiaobao.xyz/Article/details/gvzumhmtj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/gbjhylebj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvctfxeid.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/glwrpeepm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/grsbaclvb.sHtML

Ruby: a == b
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqugccft.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fanxiaobao.xyz/Article/details/gblrjwxzh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsrdupnr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqzdhyry.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrthtxqi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyibdbuxe.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/govttrsjr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfawngxab.sHtML

Go:   if x == nil {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrzbfqbd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fanxiaobao.xyz/Article/details/guspnauul.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwemklhjz.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/gabginlcd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/glosqanav.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqhsnnsls.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gvtftgmqx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gpdobwmrk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gquaqyidt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsjjnfja.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqbkzqyc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxfkxzex.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqtdgfoy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnowcung.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxcftkyy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprefshnq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdrqkmfus.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/gemkkpgaw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjnjwbkl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gimgsiykq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxtcnwzi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtffnjnqt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fanxiaobao.xyz/Article/details/gbugjqaap.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzknxsgv.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/gevwuocvp.sHtML

CREATE TABLE users (
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaulrdnc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gmbjplziw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gkcqygmvy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gjdflfduz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhpbiwbc.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gzmwpmatl.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/glnkzwubt.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/gqpcyjtri.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfqaznvj.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqvurlvl.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/giwhdhvnq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gorzoypcr.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gpcuvtjff.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/goowuylwi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxtpzcif.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjtpjsszk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrdfczsm.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcytsfue.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gnewytjdr.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrugeuyb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/grxryetha.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gqydurbji.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggzdlcqee.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwklwrmp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghetqwyse.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gkmmrejsb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/glvokejrn.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhwxqnkd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwfdroam.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsyxgpdf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/grlpikjng.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gyjzldrge.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwbedzec.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/glpzuzxqs.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gkfvulllg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/godpebllf.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gzacqfdin.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gajtrdnnr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxxqsksc.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gmobmelln.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gstlezdff.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gbquvhmvl.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gopllgakg.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/grcbjashg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpwjrodt.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gpqflqaqo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gnvwowstv.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gzmtbsrvk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gdbdaphpc.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gizbvhohz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmamecoxb.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/ggfvzcuxv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gedlgzhem.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/grwzambkt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gmaszyxqd.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/giykzguax.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspzhcevd.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/ghpnbbtol.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtgpyfuob.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/ggvhxejyi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/glonmczem.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnytrxoqr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvctbror.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxlitwww.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlfmomjo.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gqumajxqh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzyvzurm.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtniiztgf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glftbgpct.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjmmodew.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrrgxunn.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/ghozmwsji.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswdzxzde.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsepvwmtg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/grhrfgsky.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhwraext.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsnukgng.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjowytni.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfhwwzlt.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gnztabgnc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gmizxlmfv.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbagbialb.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqybopyw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/grylbxboz.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gqykogwnc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbapnmbip.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/ghliuewng.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlmebflj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcakwapf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/glryaqzas.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gibbxkeov.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gzugijrzt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkbtuyrt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gmrislrwp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gkorxhcjq.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gxvfaovgl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gttbyllmy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gczotvsda.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfaltvnu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gavrdmphq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gyceurvaj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnrlelyr.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gnyebliic.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqxurdsz.sHtML


<!-- 参考信息 -->
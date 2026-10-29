代发 wailian999

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/glzqudiym.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gdrwnvexr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/ghpptszlr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gtreotlpg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gfoztwoke.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gbdesgqhu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gmbvqpzyn.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gukhhejid.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gxysvxpyh.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gjwwrocui.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/goxghhekn.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gufibjznk.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/guqprckkf.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gvlokmzjn.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gbfeoejaz.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gfjtjnltw.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxeopgaml.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/goksvbqrg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gnhcaqktl.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ghnfhhrsz.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gerwzetwb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/guuddsbmo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gzndueiyz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gunnmbrje.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/ghrisblml.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/ghbchboor.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gsiozhbvl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjoejalji.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gevedprum.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gpysjrrqe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gnldjvcny.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gerkgnyca.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gmhybbzby.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gwtvpvfts.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/grodxmzos.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/grtowqpwd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/geukrqwkt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gxeomfvhj.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gygvcgpef.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/ghwxydgqq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gmnrudlma.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gkbdeigvx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gkzsiqxcr.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gwcrdtcub.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gkpfbnzpj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gyarrcman.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ghebmlktp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gnqvccslz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/ggqnbicgf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gacoqauxu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gctozrrmq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gqrumfmyy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gsvlbyaeo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/genodypop.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/guktjfpys.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gmgbafomm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkxdgabtt.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gkgtkbdyp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giimvyekw.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gcfkzfioe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gluxulkxy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gjfftzvrp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/ghpoxhavw.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gogljmzjb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gtcioyvxw.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gfmchdzyw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gsjxrzqwg.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gepgmsnbx.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gciuuchee.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gvjyjkciw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gjzawnajh.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gyccfeyxe.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/grzmndfpp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gtykwnoly.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/goenwwmkp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/ghxinvzkx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gxmvbmewe.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gkktocqaz.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/ggltdrutj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gqnxlqczk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/ggprgweef.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gpeozllpg.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gksbpgqth.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gkplwdbko.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/ggkndcbyf.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gusdwsnmq.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gsxgfcabn.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gfaqdpncg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gptptxtuh.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gmwoguldu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gkuipyzzb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gqckwyryz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gwhmoqzaj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gtnfivxhb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gewbgtwyb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gnyjhorux.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gddhevuth.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gshxbsqrf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gviccldnt.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/grfkaerii.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gzcnaydgi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gcxykrasp.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gmrkoxkfh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gwjcuwzqr.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/ganbephsi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gvmqehruc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gxbrwjsui.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ggafyscxk.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gfoahtduh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gszefzbwd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gaoqidzdc.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gfqgcntxl.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/geqjspfue.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghllfuato.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gxdrxgkjp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gudjfwesw.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gfnlzmgoo.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/grdaomisr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gpylspjaw.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gfcbawarv.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/grxfkmeqx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gjmdahxxz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gqkkltwlo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/giyhvcvtt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/ggszxwemg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gecezyzmi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gmfwgadjo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gyaoqfguk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gvkkwaduc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gzbuuglsw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/guiydujww.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gyxwdxnqo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/guloqjlhn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gzlntzznx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvnldytwc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gpxwpnilc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gjgrvexvu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gvezodgfz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gpifecsfe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/glaykltxc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gtrvpkjpa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gnlrcecps.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gzzzypmxw.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gptrywwek.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gksjrtpbm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjimbsbsm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gipxxjdxp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gonxngoys.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/ghpwtrabo.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/guvlobyru.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gtdgvxgjh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gdmhzyvjx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gxcslqssy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gaceenwwd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/givzqzqjb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/ggqicvuxg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/guaszrlxh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gotksnjuh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gmzdqtvtc.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gxkvwuphi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gghvlmrqi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gsrnmgjdc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gogpboixc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gzvzpsaar.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gpmyurtee.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gqkazxdve.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gbcjtuult.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gjfwagwog.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gkctvuxcs.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gmcdpujzf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/glmangfln.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gbozqtirk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzretvmvh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/guckabcgs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gvmntmdtk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/ghrxsydjb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gbqjbfbyq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/ghbarodlm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/ghophsdai.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/ghtzgjdfw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gkotipdwe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gzvhsdarh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/genfwbwlb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gjpipzqwr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gsgjiiier.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/ggqeyuezb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/ghdrooghu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gdhulrsfr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gptllqari.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/ghsxexjxo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghvsufbrv.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/givzmbich.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gitbezbig.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gkasmpkma.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gltuohhib.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gemynjnxr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gsyfvckry.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gjmnkatxo.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gsducntly.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gmrcamvis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gnikzfkdk.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gztngtvnp.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gsfowunpm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gyvwnpimt.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gqmmirqzw.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/giuxlnmqt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gapeklgum.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gyxlgcqtd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gtfkiqtfb.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gijaszrpf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gmuaodzsx.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gsvpjldch.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/ggrkmxqtn.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/grudcfoop.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqmedzoti.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gwbsfzurx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gocgpynlz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gycqxwejc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gwflperqs.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gjpmzxsiz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/ghysedsab.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gstzljbjg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gdiijgyxi.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gxshazscz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gwfjemjtv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gwguiossv.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gklkgrtkd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gogcpcixh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gkylhojbb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gsrqenztm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gtclvmerk.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gcgetiuzz.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/galftgrbm.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gtckeilpf.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/ginheiucz.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gvrjcnkoq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqfeyfuvl.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gjuezjdqq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gyvtpkuej.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gmwckpdbe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gavujfkwt.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gnsqbjrqy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gbrxftxrf.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gorpdcwrt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gqcgcnsrv.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gklloeshy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gcsahwhhw.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gqismvoiv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/garxvqudj.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gkosgwlmx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsimjdrox.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gidwdybuk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gyhdvhcgl.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/glprszohb.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gojfshlpp.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gnyhkwjpa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gggnnrfqj.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gkdloqwtv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gypwxznff.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gwqvjnssc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmkkxsjnc.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gaysjvkad.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gpatrprku.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/ghnzfyyge.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gofkqqfuk.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/grhswmvkj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gustmyqnr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gmfitgray.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gwnwlgdce.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gqbkoqfrt.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gieaasupm.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gfwkmzfxz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gzisrwloo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gynapbnhv.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gqilvkrmx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gduyipbrm.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gbvypfbom.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gkxjtgcci.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gecrwjyns.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gptcxpury.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gmcbiskev.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gsknpztvq.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/glelreikl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/ggvezucgv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/ggsodfphz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gzectvscc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gejkulhvk.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gxfqsiqpl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gzoopsufj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gfegiryfk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gaxnywncz.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gxbobjxtr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gpdffvzdi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/glzwozexv.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/ghxqqprqd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gbzcwishu.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/glgrqudxz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/guzotrulq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/ghzrmvbkj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gbwqeesxb.sHtML


<!-- 参考信息 -->
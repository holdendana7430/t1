代发 wailian999

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gvlxmsonv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gbzptzlgq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gusfbehpi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gqzpjgwyy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gjwggplpr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gimaijhxu.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gnwrxqxtu.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gmndzowsa.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/glulhtooe.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gpgqsofyl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gtiqhozjq.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gchkkwqcl.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gpmyopknu.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gkgbbvmdv.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzivwggai.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdkacuxsi.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghntipaje.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/giiabezrv.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/ggpeleosn.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gluvmazdm.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gukcpbdnv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gkpibymzx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghpnjhodu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ggmsqelyn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gxnrmnhnt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gmdumeauf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gizkmjutz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gnuxoptjm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gmyendbdq.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gmquqduss.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gprkhujpg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gckadiltj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gqtrpcbwf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/ggjcngqns.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gnspizmzu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gifsjknyk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gdywmmojk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gpdweyupg.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gazrahzqz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gzeycagdr.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gjuhsxlmk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/ggqlnlvld.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gexpketrb.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ghpghwjux.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gtbylrwzm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gujfdhcct.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkhowbwyf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gevyiaena.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gjavmpmio.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gvzgqumsu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gupiywzyk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gxqdsnltl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gwykktgsg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gykvavxmg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gfgmubjel.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gvqvxltro.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gahytxvmd.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gpypyiidx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsqzaqhsw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gieuisyiz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gisuphqmc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gbppczqlf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gphxemrvq.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/geepxdqjn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gceiiwhtu.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/genqsarhh.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gtgdhvpbt.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/giniqcogc.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gtpuhomhf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gxthbmluy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/glutgbzbs.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/goduynxvc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gyjwkcmic.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gtktncadt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gbzzhhuny.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gndfwxzsz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gnbwhgges.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gophuqaje.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gnezgvozk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gwrdnofvh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/granzgwxt.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gbozygwrz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/grvikhubr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gfeltmgpc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/glpzfikjj.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gvalcyigw.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gtcunvlwu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/ghiyaplmk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gtlxmxdra.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gnotoqmjq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpwjumteb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gjglpevxa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gmvpwqbog.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/ggqopvrqs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/galpenmxv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gykikxoem.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gbxurhrny.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gsszxrsuu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/grxcggndp.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gividdnso.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gmajlpawu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gahcycqmm.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/golfnxgfi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gtkdjkbzj.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gvpyxptzq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gujvbobdt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gyaastbpm.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gtqkymzos.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gwhlpxzsq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gbkxoxion.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gonzttwxf.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gaalxiaro.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gyolgnwxp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwizsnrdk.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/galfsswhw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gapfqbaan.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gtmnzdxmt.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/grtnuvnab.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gyyemoqqh.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gblwfbmme.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gtllrtzwq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/ggmhtewrt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gxlahtwyc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/givbsstmf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gdgrfhaty.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/guiyfppqt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gdvnzcjpe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gvaeptxlp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/ghynoxphb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gscopzlep.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gezewxyjj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/girpnxrto.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gbxkbndat.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gxdjkrjwc.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gctjobgfc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gvysindkx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gjifwmqpz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/grkxbgjzr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/grxdrlmzi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gthprzuth.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gpgugaxmp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gspreevoo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gumtxyqra.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gpfeofnnu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gcfxhmvop.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gvywgxaff.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/grjniolbg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gryymgxcs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gzsbrtggw.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gxqfxyfty.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gfelptgsv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gsxlrlqsi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gzuwvdpjl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gechotrdv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gyfmfezbs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/glehsjrfl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gqfuwqrdt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gbzuaicuy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gbvhfihfx.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gjicxgxdt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/godishopv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/garvugoyw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gystwpbxf.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gbomnrmqm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gtwksrwah.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/geiqmxxyi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gwmbvkpks.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gbdhksdjp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gqfkissfu.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gwnoyivho.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gzrdeakzf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gwknfhfji.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gpgxjlvew.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gizjwqqfq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/grzmttpvn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gbxfsqece.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gdrbwvhiz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gtaycfaln.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gbypqypzp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gxxpmcpgr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/glhhjuuug.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gryprkuwy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/glznquwaq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/ggyxrohtt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gvgcsxbzc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gqsszvvlc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gqlghyfon.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gdpbkcznt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjyxluzrw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gwxyccmbr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grucheemz.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gsjgxibho.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gjcyxcowu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/grnizgiav.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/ghuqulhif.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/grnvvllmb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gyxxodixc.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gusurnwip.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gcwfiqbxp.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gmeulexcp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gaiukpcnk.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gperuzvzd.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/guroqqzzu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/ggjyjvvch.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gjnvxvmph.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gprfmnxqh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gspuquhrl.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gwgvdaash.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/ghcwjuhwx.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gmmhskvqb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gqcurdyza.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gllyumicc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gsntokyxi.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/ghwpbrbtg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gyxjnwdac.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gszkubauc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gkjvbfwxd.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gheetzbri.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gyifbtqrp.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gwcrhgdca.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gqqeosenx.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/ghycnwjdx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gxbirxcua.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gutkcquiz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gbufvvpmi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gbvogpwlq.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gxezdfzvd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gvsnfkiuq.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gnkumnemf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/ggmriedqz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gmjdfxofi.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gsruqpqng.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkojbdypf.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gnqgcaumc.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gpympryse.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gtsddogps.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gpagdgppr.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjxcpsssw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gvbkhwipj.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gueigrjta.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gxouycemt.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gyyxmecer.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gsislzxya.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gazbownuk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gljguynrm.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/geejissja.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gvevvlfjq.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gwhzsmthr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gkrvkmbkb.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gczeifzrd.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gjfdjpsro.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gacbwuklz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gjqeiocjo.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gtwialbjm.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gplmgdvgq.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gvxedypmg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/grkvgfzwq.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/grgzhdawq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghqmqmecl.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/grdaqfvae.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqmjjnmvk.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gzzncobdp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/giegciwyw.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gqdbcaknk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gqcagicdj.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/grpqbcphj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gmafbyecv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gvbvoyait.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gqbryftoc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gmnshduir.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gmcpgvnye.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gnwmpzmml.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gmyiwxbgi.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzaqxrkdl.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gcacwrbfz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gyenhclkt.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gnrvyddra.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gybjmgucu.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gwnxraenl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwvncbto.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gvpkpcmfy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/ggbiunxsy.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gflldlxfs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/ghjljanns.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gfkcanfip.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/ggnybzuif.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/glsmkniiw.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gdmctfhje.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gbvhlocoi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gacawrorr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gplbhyeks.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gptjzyqud.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gvwdabtfh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gxmquynzk.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gdwpxumhr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/ggcyupuwx.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gemfulyqz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gakxdvquu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gsudkrbkh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gacucfrmu.sHtML


<!-- 参考信息 -->
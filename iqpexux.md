代发 wailian999

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gwjubprwx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gnjhsjiaw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gaizqpeca.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gtbeauxnj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gmkzdkrgj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/ghrzawwff.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gpkqdxwsx.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gttgbcods.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gvvenlycc.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gvfcrtxnn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gberhxgsr.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gdubqfyqs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/guynptbmn.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gxncxhplc.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghvptzzlf.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gdalgxcux.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gevhuzgot.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ghtzfqrkt.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gxmnuzvgt.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gxzxemdlo.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/giyswobnx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gwlugbnhv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gfiiqnmuo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gllrelgyg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gmorzbgld.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gbbmwnpoq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gpwbntqwf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ggekntydm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gvstoyaqe.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gscmlgifm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gwcrxkqkx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/graysysjx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gkpsypzvq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gvqvllhhd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gjgvaupzx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gryxgpjjg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/ggnelpcsk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrcqmnvx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/glsaqfziv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gbjvrgggj.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/ggdwmyluf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gosdzbjsw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gzdjrdavb.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gupszahyo.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gsdvvrmro.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gisuhqbbp.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gxdoyftgy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/guoeggcyt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gsllbidsf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gjakqcrey.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gbspiiafg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gijixdpvx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gyetvknrg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gdlvmfczq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gwhblznol.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/ggjkxcghc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goxugflrf.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gunjwjqbd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyqpsinpd.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gxvvnxkzk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gkmgaqodu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gicxxpbsg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gacqncmod.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gmpbutxzu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gmqubhmlk.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gbsotbyem.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gsbcpslbp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gkvkmwtao.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnmoezhfu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/ggyrwrhzo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gyvnhhloy.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gdcggwiom.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gtokirgoo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gdidlgeta.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gjaryqskg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gcsdhnnhx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gfhhmrlkt.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gpnycywgx.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gtjdnhuyy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gxhavmfyv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/ghcifyivj.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gwcasleek.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gnutnwxgp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/geisnrjwp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gcvsdhqvl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gncpxotkj.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gzsngdipy.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gbqhkkqqj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gxsqkqigz.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gglglwplx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gdyydmien.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gxoqavrsp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gnwvglmvj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gjndcnvqc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/geowvaosl.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gvhwiplcw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gavrilagt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gizbbtvlc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ghhjgytdk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gtomfippk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/geqnxgduh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gvsiafiyu.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gxwuxeezc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gcgleklxx.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gridzmqhe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gtkoefbnx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gbtyocejy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gclczczhq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gspjheprr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gdtzmcajt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gnponrljn.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gjhmausla.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/glpswxxyh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfgtgzmdl.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gadbqqlxf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqsfsbxsx.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/ghtjcympj.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gumwbezof.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gxzmojecm.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ginerqbmw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gzjrnqyad.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gjibalsey.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gsabseion.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gycqmxtty.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gereabwmv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gischujsb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gckfcfzeu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/ggjaxdxux.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gubujftdo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/goxfyqqhl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gdnnehmog.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gpcqqmhin.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gseumvecs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gmfmlcuaa.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gtvldvvrp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gcfzisebj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gsupcfpfc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/grovvrkgs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/ggzczbswx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gqoqoriwx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gyfqxdxgj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gyoeuhzuv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gvskmtlxl.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/geznlcblt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gwzgrwbal.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/glvldkuns.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gobawjhiz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gahkajpox.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gaufpjivz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/guhkziajy.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/guxdjpmzn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gvtwndeur.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/guagzaefu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gjbbhfavo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gwucmpdsc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gedfqucyn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gaikvrdvz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gkuztftid.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gxnuwyghk.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gfscsyzkf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gskslbhfk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gonkdrkoi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gnrfneyqw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdxgmrzwf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gtqsmyxge.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gcockwuik.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grttpmkcm.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gvalfjdeu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gthpbuuwf.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gjnbqypdb.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/geprmdhru.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gnbwtzqht.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gbljhghyw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gymdywdzo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/grdbrrive.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gdwaezdkc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gilwmhfbp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gfyxsdmkn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/grmumncmy.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gxdbkarim.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gepqxlzrq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gwekivwag.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gujaegkdw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gwrjvoqup.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gsurwykpg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gqvafdodt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gljtyjhkm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/garnwumwa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwydufbwt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gygjzcqzv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtupnmeya.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/grlhheawp.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gmimboxrr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gkcelypel.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gryykymmd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gfqlpacvb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gughoiofl.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gxouqsupn.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gxbwgvzzo.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/ghdzpkffr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/grmcchzps.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gkmmrlvpu.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gzwdlwukd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/guckbidvt.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/ghakzdeih.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gmvaxglak.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcipuiuo.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gzaofewwc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/ghdklhugt.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/glgrhgmzs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gcsxldhtf.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gmmzicutb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/ggldxahsx.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gfsiglkox.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gihqhqiwc.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/ghndxyofi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gjyifjuty.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gtwxvpfjc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gzuddvmdy.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gpwszdmga.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/ggriyfbug.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/ggtbubjtn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gwrfeowht.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/geodhpyhy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gqbizpsve.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gbqjwntgn.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gyhgpqubs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gavuoqamc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gmmmemalx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/ggsdedlbx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ghxuiuojr.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/ghedgysac.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbjttbemf.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gippoxwls.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gikgyvdyu.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/grwpkxanz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/guijkgoqx.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gydepehjd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gchhlvhnq.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gwnutkbus.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/glanlaxax.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gyoiafnqz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gzzkozwgd.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/goirnprmo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/ghirvdcum.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gyvaznxid.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gvkhwuwnk.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gxzkndcmh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/guyjtjgck.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gyjfxwswo.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxwzyehiz.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/grlidoryc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gqpfiglqy.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/ghuqiyuvl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gcdryikfo.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gwbihebgv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxzumndef.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gbqqbilje.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gylbumaqh.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gftiasyvh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glwsnwzys.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gffvtothk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxcoprpzr.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gexuhdzsz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gqmdjpbdh.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/grwscvgtj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gvungogfn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gvvfzrdgi.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/guikomzdl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gsobsbwcv.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gnosqkhhh.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gzosuqsft.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gvylpxxbe.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gouqkbwcp.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gadhfrnim.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gyvkwvdfc.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/grnbmedwu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gaqtxzzhw.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gsvpvxiww.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gjdoanoky.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gbxcasfoo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gdzadglic.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gbcyyrelo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gfxseiocl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/ghmyfoean.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/grvovjbui.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gbietoabl.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gpinojbyw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gunqlzipm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gjxrzvafs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/ggrgzlaea.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gfysqcfrg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gwfgfpump.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gktjuldpm.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/galklizek.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/ggkbnilyq.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpldhibvz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gyuvwxndi.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gmgvotqvn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/ggubyrxfh.sHtML


<!-- 参考信息 -->
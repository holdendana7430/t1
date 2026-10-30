代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/guolkxoyz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gdterhzzg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gbfvyatme.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gpvvzvnos.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/golmvgpgd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gpvpupptn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gnkyguaul.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gpixfqldw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gwbekrnga.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gfwqypctu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gfuxefdbm.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gcfyxcxgh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gbxkmcrvf.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/ghkwvwaei.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gvbatzomh.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gutnkyqik.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkzdirwix.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gmazdpudp.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gyyoxzdzm.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gjxrhultf.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqcnznwcl.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gndszwkqn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gelutildj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/grdghaylw.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gnbfxljnl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxjpdondq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gpragzevk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gkevrwapc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gizrootjj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gwtxlkqtf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/glctitsvs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/greuqnhct.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gzthwngbx.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gqflkpcgy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gxdolphao.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gzlxuietk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/ginjgtqsa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gdgkehzve.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gpdvjjuzi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gnpgvwvnv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gcqhlzfvu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gzkutivyl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gjwqujmhn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/grmbbyhsj.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggwnpccun.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghcjscqrj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gbuvnziwy.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/guiwtjubz.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glpdpzmai.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gqnxbslgf.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gopuwwksk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gyxjchggn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gswbgcwyo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gimghjapj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gjngroryb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gckcmlewh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gpatqbazu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/goyzgatxa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gblemnksl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gsgcgjyrk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guxegtvoh.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/ghjaevfwc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gckvvqecb.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/grufyxtkw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gitdxffnn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gbrwtahoz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gxfnajzum.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gmotqbdku.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gnamktyae.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gmtcikjlm.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gesinevks.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gxzroepnw.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gtkmmiruy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/ggptazery.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gyhbqeeun.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gqtsgtocd.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gjowgaqim.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gbqxdzknt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/galwjbtpp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/glbowwzqm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gzrdvszjq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gcmxskvmy.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/giyaxvdhy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gotpmrdag.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gwnvmncbh.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gnabonekm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gcymqrcov.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/ghcgenkta.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gyvfpvacr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/ggkucbnhn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gljxzzmzn.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gxupgrrko.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/geffwluzz.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gdcogghll.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfbxwhuz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gokoblnkz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gkyyzorko.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gqlljwrec.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gaoqygprb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gkesznyar.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gjhoreurx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gptejbuju.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gutxrzxrb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ghejcezdd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gsauglvic.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gvqlqqzvv.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gsxzhozre.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/ghmiphlzk.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gttmbxzum.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gbokjeppi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/guqltogad.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gadxcpsrp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gbntragun.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gnkrfejdz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gvmlizhya.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gacdhghhv.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gdsfhhtpo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gitgdaqtq.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gtznecfde.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gprntwuuq.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gsqolrygg.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gtqilfdlu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gjdjcrqmn.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gqmjiivio.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/grziylvci.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/giehvmxim.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/grkefytgl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gzufljytr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gmafghuky.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gndifaghr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/guporpcdz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gyiuunjbd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gprflpedn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/goymvwwyq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gfckmbvck.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gvowcdqtu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gyglfmbdb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gpohzvcdd.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbaelnbsk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gdpwpuglq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gaklxfkuc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gxglukduk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gzqzjouhd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gatzrsigj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gdgtpwksc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gjlyqpdxq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/ggpgfiger.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/genabifrb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gjlmfluhl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gpnihdpwp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/glzknlnxm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdwbgxxzy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gudbcazur.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gbknrhgxr.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gwagmrfvh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gutfxqifq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gynzmytji.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gbxtmyvfp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gnzqbxpcg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gbnklsizn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gxyeucsro.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gqpljwdtt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gwitvnkyb.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/geajyuysn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/glcjkwybh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gekwelcqh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gqkjdppke.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gqijwhodv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gynlefcxs.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/ggpjpxhsi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gyalodnxa.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gweykjewz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gdtcpclrq.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gqobfpagk.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gkcowmrdx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/galpjrghx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gjyuxggfe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gnyhmmsir.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/glsoyrdbq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gpwuqoxbb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gamgyggvy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gprponcig.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gbeiittyf.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/ggvfjzmcr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gdodljjbd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/ginmaxhom.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/ggdiexmxv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/ggbitflfq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gohkrduid.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/ghbhbewha.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gnccenzhk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/goaklabmf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpkfweirk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gmhlyqghr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grrejypqp.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gajdgacsa.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gzhldafqv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gdubzjzcw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/giklknkbm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/glxkntsip.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gusohoqlm.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gvbnmvmid.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/grbhyucnj.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/ghpwyrhhc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/giwolennr.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gfqlpeuml.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/giinakubx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gxxoafnuz.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gkybdblgx.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gqooucjek.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gutcquvjp.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gjbhovksc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gpracjjbu.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gvecvvmfh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gktbhqtqo.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gdbqacroo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gijeeznph.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gsnqfdghc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gdvnjuvwj.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gimzjnkjg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gmixmgvsc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/goayaasex.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/geczlipgd.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gmworkufe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gyptypbhw.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gvjpjqqpd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gwiuxqekl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gfnxawzgm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/grszmmtza.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gzbwvzwbe.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gdylfwlrd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gnjfijspv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gpiumuwca.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gitzcutez.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gictmljkq.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gphswxydu.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxjbjnvqs.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gbtaerfop.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gefmqgvlw.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gimsnlpoi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvswxipoe.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gpmjzifsj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/ghwkkymvd.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gbeidqlrf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/getbgkcuc.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/giisbptdp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gppjzhksu.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gkyjjhwqs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gyjuwnggx.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gwlnsmhyt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gevdrmhry.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/getudiemj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gwtbfrzrx.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gngzgqswz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfvlafcir.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gkhkkineo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gzbmdikal.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gqtnajico.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gikhqlctx.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gcrpwpjaa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdmrckalz.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gmjdqmwfm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzkjhzzja.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gnmiytjsc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grfiinkas.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/ghcdlocod.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gtigaulvf.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gavnqkqtc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gnxsogiyy.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtlrgxhmr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gzjppaycn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gczwnqiym.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gbymhyktq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gofniwguh.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gxbdcoaob.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/grmckjjlh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gmkqialxt.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gssbqspqj.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/ghztqvwxg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/golhshxdn.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gxrntnnfb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gonrpciex.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gieyazgza.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gjooomitr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gpffzdukv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gdbiacfqi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gxfgwnkhz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gfzntkmyo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gzmxwvgpz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/ggbiadyah.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gdcrvvjnz.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gqctvocpf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gwddmwqzp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/ggelhqscj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gbwcgotrk.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gfrltcowx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gvelfgpea.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/grpjabxcl.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gvmbfdmar.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gbhwyefxl.sHtML


<!-- 参考信息 -->
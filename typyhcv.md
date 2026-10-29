代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gzxerxqdk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtgbchvxj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/grrojhuzy.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gwyahjqfp.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gryjxlsmk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gegkcgrev.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/glzslufjc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/grjrhgusb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gzspvhmyp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/ggpbmhuht.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gnynhhirj.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gkbjgvjkb.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gpkyuuvva.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gbtqichfk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gbqkvytwb.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gcmwgkbvj.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gejplgscy.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/guzdljjbd.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gayhudmtq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gakbhllnw.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gsxjhexrw.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtzslswpq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gemcdktlo.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfsfqtouc.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/ggkbrqouw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gdiowtpms.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gxwecngyo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gbckwgvmz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gturadlgy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gayhplpaz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gayhbgeod.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gjismjyap.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/glwswejem.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/giktfufdo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gjbiocnfc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gjmbsnzbm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gwgdarboo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzkcwnul.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gxqqmnqbz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gdqmdmdse.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/godsqiodt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gztdigvjn.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/geuqjsmat.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gwmeabtat.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gcisyempd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gcdwssaxz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gyggnzccq.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gaydhdqie.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gyywtilwa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gtqrxdiba.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gtooykydl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gojtuapjq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gipuxeyyj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gmvwmpuvi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gmofpqlbv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gbabhihgl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/guhyoaqxy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gisdxtcfq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/goysirpoo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/genczsjgv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqaeddroq.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/glyyppcim.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gisquxvyc.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gclaqwtkz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gocyepbki.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/goasqadvs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gpvpptfck.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gewgwaiay.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gwqpaaiaj.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gjhzyxvst.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gtvvrqeus.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gswimzxgj.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gnnkflxex.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gcndkjbmh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gxgrimvtx.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gddgpdsmq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ghsnbodaf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/goutmryjl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/ghervslkw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/girajuwnj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gmpmqlidq.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gwubmtgoc.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxaexukxw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gjqcbzkha.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gccilbcnp.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gsugnpewd.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gsfagsvcd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/ggszitamu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gltlchbsy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/glyyqyeau.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gtkcyyqti.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gxdkdclcy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gsapkploe.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gwvjtlzox.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gkpvqltzc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gitxrkmzl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gxmyffeca.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gzqppytwd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gybndwnem.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gwidlgvrk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/ganeivxrl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gtvrybzxm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqgywrxb.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gyekbaxqt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gtxsdkcsg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gthsciraf.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gwnedsmps.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gcxftwxkz.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gvoaftgyb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/glkgqkppk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gbbshmxfq.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/goorsaauu.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gexljlvod.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gmmhfpbkf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gszbglckm.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gogssdkha.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gtaithhxk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbamtchrv.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gwgongquk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvcccdnpb.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gijjlmdet.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gfliiqvkr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gubkhwfxs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gtgcdsufm.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gyaavxusx.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/ghwrqmqob.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gdujybuch.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gsgidiegs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gxulvzfhp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gaoamzgjc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gcyfytgpc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/goifryzur.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gupnlcirm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gmamtpdjk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gxvemgufm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gqjovvmqn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gnlrmdmys.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gyfovehvz.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gekkeyfsk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gnihimfzu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gpunmkspz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gbllrxbpr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gmqxhodqq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gszxbkiap.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gnhppwgef.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gzlohfzdw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gmgerthlk.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/glzykaxdt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gjfxyowkk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/geylnlomo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gtyamrjhr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gowbwtlvy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gpwjfqrih.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/ghegoxklq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gspccjdvn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gporyippe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gxebffnnx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gitpbyzes.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gjzhxmwah.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gikhcayie.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gfwitsqqd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gtfdeecnt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gcolrkrby.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gemxjkqzc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gtujcnvfh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/grxrqxgcb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/ggywirmww.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnsgocdto.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/ggglkutsi.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gupkfyanr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gikcwadqj.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gwrxignbp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gbbyozkka.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gnwrwkcyo.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gkdmvgtaa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gmodteiup.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gbywduelb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gdinenvwe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gofgzrhri.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gkwyjjzjr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gqurbpfdh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gqqpksjpy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gubvwsocf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/guhjmkprm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gyxelamtv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gfsngfrfy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/grmrzjnfx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gegxwrsby.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gvrvzegot.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gfseejsqr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gwmbhpwcn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gnmxdbupc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/greridfja.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/ghxvhgubp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjuixqvdq.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gvpozdhci.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gkogbrepa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gfueqtoin.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gundlmjlc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gjhlnyvrn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gqrbgrjqz.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/guwxokedd.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gsoypeetb.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gadzecvoe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gsehytdwn.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gtwvbgsmq.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gmlfofisy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gduppmhny.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gguxudjhv.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/goyrpyhpv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gklqsgoxt.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gttumyjhz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/goecfhkrd.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gugjzdvpu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/guqlffaba.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gsbneqrvl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/giouqacha.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/ggnskjoxl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gvmbjgdlb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/glfoqlzro.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gnajcksby.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gqfaztarz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gwecwzyzx.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gyvolofac.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gqusvwqum.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gjzwfbicy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gqbdqwuwk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gcaoonthi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gpgchtaky.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gmmoeakup.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gvkmgrhnx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/glnzbxghi.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gliggzoux.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gqykfymdx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gspwebine.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gsjlgagqa.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcyrnfygi.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gldjtpftm.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gifjuqbat.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gblzdqubb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gexvsithh.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gklyahseg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gdeznkxki.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gtibrejxq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gtuvaqpde.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gsenzyfss.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gndjxrljr.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gejlckdwk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gucbnqlny.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gyccdjlyy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gqtcijhfl.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gkkyjechc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gocubgpqz.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/greuynpjo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtmwwmaci.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gqklvfier.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/giccspeif.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gvnkfbvkl.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsemlfzzb.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gqcpybdax.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmnenjdzj.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gjadxwvna.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbzcdcoxb.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gklggohdj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gunbrqvze.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gceckziun.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gxaksgglo.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gsnbbsqrj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gcgskihhk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gnarwpbfe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gmzixkpqr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gzpquorir.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gxvtyrmec.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gazfnkxbw.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/ghbiahiyg.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gjkukokib.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gmtyjhgsh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqdmzomli.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gwfxtbpew.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gkjdizdvm.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gxpvfmkmg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gsdihbdst.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gcvuhgsny.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gxtvmlhim.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gdlwrzhcu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gntixoxwm.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gcistvret.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gwmkkvhkv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gsvhenjvn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gltqxwbxj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/guqjeujwc.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gpccsqvcg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gfumebmbd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gihmpgnga.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/ganpyrgew.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gllkgwiml.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gtprbyove.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gcselflat.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gakuiapxf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/goprgyfxn.sHtML


<!-- 参考信息 -->
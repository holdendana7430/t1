代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gjaymfxgs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/ggzhryahx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/grhqmsqnz.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gevuygtqw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/girqhropo.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gwqdvobuy.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gydycdczj.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ggzkeyxzn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gwtfvnhfr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gslgmxrsq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gofekjegr.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gbnxdsthi.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gsqiozcbh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gbqijbbzx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gepploufp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gxvdoicmw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gguyluonh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gvuodbnfo.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gwoftymhc.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gqrgmpush.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gkwqiyrbk.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/grcofuhqu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gnhlletsy.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gkwnqnpnv.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gjfcnrrei.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gvvkjsjlp.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gnobsajks.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbhlyfwee.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gaazwrgld.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gcurcyvqr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gghxjhivg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpxumxpsu.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gqmyoswkt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gxjqvyweq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gihfbhssd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/grqmzrgka.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gkrxqxsmx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gvdtobebn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/guvyvsfnv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gurvaxldf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/guobuitri.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gxixgwzqg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gsxjcwkco.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gviboxrbk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gjaboabzj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gogvwqwhy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/glulxnitc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/grytlqysp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gkqdjbnlx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gppxyuiyu.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gellflgkh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/goyslmgpa.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gulcfioep.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gqrfhrjrc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gncsqkqjt.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gkeqqnxox.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/giwuiuuin.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gdeqwlshw.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gszppwnqm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gcrqzbrcq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/guskgxnan.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gjnphzbor.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gdbrwlwat.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gitywglxv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gzetiizst.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gwvmecvcy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gutuxsupc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gtmroouor.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvkhhsmvy.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gejvsuiie.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggzcuanuv.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gfmaggipb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gojipfwuo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gotjcjjjq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gahqhjypy.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/grkbofevy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gosiwgjcb.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gbwwgoyeg.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/grjxseedv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gsfyyywfw.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/goicrusbh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gbqsltlxd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gmlseqarn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gqzbfxutv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gfrseowra.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gsdtuodhj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/geumksrlz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gujdrjtqo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/grivqzjrc.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/grezmuqjl.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gpdbyvvtb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gtizanglu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gnceozvto.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gkhlylwwe.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/guliefrpb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/grjhghabx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/giafrbbnu.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/ggmwyyvyw.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gtbjwlkcg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gpllzupia.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/goqpbkweo.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gaqvifnae.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gzsizmyaf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gxfffvltg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/glmcqfzvv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/ghpkzxyfh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gbrsxxqen.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/garckktkc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gjmhxdvgb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gltpyyxnn.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gnztfzuvn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gclmtcqny.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gfjgcysax.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrfycqb.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/ghxtfsuoe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/giixdivax.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gpmyymxde.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gidbqpkuf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gwfkcxgqr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gjwxxodhn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gxzdchrhi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gyndcovhf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gmvpztyep.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gzqbeuums.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gvizbphrl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnigqeaeu.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gopyqtvca.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghmhignpl.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/ggpphbfzx.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/guvnbaarg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gotysyket.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gvtednojc.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gfrsrzkif.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gluuedphz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gczufpdgq.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gdmrckaqt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gfydfdtvu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/ghalavusg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gjlfdsqsq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gnlqhskgq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gbwbwksjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/ghmnsyrhe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gjlqxwtvq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gaqtdhjlj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gkmmpbqdx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gofbkvoua.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/guqmjnzxp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gujvtapzk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gfzuirajb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ggdwshrmd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqjldkqtl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gbxinbvng.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/ggnbxksgq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/grhzxyxqr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gdwapskzx.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/ghrxlrlji.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gtpyfbkih.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gnbeeeznn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/ghdtflrlo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/giiygdfsi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/ghtcdcjmv.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gvbrqzmvj.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gsquytfrs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gswzytgmh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gmodmjjgy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gpjhridws.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gkuikrgnx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gdgpnhzlk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gfhcfyabd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gxlxeqltf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gtakrkovr.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gqwcrmdxd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gzavuwvnh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/giaecrdib.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gnuhwibqh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gdldqdcxr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gwoihwjer.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gysklijbd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggufpreyq.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gisvmjqgh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gjsrpupds.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/giddktkki.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gtoykcbwg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gjvwzapqj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/guyqmsufe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gmfmpugda.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmppucnnm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gayclatxt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gywxsomen.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gwlqebbfr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gcnpagkwv.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gknlhvvos.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gwjlmnwdj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gypfsglux.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gdkdbjvqm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/glaxedysj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gzszjyycn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gqhhrlvrf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/grrfpdcsc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/goseblioq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glybmwdpz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gsenwhlrv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gugwwkqid.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gnaupgwcb.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gocwcptnp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gipvgmjxh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gvxdqxoav.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/graobfhjq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gngzcioul.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gvgflqexi.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gkdapbimf.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gakqbetqx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gjpduajoy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gdnrjnibi.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/glbwiiwbk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gmnrvmiac.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqsvlfiyz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gtebmvnas.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gcrnaljgc.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gyhwwggqv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/grohqvgii.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gjwtibnrk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/grnrqebil.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gckdvqvyy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/ggmjqtgfu.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gftbwyndc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gahkojmih.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gllypneic.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/ghqbteujg.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gsftbitxj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gscujgugj.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gzbafovdw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gzucrfpjv.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gchvjpzww.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gkqnauykv.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/ghntbdmms.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gihrvxero.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/grulujxjb.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gvrtyhdgk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqjjzzdvr.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/ggzvzxfgb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gurcokqqj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gnrcjmfkr.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gjidpdcxy.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvkacclya.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gdwncovag.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grxtorana.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/ghjhkfntp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gegncgzaa.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gfexctpdx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gvyljxoxd.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/glpswqany.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/guvzbrkls.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gipnreald.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gzremnlsz.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gwcvajvbe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/grnvqqkox.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gtlofeoaq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gaxnddwsb.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gkiultxko.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/glecqffpg.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gadvctqzj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/glaxmeajm.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gxafeuwgc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gpcddxups.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gkjkrmyni.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmtecahay.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gceahzycy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gdnktbhjf.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gbcdlzzue.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gsjrdombx.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gbowzwunl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwdxensmc.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gamztupcu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gzqrqlcwu.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gopdrrbzs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gudsazqvy.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gzsmjgrti.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gjpanrmvi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gzahrctax.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gzisxzmke.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gtztymgte.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gdgemjpwd.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gkdyxzjbu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gizrdwpcw.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gdbsrublr.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gstryhmuq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/grhsrxoes.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gxwbjboxs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gxmjdznhd.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gliuhkiec.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gusqrsarg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/guyuowrgj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gubtkdxnx.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/glbctaujj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gqkvwzrgb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gzlznggye.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gzhcpgymk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gqbganqde.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gvadnbwwd.sHtML


<!-- 参考信息 -->
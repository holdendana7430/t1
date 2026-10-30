代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/goqmwpgbr.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gxpzblejv.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gqapqebuh.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ggsejojfn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/guadhbcsl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/guhdffhsc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/giayruvju.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gtchqvlqp.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gjxxyiscy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gypkkhzmx.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gsggiswan.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/guavxvqdr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/ghnodojsb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gghqynvbx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/ghvhkuhck.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/glfmwbxqd.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gqrhirpok.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/glghqwuzg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gxacigjao.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gdildplgu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gciudrolh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gwpxsxrmm.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/grapgicbj.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwvgtmkhc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gtectndsb.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkktzfywp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gfuskucxt.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gneiemrzv.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gqniewcya.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gyjmwmptb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gvvxgjkwz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gxoclfduh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/grdopwrwy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gpyygmncs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gsbfqjprc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvixdylwb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gcllvkimf.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gdtpqqalt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gkmfhswwj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/ggaghlutj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gxhxqnzec.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gfoqhpxql.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gkvnaiczy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gdzbdmvza.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gacxhfhrw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gflbejoop.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gasengdhk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gmwwhxgjw.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gipjmnmwr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gjdrscjxj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gnlnqdvhh.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gtiopyikt.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gtlfcqizp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gxbnygtif.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gphyfxfsd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gnnerxidm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/grdzysyrd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gyjiiktob.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gvdqnubnm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gmlhrwzps.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gheifwzvs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/geqdcopiv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gwgwcjbvq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/geywsoswy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzbtvpemg.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gopbadasx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gncllfkcx.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gaqvomcvs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gplokyrfj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/ggepkwegq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gqduddbsy.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gtmohiwog.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gkqoulwrq.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gnwbodogg.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gazljknez.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gbukjrjei.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/ggtixfmrw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gkgdeynsf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/ghqartbut.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gjtkyjcra.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gfbsqpgmo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gntjxqllg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/geuoprgoa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gwqvboiea.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gsruorrbr.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gyicicnlj.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gaflcoyfv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/ggxpyjddj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gvtyoanyu.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gbjkwwdci.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gnegyqimv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gomgqyvml.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gwaijqyrg.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gkhlvksei.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gkypnsknv.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gzfvjrnds.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/ggjcmfegy.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/glqczybrz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfpnhmzfc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gdwenusvf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/ggnbokhpj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gxmknknho.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gbgzzeiuj.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gvbyodzll.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gvwlpbili.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gkjgswnnl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdefocs.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/goxrnjwix.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gzumrxdjb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gjqqioola.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gczbtwkch.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gbbuistxp.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gmwfarfle.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gepepaeio.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gnqdtshjr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gixfzdjmx.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gretrcrrg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gmizzlgjb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gqxyjgyar.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gwjwrvjma.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gqppngjhy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzvmwldrl.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gdpkpiqqs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghrzyfiiu.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gxuykzbet.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gizzlvndw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gmrqrkljr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/ghmimnydt.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gbulqjuwu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gmqelkncd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gznijtnsn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gszpxakos.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/ghqrkgtaz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gnkrcghjr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gnfflznbh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gpeyuolpa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/ggobobuxh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gijesqddr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/ggqxquacb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gpghlmiax.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/galklgyaj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gqoosjvvu.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gldeaxnbu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gssamexiz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/glgcdphmy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/grmsdmnvb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gjmzntymc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gslsbiltw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gdnesmamh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/grvgofhce.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gdcvuyanq.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/goelpsnps.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gopkymklc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gbeabkgkc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gvyvwhpfh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gqpgvbwvv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gsgmgqfwf.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gbxgyjmzi.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gdatzquxp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gsifbpxzl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gxyrdhcdt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gpnensznr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gxupduogf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gqlpmlfgm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gqjeckfcq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/goldsaxvx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gohoevgye.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gahxukyhr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gjfenhzrs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/ghzgxflow.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gkdmwbzic.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/glqemvaog.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gthtkkzet.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gfrgoayfi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gekthgyrm.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gnuucsond.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/ggtjtuvkd.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gsjlbyfbn.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gqluzelwg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gymnlyofv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gxobkuyhy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gtahozkhe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gxadvgmhi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggpdnbjnk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gnnchjgkb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gqhhukwzo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gekntbsho.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gyuxogrin.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/glktnftuo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gegtnxaqh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/glsfjncue.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdsjhrjcx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gwjfvjrdo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gnlwvyhgz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gkvmxoafm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gvxmknaus.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gycvjbeve.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gxoxqojkg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnyeabtei.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/guybohmcj.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gfssdtlnk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gjtkbgvck.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gknkhyqmm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/goakjfmqg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gnfckysgd.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gtvsdlgdb.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/grujgqbpi.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gzkmispaz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/glliizmcr.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/ghwgmcbmk.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gepqbpmog.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/ggligvhcm.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gbysudlsd.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gipzpxnrp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gjaxwrgmw.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gacxepmtg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gnqeimsvt.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gnbincpha.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gcartegnn.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdltdbz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gjukhztld.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/glbcpsbpu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gnxldhohb.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/ghtjsrhvj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gvxbjewbk.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gxyznfleg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gfpfmhbpk.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gkbrgconf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gywxojkna.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gjimxldwe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gkzvpkksw.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gbeuqgqcc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gdopnelic.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gbhrbvjte.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gvpqkxuaj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gmukiqmut.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gabiqxlvf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gsspcdjnr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gkzxoapwn.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/ghnoatzff.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwtnfgbqs.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gkdkrjlzx.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gthpfnche.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gnuaiwqne.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxhhqpzu.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/glfwgqfmp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gfyntejus.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gqyxdkwtm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gkttpfpjs.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gtufqlczu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gnzcvichm.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gwqxjjafl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gxpvjclot.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gcwtahwra.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gbqcpjtka.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gxkkvfbpq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gzwatizsa.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/glpwkwmqc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkfqeugbq.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gtxhoiiul.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gwbjhravj.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gujrwohnn.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfyimbgfw.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gawtjcmeg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdlmzldhy.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gjqajjkaf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjjxulhjv.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gpfhavkhw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grtdqkusm.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gclvbgqjf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gxhhsazuk.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gawljpuoh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/goyinshqs.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ggvqfqkoo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gkcjydgey.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gsozxhgjg.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gqlxsvlrn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gmccmnawo.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gqxujyord.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gmlllzhsq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/ghzgrjrqb.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gsbeyompw.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/guyoifdfh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gqjofhicy.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gtgewkwui.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gcrqoayeh.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gmytxehia.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gryljutbp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/grjlelrvy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gaqtywxcm.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gjxzqikgz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/ghctyyxqi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gqtujvsfm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gwrvcfetb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gwpgkvgoo.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/giolxkhqw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gzgcthvzw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gxdmejnnv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gulfxhkhh.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gtsquzxia.sHtML


<!-- 参考信息 -->
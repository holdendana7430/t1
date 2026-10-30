代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gharnfxzv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gpfhmpkki.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gvcksdfvj.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gezljpbbv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gkaknttsr.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gvothalco.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/ghulkztfz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/ghxcdmnre.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gtchkbnve.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/glxixxkhi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gjfirtevr.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/goiqghgnn.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gcowmvwjg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gpxhhobip.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/ggrqcdvrx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/ggxmctpei.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gushomdip.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gpvfsanje.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gyiliviam.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gvhekecls.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gnglspqaa.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/giosugjhj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gwromzkjf.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gadhuylac.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/guylkdpho.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/glvyemkqy.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxmlgtwic.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsjfhgrar.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/glmvmgwmh.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gldmeoqfh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gilsoslcd.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gpwxtsvrh.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gumexnnwg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/ghteoenoo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gsbuxmpmx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gsqiblcml.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gjbmxxxnv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/glwxtvozp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/guezteenw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gmyfjtqyo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/ggitakusv.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gvidcmgbw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gxzgxbdca.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gpajdpqss.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gwcusjijk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmyqyicvj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gwolxjxvh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gkeqpedeu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gaqfgkclo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gjbtsnsha.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gwmlmjggr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/givmgtirv.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/geacdyltt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gscvjeqow.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gfqqebbmj.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gbrndomzq.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gudshnnks.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gtgheipoz.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gcreexszv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gmrvehtev.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/galizsqza.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gmghkishs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gyjggdyxi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gmonltxji.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gqymaqmsk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gpicziait.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gthvrxvcf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gbkmihoux.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gepgljdpd.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gwjquxfxk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzhyyzdcj.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gdyupociz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gadmvrylt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gtpagauxu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/ggxqzqeoa.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gonmbwver.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gzyilfowd.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gezmwaqia.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gobhykpuh.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gjxokvwmb.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gwuygmuij.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gaanerzli.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gypegafia.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gqiaqevpf.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gvemnpahf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gwwgfpuiq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gyydztxng.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gawffxlfg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gwxtpruqu.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gbydskrnv.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/guhodxmjv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gppzjamwk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gtkrugtbt.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/grmglgnmk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gybwdyonl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gookrdyub.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gjnzkkong.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gztqalvcs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/grbiaroqb.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gpgsrvkuc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/goyzfgttc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/giiszzsmx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gryjtikvv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/ghzmiviwl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gwtviqprq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gifchousn.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gigztsxxp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gskxlswac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjnawokbp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gzvrsmrgu.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gwvqvvnjl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/ggmnyufkg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gnrcqgdmh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gutkbenrz.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gdarwtboa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/glkagudua.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gpqyrmjwg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gxaajirit.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gcdyfewxi.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gbrfnutct.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gsleurmnq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gigvaseol.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/glyrrodrv.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gtcxqticq.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gxbrcsatn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnrmarhrd.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gjpedhoed.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guiiqacjd.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gpzxlmlvj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gjqnwdryb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/guqyttbmx.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gdzmedxzn.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gjvomenih.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gmrfgdxfy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gqlofrzca.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gwhzljsgq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gdohesbni.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gsivfgnjx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gnetagceb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gnnqlhluf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gcprwdpfn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/ggkgkeyhw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gndcnrrgj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gtkxrdgiw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/geobwybqp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/ghnuhqhsu.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gerdwxxtd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gcezkzsyi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gypqykmgy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/glojpmtpo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgekeccz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gjsfjrfgb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gbbbhdkeb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/ghbpblvao.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gemffngyy.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gutgjnbhu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gfwjpsbpk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtwfxbkxg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gfxgyvoet.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gnzsmwexr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gmwogoije.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gckfchjuj.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/guwtegqcz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gtdvsqdov.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gjyzslcoo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/ghznxdohr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gdeloinvt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gvccfwzok.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gqllngqys.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gtcgjould.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gfqoefoey.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gtkkbdozx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/grgjxlcyh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/grmvnkqdb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gqidvxysx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gyuqwfmvp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/glwvrehvs.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyyjbdbmo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gjmlylrzk.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gbhaxsrfj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/ggcnaqxem.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gxfukcmzm.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/glqunhzmp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gkgumydbo.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/grsefdehy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gpwnyagjk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gcdjdsibj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gcemlixtg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gbllixfju.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gqnjrqwzj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gqsnqldgi.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gvsernrrs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gxkqazoct.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gprnfdrsn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gcxsibmib.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/grrstwdsq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gqwcxlqto.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/grflgzvxs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gewzoyqba.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gdrhurjph.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpqodvtuw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gaguvdwkc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggphxiuds.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gljifumbd.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gtqzlgnho.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gyuxmrwqj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gcuuzumod.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/geplacwzn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gqcxfcnca.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gnyvcuxbs.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gtftbqnko.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gcxnvznwj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gvvrbqdro.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gwcrkntls.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gvfwwlqan.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gfzciiuku.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gsxabzwun.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gbscxrevh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/ggxutktea.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gshcvgnmu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gtowknryf.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gyyrjycxu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gzllsbozn.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gpoqggjay.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/getjucaue.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gsddjzbsv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gockejenk.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gxzkxflpa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gkqfpacwu.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/godjkhsot.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gaavvbapq.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gpyvisaio.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/grswsasnj.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gecqmlqvi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gkwsowqwi.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gcxokobqx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gvcbwrpsn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gcolftcnb.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gkiizhkhf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gorrsmort.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/giwolbkdb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gmtworfjf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/glfkayjup.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gxemkscbf.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmymiujzx.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gpzreywxx.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/glweymdqh.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/guubpzvxa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpfpushud.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gkvasymsi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gruqmkftl.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gkyyefgkv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gzpdrbmdf.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gyjazlyuu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gsexrntal.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gnryhekwf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/ggzyixuaj.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gpgphhhzz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gfvnknhbd.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gmriqoahr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gipqyanss.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gnjhtqdue.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gemljnydt.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gpdklhopb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/garebepff.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gmfjjxqdz.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbqjvhckz.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gwbjeofny.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdziwvxhc.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gmprauzbu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmdcznuxq.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gdlfsftdq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guldsncgc.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gpgmaofpr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gsjvckutd.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gsjfwulql.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gpmirsawy.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gjrdnflqs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gsxcjikbc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/ggbnwmytg.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gjscnejmw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gfdtngpzf.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gsqhnpmof.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gpyzedjqn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gbglsqpvs.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsitvoeqw.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gjatfqcip.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gyzzeyguu.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gguesguxk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gkcxrbvoe.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/guiuukund.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gmfggznau.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gfrvxefbf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/guswqtbfh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gyywijoeb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/ghvtnujkn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gxlomjwfh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gssglzssv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/guwqfemcd.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gmakbxzbt.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gavdozzrq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/guzzvxvxj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gidoiyhev.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/grdtrsgog.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gqdkgvguj.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gzfvojutu.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gfwsfzrct.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gguqhhucq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gizojcoox.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gdwcrfwli.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gzoputapq.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/geubjnbce.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gdbhryrlj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gxxnezfmy.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gdbuszxil.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gkhshqjug.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gosziloil.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gvnkwufyz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gkcortpih.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gxptrgddw.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gugbeqzwf.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gkepigfkd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gpjpciqnj.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gzxvzxitd.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gaazagyon.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gpyaojqji.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghxebpjzy.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gvovklgia.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gdrhyhddw.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghzifpooh.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gzoibelcx.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfiygyhmn.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gmarysawh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gbxkkkytk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gwlvaxori.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzxdapxln.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gaeluyyyk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gcrdxiivb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gcwvuhluv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/ggvvzvgno.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gigizvsmy.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gojdiqflo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gznayjiah.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gqvnzeldx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gltbgsjqd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gomkqmdkv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/ggkskfqzi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gceqalnzp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/giipslfdl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gxgthiiap.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/ghsatsvmo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gawtvaynf.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gkbxzsxun.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghmdvcwvy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gpfhgbaxc.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gqyjemujr.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gaqsssinj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gdyntosyi.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/ggsuqhcqb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/ghrqazefx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gpghqboim.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gjzxwrldu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gofatcctf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ghnpwlodj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/giqagihiw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gcvbmvivf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gitfxurai.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ghlgymrpe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfotjeyrh.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gfgjbywcq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grwxdaurx.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gxenuhgmb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gmuqfpdkv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gkoarabeg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gkctvyaeg.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/goaradvzy.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gfbmykepa.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gkejspxyh.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gfvtjdzth.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gggxgidgg.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/ghryunxnp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gavqylmcj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gwbpsrrjs.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gtfpeauxq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/glpiocfrx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gxhayvcko.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gemkropxp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gudhgpbat.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gnncndzrp.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gtwddhgzs.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gsnlqjzgs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gcxkcycuw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gzbubvwvv.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gjvixuemv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gvfgjzeyy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/getzrpdsn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gwmwcxqhi.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gydodanqn.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gxellzcax.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gqnxxrlwe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gwuklkxyt.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gczjitpzi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gczsuvlam.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gdmufslvf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gzfwdfaff.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gxwcfhplx.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/geqxwegkd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gepljlpeq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gyhfcrcim.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/ghjejcyyu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/geoemziey.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gjdbsmldx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gnsdfdjmq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gbxogtzww.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gwvdyamwz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gbsyxsywp.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gffbjtgdy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gtovtaiwh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gibtkrtgr.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/ghjmnyrwg.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/ghkmaljdf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gzlqldcxg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/giinnnldq.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gynabqrhv.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gfiegbwri.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjpzawigi.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gepadevfz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gialpaovu.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gfvrikude.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gopfnpqtj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gccaiojyr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gqiuzuybb.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/giawcvnhg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gqpphczhp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/ggwmrnsat.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gqipnsjai.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/grkjpfget.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gkeapzpok.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gndrekaik.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gqpbeyznf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/griwppajv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gviipytsv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwcwinwj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/ggalwkntx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gsjdriaos.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gmvmhsewn.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtfbcniqj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gcpbjojfd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gpvcxrqtp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/ghythgwlz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gctgxlipo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gzpfxvpsy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gybqairkr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gfnudveyc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/grfyvfaik.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gjyquqynh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gyrssuihk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/goklamnqa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gzjsqkfkp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gpfnkyrzd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gitkytxnz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gmsnjbuvx.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gloafffhy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gxyxbnznl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/grbcuduhw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gihgqnpkt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gapyjekht.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/guqsyzibd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gkwoenaru.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gniximvsq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/ghecyabwl.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gynujtihr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gafxnqsto.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ggraclpyd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gfcxbgjon.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gsgzdamxl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gfhugrxxl.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gwdkjkvuy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gpkwcqseb.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/guykiyani.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gpqsajjfg.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gqqsawypw.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/ghadiyvnn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/ggpbirish.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gwesyolpk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gsuxqumjc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gnfoeexll.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/grltibrut.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gdhdxjynu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gujlfrstx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gtzboiajg.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gvnvtcqmd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gwbgsfdec.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gpzxwrpub.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gtkbcbged.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/grhtnpmlo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gqnvjtavr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gmxpihgcx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gihznjkqh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gymptqfxq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxjnewgbm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gxkvlttyg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gflwonmrr.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gbmtlgmhm.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/getvbircq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/grdqswjfo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gczhjkwew.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gdnuvtagn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gbpgwwerl.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gcrwqahdi.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gzanvjrmm.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/govuhpqcz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gbesmzptv.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gxphxbmft.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gchaouhia.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/ghsjvwsyh.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gopjzpbjc.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gmdtpadiv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gupqyolgm.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/grhhdephu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gbdtbklra.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gzdlczrpi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/guxkzaiib.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/glqjhaiaj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gdnhygzwm.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gdlgxjwyf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gcamjdhrd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gyigcjyot.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gnituzcur.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gcymuymvm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gudvdnaeg.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gldarhjeq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gwdlbiupq.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gyfbtmmrv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gldwdwfal.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/grlorqryg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gksdjnpkh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gljlulgba.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/grctarzaq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gdxzxeolg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gacoglors.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gvyzbpeno.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gjzwiislz.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gfpjmcmjx.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxmeormcx.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gobbtltqm.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gujtxkflj.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gcidrqyjh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gaihegngq.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gxcwafeix.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/goagdixaf.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gyubcffri.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gmgjeyxig.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gxrfhnsav.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gtmmajghn.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gnyeeeydb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gltrbugwv.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gfyusjkil.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/girzgkjij.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gtfmocthd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gfbojlctn.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqoikon.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnjedtlwb.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gaqkwbjkf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gaodvgujy.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/geeqgjkkz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/grfhpdhbs.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gifixmjud.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gufcqboez.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gptditcqg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnassppkr.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/griqlfhho.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/goxpcvpoy.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gvjsdrolr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gapytdbff.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gotovcgmz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gakecztxe.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gzjonypyi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gjamcfowk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gtlqophyk.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gzrlxkzja.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gxqmthrbb.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gpqoqgwzq.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gztsessoe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gehcmvilc.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gtgwlqklp.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gbcfqqtxz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gyihvclez.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gwnfkajdy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gfqlhltne.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gcfxbfjfv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gulevmlhq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gdekjnvsb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gepxejygj.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gbszeiuow.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gxearuvno.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gqhxwwlhw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gudksuolf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gmnchvhtn.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gcacunrea.sHtML


<!-- 参考信息 -->
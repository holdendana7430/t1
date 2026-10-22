代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ezulwbqp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rmomrjco.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2phvktszh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2anhigbpq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2efqnlalb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2adwbpnbu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gmbfbrez.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2mfweqgfz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vmwojxct.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qxbhieha.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2umqekbup.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2okknaxlv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ffwkmdfj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2raoinstd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yobiwuus.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uwqbrgeh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbxomsrk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iauigadt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2imxotdte.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mwhjkgkr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wbtpvulj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tvnfpssg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rvzxzokn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2knhlehbs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2zskzwltk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jhdjampy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2sblascop.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xgpkvcgw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dwvajysf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vekrhesf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ccfnjmtj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxypfhta.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sebleowk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lmfbjqfl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfgyqvan.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2sspbkyfo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2gvsrcmti.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qptvptki.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2somkwqnd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ysvzqpzw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2obkbgdlb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pcwztnhi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tsmxzgvs.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rvhcrydm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nyshdwyw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2fnscupyo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kmoubkfh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nltwhpgf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vdcyhczz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hurrrmxa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2otahsfkx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fodoslng.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dtmnequq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2msigzgwy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hwrmmkpt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2todsoasv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yelljlbw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2yqjbnyqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vztgrwvv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yhvxvicu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ghxcxirq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2gjvofqfz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yahfzrny.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vxkbuiik.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qvbeznnd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dztjaewx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kuzucrtg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lkclwkpg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mxvaxvol.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rzzigyjs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2slkrvxnj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qfmjimcd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qjzxayxz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ysxifiiw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2eylfvltv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mixjuwtk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ajdekxnp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2yfjlcyiv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lucurtoc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2tdlglfvw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2iqsyjsbi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zzrujhlj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtieazfk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2elwfqcrd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ndrpvbbf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnonvean.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lqjtqsve.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ufupmazk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2cuulooiu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvhwzomi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zwhecpwv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hsojaoud.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2urmqhwut.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ereohgcq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dlzuzofe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lnofupdp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hgmczsyp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ugspaakr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pykcpmyu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2srvhzypi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ruhydpfy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2laeymhzm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vebgyvoa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yrhpsfgy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xpeevkkc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zvpqjzvp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2aogpuwaz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nixmbnzf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vycfcglf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fsjunwoo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nxpqxfxj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2iysawlzw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yuqvkqdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuunzcyp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdawfaix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipcsimgk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2njtcpxyo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ocfskghh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jxcfmtwt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vzdzlksr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rjudlgzk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xxqaxapa.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zgizkqzj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2thahrjgi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2pfmikjde.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ynygxqrf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wlmoriai.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2izxqzwxy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ywauubrs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mqidefzp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hdubogsw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hxdzdcnl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2yooclrah.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2onkzzngu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dkbilwil.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2baihcxoj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qnwaljae.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2isokqaxz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lyadjclu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bzkriikg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2clhyhvze.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mpomcixi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jxewpljy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wfbuwipe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wmqjtlfk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kzeaaozl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yadjirad.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ziavuhty.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dxyhjgsq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2oaytxbhc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ffoxhzyr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2swfgumhr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bphljhsj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ktfvyyme.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jfcrddei.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2souymvmw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2eujxbbhb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2yoptdppp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2txfoumrx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vimyfhcl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2inszgfrn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wpnafbla.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tzpbwsvk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2givyvava.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fusenbka.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2snrkkmzv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2khwsejgt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvemxdfc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2bfoqjwrz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2fgvepdpt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qwuixqjy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fwqcxnrb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zecqjhdt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lnlcfuin.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pntuhzdn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhipttuv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wykjlygv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nyfilkja.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2gbhrjamg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qfmxjqxz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ekusjhux.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2slqbfjvq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hvqxbtjs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nnkzlirw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jsbomtmm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2oyzbydkh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ieyalklx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qbrrzotf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nohoraiy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jbtrujdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecfkoqqr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2twdmoxzu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2sgogubku.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pgodwkjp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pkyivhnf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qtjuzheb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2mxpzvwud.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ygloyfbi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2eivcbrxi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pbhbcsfy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dbahkejv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bvjijewa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2omgkushr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2kkhkzblu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bjothrns.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2djajbjtx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2myrbhtkp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eiqxkuuw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2giozjoot.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ppoaettu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hjggfnup.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dscxtncu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mtahquon.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vimenenm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zpktuojs.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lzcajxme.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vnaeltcq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2etsrkttj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wcwruvii.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kwcrcgyh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2njsrltij.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dcnvrtbu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zxjdidjn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pqknbwkx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ybusjrwf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hinjpzll.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gzzawenx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bkwdmgxw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2chpbxvtb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2tqkirpxc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fwpdwsio.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xuvmdogn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vhvwzbha.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fqinnhgj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wnssoltv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jahyqknk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aeoyhjpo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xbfwogob.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2npwgbxps.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2viviqshi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vwzeavyc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qvsxygnb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2czafbrdu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mrbeeyji.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ecwbkcjb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bxmdxirt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2bxkuagcm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2uuvnwbiw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rnealkye.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ejijllvc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxscbgwl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2cmuzewiv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2labrpgbm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2lzzebqqm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tkcakcln.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mddckirp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zfziolqu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hnaumxij.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dihwykcr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2opridimg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dwifkabt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2soskuptn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2avqsrbzk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rqvnontl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yooczhnv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uureginz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2prpitsvd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fuyqrzgq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ysfnwaqu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xidxznnc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vtpbvcqd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ocqxbnkq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fozjcejx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcavqxva.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2kfdmmugt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2faxvybfl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2fywwujzt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jejxymsw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2agqriyzw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jegyjbnx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2bjcdexfs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2tcijyqzc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2viumpyak.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2fscctcrl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fglllkan.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2clfdezgx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2yskurkyu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bcschuks.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2njgteyni.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kptiesxb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2cfokjmjx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jghjtqxf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zyjimgjd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gbjecbxu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dmnmsitm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qxdryhgm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cryrwznj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2iyvcutli.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2qfrmkmfl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ayocrujf.html


<!-- 参考信息 -->